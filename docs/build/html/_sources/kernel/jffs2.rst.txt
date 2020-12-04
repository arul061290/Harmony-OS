JFFS2
=====

Overview
--------

JFFS2 is a journal-type file system implemented on MTDs. JFFS2 is mainly
used in NOR flash memory. It is readable and writable, supports data
compression and write leveling, and provides crash/power failure
protection.

There are many differences between flash memory and disk media.
Therefore, running a disk file system directly on flash memory causes
poor performance and security. JFFS2 is introduced as a file system
specially designed for flash memory.

JFFS2 in the OpenHarmony kernel is mainly used to manage files of the
NOR flash memory and supports multiple partitions.

Important Notes
---------------

-  The JFFS2 file system is used for NOR flash memory, and NOR flash
   driver APIs are called. Therefore, before using the JFFS2 file
   system, ensure that the NOR flash memory is available on the hardware
   and the driver is initialized (the return value of **spinor_init()**
   is **0**).

-  The system automatically aligns the start address and partition size
   based on the block size. The valid partition number ranges from 0 to
   19.

-  **mkfs.jffs2** is supported. You can change parameter values based on
   service requirements.

-  When you use **open** with the parameter **O_TRUNC** to open a file,
   the file content will be cleared.

-  You can perform the following operation on JFFS2 files: **open**,
   **close**, **read**, **write**, **seek**, **opendir**, **closedir**,
   **readdir**, **readdir_r**, **rewinddir**, **statfs**, **sync**,
   **remove**, **unlink**, **mkdir**, **rmdir**, **rename**, **stat**,
   **stat64**, **seek64**, **mmap**, **mount**, **umount**, **chmod**,
   and **chown**.

-  JFFS2 files can be mounted in the read-only attribute. When
   **MS_RDONLY** is carried in the **mount** function, the read-only
   attribute is enabled. All APIs with the write attribute, such as
   **write**, **mkdir**, and **unlink**, and files that are opened not
   by using **O_RDONLY**, are rejected and the error code **EACCESS** is
   returned.

Development Guidelines
----------------------

**Adding a JFFS2 Partition**

Call **add_mtd_partition** to add a JFFS2 partition. This function
automatically names the device node in the format of **/dev/spinorblk**
plus the partition number.

The **add_mtd_partition** function has four parameters. The first
parameter indicates the medium, which can be **nand** or **spinor**. A
JFFS2 partition is used on **spinor**, whereas **nand** is provided for
a YAFFS2 partition.

The second parameter indicates the start address, and the third
parameter indicates the partition size. Both parameters are transferred
in hexadecimal format.

The last parameter indicates the partition number, which ranges from 0
to 19.

::

   if (uwRet = add_mtd_partition("spinor", 0x100000, 0x800000, 0) != 0) {
       dprintf("add jffs2 partition failed, return %d\n", uwRet);
   } else {
       dprintf("Mount jffs2 on spinor.\n");
       uwRet = mount("/dev/spinorblk0", "/jffs0", "jffs2", 0, NULL);
       if (uwRet) {
           dprintf("mount jffs2 err %d\n", uwRet);
           dprintf("Mount jffs2 on nor finished.\n");
       }
   }

   if (uwRet = add_mtd_partition("spinor", 0x900000, 0x200000, 1) != 0) {
       dprintf("add jffs2 partition failed, return %d\n", uwRet);
   }

After the partition is added, you can run **partition spinor** in
**shell** to view the information about the spinor flash partition.

::

   OHOS # partition spinor
   spinor partition num:0, dev name:/dev/spinorblk0, mountpt:/jffs0, startaddr:0x0100000,length:0x0800000 
   spinor partition num:1, dev name:/dev/spinorblk1, mountpt:(null), startaddr:0x0900000,length:0x0200000

**Mounting JFFS2**

Call **mount()** to mount a device node and mount point.

This function has five parameters. The first parameter indicates the
device node, which must match the **add_mtd_partition()** function. The
second parameter indicates the mount point. The third parameter
indicates the file system type.

The last two parameters indicate the mounting flag and data. The default
values are **0** and **NULL**, respectively. This operation can also be
implemented by running the **mount** command in **shell**. You do not
need to specify the last two parameters.

Mount a JFFS2 file system.

::

   OHOS # mount /dev/spinorblk1 /jffs1 jffs2

If the following information is displayed, the JFFS2 file system is
mounted:

::

   OHOS # mount /dev/spinorblk1 /jffs1 jffs2
   mount OK

Now, you can read and write the NOR flash memory.

**Unmounting JFFS2**

Call **umount()** to unmount the partition. You only need to provide the
correct mount point.

Unmount JFFS2.

::

   OHOS # umount /jffs1

If the following information is displayed, the JFFS2 file system is
unmounted:

::

   OHOS # umount /jffs1
   umount ok

**Deleting a JFFS2 Partition**

Call **delete_mtd_partition** to delete an unmounted partition.

This function has two parameters. The first parameter is the partition
number, and the second parameter is the medium type. This function
corresponds to the **add_mtd_partition()** function.

::

   uwRet = delete_mtd_partition(1,"spinor"); 
   if(uwRet != 0) {
       printf("delete jffs2 error\n"); 
   } else {     
       printf("delete jffs2 ok\n");
   }

   OHOS # partition spinor 
   spinor partition num:0, dev name:/dev/spinorblk0, mountpt:/jffs0, startaddr:0x0100000,length:0x0800000

**Creating a JFFS2 File System Image**

Use the **mkfs.jffs2** tool to create an image. The default page size is
4 KiB, and the default eraseblock size is 64 KiB. The image size adapts
to the source directory and is filled with 0xFF, which is an integer
multiple of the eraseblock size. The default command is as follows. If
the actual parameters are different from the following parameters, use
the actual parameters.

::

   ./mkfs.jffs2 -d rootfs/ -o rootfs.jffs2

**Table 1** Commands

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row325613545615">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p153851336772">

Command

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p43852366714">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   </tr>

.. raw:: html

   </thead>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row125715410619">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p20385103615715">

-s

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1338510362717">

Page size. If this parameter is not specified, the default value 4KiB is
used.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row787741814720">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p538673616710">

-e

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p6386123612719">

eraseblock size. If this parameter is not specified, the default value
64KiB is used.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1160020211719">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p83861361079">

-p

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p538612361575">

Image size. If this parameter is not specified, the source directory is
used by default, and 0xFF is filled as an integer multiple of the
eraseblock size.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row151563245714">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p183864361579">

-d

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p238618361573">

Source directory of the file system image.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1323210319714">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p103867369710">

-o

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1938603617710">

Image name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>
