Kernel File System
==================

The OpenHarmony kernel supports the following file systems: Virtual File
System (VFS), Network File System (NFS), RAM File System (RAMFS), File
Allocation Table (FAT), and Journalling Flash File System Version 2
(JFFS2).

The table below describes the functions of these file systems.

**Table 1** File system functions

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row6331184864111">

.. raw:: html

   <th class="cellrowborder" valign="top" width="11.559999999999999%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p17644161411438">

File System

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="88.44%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p116441414184312">

Function

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

   <tr id="row371213562318">

.. raw:: html

   <td class="cellrowborder" valign="top" width="11.559999999999999%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p37130569316">

VFS

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="88.44%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1771335615316">

In essence, VFS is not a real file system. It is an abstract layer on
top of a heterogeneous file system and provides you with a unified
Unix-like file operation interface.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row189255844219">

.. raw:: html

   <td class="cellrowborder" valign="top" width="11.559999999999999%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1564481494319">

NFS

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="88.44%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p764561414434">

NFS allows you to share files across hosts and OSs over a network.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row17332194820411">

.. raw:: html

   <td class="cellrowborder" valign="top" width="11.559999999999999%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p2064561415435">

RAMFS

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="88.44%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p12646614204320">

RAMFS is a RAM-based file system. All files are stored in the RAM, and
file read/write operations are performed in the RAM, which reduces the
read/write loss of the memory and improves the data read/write speed. It
provides a RAM-based storage buffer for dynamic file systems.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row16332174894116">

.. raw:: html

   <td class="cellrowborder" valign="top" width="11.559999999999999%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1864571410433">

FAT

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="88.44%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p364511141434">

There are FAT12, FAT16, and FAT32. FAT is often used on removable
storage media (such as USB flash drives, SD cards, and portable hard
disks) to provide better compatibility between devices and desktop
systems such as Windows and Linux.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1880218157414">

.. raw:: html

   <td class="cellrowborder" valign="top" width="11.559999999999999%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p19645814144312">

JFFS2

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="88.44%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p8645161454314">

JFFS2 is a journal-type file system implemented on Memory Technology
Devices (MTDs). It is mainly used to manage files of the NOR flash
memory. JFFS2 used in the OpenHarmony kernel supports multiple
partitions.

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

-  `VFS <vfs.md>`__

-  `NFS <nfs.md>`__

-  `RAMFS <ramfs.md>`__

-  `FAT <fat.md>`__

-  `JFFS2 <jffs2.md>`__
