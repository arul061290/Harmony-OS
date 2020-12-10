Developing the First Example Program Running on Hi3516
======================================================

This section describes how to modify, compile, burn, and run the first
program, and finally print **Hello OHOS!** on the develop board.

Acquiring Source Code
---------------------

You need to acquire `Hi3516 source
code <https://repo.huaweicloud.com/harmonyos/os/1.0/code-1.0.tar.gz>`__
and download it on a Linux server. For more obtaining methods, see
`Source Code Acquisition <../get-code/source-code-acquisition..rst>`__.

Modifying a Program
-------------------

The code of **helloworld.c** in the
**applications/sample/camera/app/src** directory is shown in the
following example. You can customize the content to be printed. For
example, you can change **OHOS** to **World**. You can use either C or
C++ to develop a program.

::

   #include <stdio.h>
   #include "los_sample.h"

   int main(int argc, char **argv)
   {
       printf("\n************************************************\n");
       printf("\n\t\tHello OHOS!\n");
       printf("\n************************************************\n\n");

       LOS_Sample(g_num);

       return 0;
   }

Compiling Code
--------------

On the Linux server, execute the **build.py** script stored in the root
directory of the source code package. The result files in the
**out/ipcamera_hi3516dv300** directory.

::

   python build.py ipcamera_hi3516dv300 -b debug

Burning Images
--------------

This method applies only to development boards that have network ports,
for example, the Hi3516DV300 development board. The PC and the
development board must be connected to the same network through a
network cable.

   |image1| **NOTICE:** If the development board fails to connect to the
   PC, check whether the firewall settings are correct. For details, see
   problem 2 in FAQs.

1. Install the USB-to-serial adapter driver and obtain the serial port
   number.

   | **Figure 1** Successful driver installation
   | |image2|

   1. Power on the board and connect the serial port of the board to the
      Windows workstation.

   2. Install the driver.

   3. Open **Device Manager**, and then check and record the port number
      of **Prolific USB-to-Serial Comm Port**. In this example, the port
      number is COM11.

      After the driver is installed, right-click the device to uninstall
      it if a yellow exclamation mark is displayed on the device icon.
      After the driver is reinstalled, restart the PC as required.

2. Add an IP address 192.168.1.3 in this example to the interconnected
   port of the board.

   | **Figure 2** Adding an IP address
   | |image3|

   1. Choose **Control Panel** > **Network and Internet**-> **Network
      Connections**. Right-click the network adapter connected to the
      board, and choose **Properties** from the shortcut menu.
   2. Double-click **Internet Protocol Version 4 (TCP/IPv4)** and
      right-click **Properties** from the shortcut menu.
   3. Set the IP address and gateway according to the preceding figure.
   4. Click OK to save the configuration.

3. Choose **Board Configuration** and enable the hi3516dv300 board in
   the **Board List** area. The hi3516dv300 board will then be added to
   the **Board Configuration** list.

   | **Figure 3** Adding the hi3516dv300 board
   | |image4|

4. Open the IDE and configure the content to burn over the network by
   following the sequence in the following figure.

   **Figure 4** Network configuration on the IDE

   |image5|

   1. Choose the Hi3516dv300 board.
   2. Click **Burn**.
   3. Set **Burning Mode** to **network**.
   4. Select the IP address **192.168.1.3** from the drop-down list
      after clicking the refreshing icon.

5. Select the flash memory type and set the burning addresses.

   **Figure 5** Burning parameter configuration

   |image6|

   1. Select **emmc** from the **Memory Type** drop-down list as the
      **flash memory** type.
   2. Click **New** in the **Burn Files** area to add three file
      configuration records, fill **OHOS_Image.bin**, **rootfs.img**,
      and **userfs.img** in the **out/ipcamera_hi3516dv300** directory
      to File Name one by one, and set the start addresses and file
      sizes according to the configuration in the preceding figure.
   3. Click **Save**.
   4. Click **Burn** to start burning.

6. Click the text box on the top area of the IDE and select a serial
   port number from the drop-down list, for example, COM11.

   | **Figure 6** Selecting the serial port that is connected to the
     board
   | |image7|

7. Start burning. If the following prompt message is displayed, you need
   to manually power off and then restart the board.

   **Figure 7** Prompt message

   |image8|

8. Check that the burning is successful.

   | **Figure 8** Successful burning
   | |image9|

Running an Image
----------------

1. Connect to a serial port.

      |image10| **NOTICE:** If the sconnection fails, rectify the fault
      by referring to problem 5 in the `FAQs <faqs-0..rst>`__ section.

   **Figure 9** Serial port connection

   |image11|

   1. Click **Serial port** to enable it.
   2. Enter the serial port number “com11” and press **Enter** until
      **hisillicon** is displayed.
   3. Go to step 2 if the board is started for the first time or the
      startup parameters need to be modified; go to step 3 otherwise.

2. (Mandatory when the board is started for the first time) Modify the
   bootcmd and bootargs parameters of U-boot. You need to perform this
   step only once if the parameters need not to be modified during the
   operation. The board automatically starts after it is reset.

      |image12| **NOTICE:** The default waiting time in the U-boot is
      2s. You can press **Enter** to interrupt the waiting and run the
      **reset** command to restart the system after “hisillicon” is
      displayed.

   **Table 1** Parameters of the U-boot

   .. raw:: html

      <table>

   .. raw:: html

      <thead align="left">

   .. raw:: html

      <tr id="row1423410183818">

   .. raw:: html

      <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1">

   .. raw:: html

      <p id="p623461163818">

   Command

   .. raw:: html

      </p>

   .. raw:: html

      </th>

   .. raw:: html

      <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2">

   .. raw:: html

      <p id="p42341014388">

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

      <tr id="row1623471113817">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p102341719385">

   setenv bootcmd “mmc read 0x0 0x80000000 0x800 0x4800; go 0x80000000”;

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p92347120389">

   Run this command to read content that has a size of 0x4800 (9 MB) and
   a start address of 0x800 (1 MB) to the memory address 0x80000000.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row12234912381">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p172306219392">

   setenv bootargs “console=ttyAMA0,115200n8 root=emmc fstype=vfat
   rootaddr=10 M rootsize=15 M rw”;

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p13489329396">

   Run this command to set the output mode to serial port output, baud
   rate to 115200, data bit to 8, rootfs to be mounted to the emmc
   component, and file system type to vfat.

   .. raw:: html

      </p>

   .. raw:: html

      <p id="p12481832163913">

   rootaddr=10 M, rootsize=15 M rw indicates the start address and size
   of the rootfs.img file to be burnt, respectively. The file size must
   be the same as that of the compiled file in the IDE.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row18234161153820">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p823417118386">

   saveenv

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p32341616389">

   saveenv means to save the current configuration.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row192345113811">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p7235111183819">

   reset

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p123781411114016">

   reset means to reset the board.

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

   ..

      |image13| **NOTICE:** **go 0x80000000** (optional) indicates that
      the command is fixed in the startup parameters by default and the
      board automatically starts after it is reset. If you want to
      manually start the board, press **Enter** in the countdown phase
      of the U-boot startup to interrupt the automatic startup.

3. Run the **reset** command and press **Enter** to restart the board.
   After the board is restarted, **OHOS** is displayed when you press
   **Enter**.

   **Figure 10** System startup

   |image14|

Running a Program
-----------------

In the root directory, run the **./bin/camera_app** command to operate
the demo program. The following figure shows the compilation result.

**Figure 11** Program started successfully

|image15|

.. |image1| image:: public_sys-resources/icon-notice.gif
.. |image2| image:: figures/successful-driver-installation.png
.. |image3| image:: figures/adding-an-ip-address.png
.. |image4| image:: figures/adding-the-hi3516dv300-board.png
.. |image5| image:: figures/ide.png
.. |image6| image:: figures/未命名图片2.png
.. |image7| image:: figures/selecting-the-serial-port-that-is-connected-to-the-board.png
.. |image8| image:: figures/reset2.png
.. |image9| image:: figures/successful-burning.png
.. |image10| image:: public_sys-resources/icon-notice.gif
.. |image11| image:: figures/chuankou1.png
.. |image12| image:: public_sys-resources/icon-notice.gif
.. |image13| image:: public_sys-resources/icon-notice.gif
.. |image14| image:: figures/qi1.png
.. |image15| image:: figures/qidong.png
