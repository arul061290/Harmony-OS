Setting Up a Development Environment
====================================

Environment Requirements
------------------------

Hardware
--------

-  Linux server
-  Windows workstation (host computer)
-  Hi3861 WLAN module
-  USB Type-C cable used to connect to Windows workstation and Hi3861
   WLAN module

`Figure 1 <#fig1651211924914>`__ shows the hardware connections.

| **Figure 1** Hardware connections
| |image1|

Software
--------

**Table 1** Requirements on the development platform

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="ra9df6acc53154b819d5f86d885d994de">

.. raw:: html

   <th class="cellrowborder" valign="top" width="12.41%" id="mcps1.2.5.1.1">

.. raw:: html

   <p id="a999bb40532eb4f74a7383e1e776bb94a">

Hardware

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="12.389999999999999%" id="mcps1.2.5.1.2">

.. raw:: html

   <p id="ae63cf791fbe348d3b907d20fc4927df8">

Software

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="46.21%" id="mcps1.2.5.1.3">

.. raw:: html

   <p id="a54c4c80c43c84cb187342865a1d2b51e">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="28.99%" id="mcps1.2.5.1.4">

.. raw:: html

   <p id="a11e8d096fb204378a63d8805cd6d1f88">

Remarks

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

   <tr id="row117591159175819">

.. raw:: html

   <td class="cellrowborder" valign="top" width="12.41%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="a0c1290183f2548898dbfc516a4db2c4b">

Linux compile server

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="12.389999999999999%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="a687efa8001f140488dc1da9a2ee8f6d1">

Operating system

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.21%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="ace724e00c9094eccb8c600d6ad426ed8">

Ubuntu 16.04 64-bit server or later (Use bash as the shell.)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="28.99%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="a4d0e2c8444484554ab58949ce322be32">

You can develop programs on the Windows workstation or Linux server via
a remote login.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="r85c4bf56ff3244e48db9d2f5b622b340">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="a8e99fd0262cb4489b70cf86c2144c294">

Windows workstation

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="a44d6164ce2e9421f9ade362f600c2815">

Operating system

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="a1c17349e334a44ada5c5f150457fe17d">

Windows XP/Windows7/Windows10

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

Build Tools for Linux
---------------------

The following table describes the tools required for setting up the
general environment for a Linux server and how to obtain these tools.

**Table 2** Development tools and obtaining methods

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row122993276512">

.. raw:: html

   <th class="cellrowborder" valign="top" width="25.562556255625562%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p1829914271858">

Development Tool

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="20.7020702070207%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p429918274517">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="53.73537353735374%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p12997271757">

How to Obtain

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

   <tr id="row1829915274517">

.. raw:: html

   <td class="cellrowborder" valign="top" width="25.562556255625562%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1629902717511">

gcc_riscv32

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.7020702070207%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1219863434519">

Executes script cross compilation.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.73537353735374%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p14145637348">

https://repo.huaweicloud.com/harmonyos/compiler/gcc_riscv32/7.3.0/linux/gcc_riscv32-linux-7.3.0.tar.gz

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row430016273514">

.. raw:: html

   <td class="cellrowborder" valign="top" width="25.562556255625562%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p330015271158">

Python3.7+

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.7020702070207%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p43003270510">

Executes script compilation.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.73537353735374%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p18254155164617">

https://www.python.org/ftp/python/3.8.5/Python-3.8.5.tgz

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1397335913612">

.. raw:: html

   <td class="cellrowborder" valign="top" width="25.562556255625562%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p097355911620">

SCons3.0.4+

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.7020702070207%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1973195917619">

Executes script compilation.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.73537353735374%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1722663441514">

Internet

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row42668197206">

.. raw:: html

   <td class="cellrowborder" valign="top" width="25.562556255625562%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p426711912014">

bash

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.7020702070207%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p14267131962014">

Executes commands.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.73537353735374%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p14267101962014">

Internet

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1463517494402">

.. raw:: html

   <td class="cellrowborder" valign="top" width="25.562556255625562%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p258814561424">

build-essential

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.7020702070207%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1749611716181">

Provides basic software package for compilation.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.73537353735374%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p8635174916403">

Internet

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1711946154018">

.. raw:: html

   <td class="cellrowborder" valign="top" width="25.562556255625562%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p15588165684216">

gn

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.7020702070207%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p4588135634213">

Generates ninja compilation scripts.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.73537353735374%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p10572194318318">

https://repo.huaweicloud.com/harmonyos/compiler/gn/1523/linux/gn.1523.tar

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row16990164213404">

.. raw:: html

   <td class="cellrowborder" valign="top" width="25.562556255625562%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1858825613428">

ninja

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.7020702070207%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p15844174611816">

Executes ninja compilation scripts.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.73537353735374%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1923373393515">

https://repo.huaweicloud.com/harmonyos/compiler/ninja/1.9.0/linux/ninja.1.9.0.tar

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

Development Tools for Windows
-----------------------------

**Table 3** Development tools and obtaining methods

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row3133133312711">

.. raw:: html

   <th class="cellrowborder" valign="top" width="16.371637163716375%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p16132203372716">

Development Tool

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50.29502950295029%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p1413219339278">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p17133183312711">

How to Obtain

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

   <tr id="row138432533451">

.. raw:: html

   <td class="cellrowborder" valign="top" width="16.371637163716375%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p163612016916">

Visual Studio Code

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.29502950295029%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1563690791">

Edits code.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p146361701097">

https://code.visualstudio.com/

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row12133123315277">

.. raw:: html

   <td class="cellrowborder" valign="top" width="16.371637163716375%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p613393317271">

HUAWEI DevEco Device Tool

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.29502950295029%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p10133193310276">

Supports code editing, compilation, burning, and debugging.

.. raw:: html

   </p>

.. note::
   :name: note7133193392718

   NOTE:

   .. container:: notebody

      .. raw:: html

         <p id="p1133183310277">

      HUAWEI DevEco Device Tool is a one-stop integrated development
      environment (IDE) provided for developers of OpenHarmony-based
      smart devices. It supports C and C++ languages and is installed in
      Visual Studio Code as a plug-in.

      .. raw:: html

         </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1240954393114">

https://device.harmonyos.com/cn/ide

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row18342145821513">

.. raw:: html

   <td class="cellrowborder" valign="top" width="16.371637163716375%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p123421958131517">

IPOP, PuTTY, or other HyperTerminal

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.29502950295029%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p18342658131511">

Remotely connects to a Linux compile server or a serial port.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p17342125851518">

Internet (for example, https://www.putty.org/)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row244884215147">

.. raw:: html

   <td class="cellrowborder" valign="top" width="16.371637163716375%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1044974291416">

CH341SER.EXE

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.29502950295029%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p94491342131413">

Identifies serial port device to transmit data.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p6449184214148">

http://www.wch.cn/search?q=ch340g&t=downloads

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

Installing Basic Compilation Environment
----------------------------------------

Connecting to a Linux Server
----------------------------

Using PuTTY to log in to a Linux server from a PC running Windows

1. Open `PuTTY <https://www.putty.org/>`__, enter the IP address of the
   Linux server, and click **Open**.

   | **Figure 2** PuTTY configuration
   | |image2|

2. Click **Yes** in the PuTTY **Security Alert** dialog box.

3. Enter the account and password.

   | **Figure 3** Login
   | |image3|

4. The login is successful.

   | **Figure 4** Successful login
   | |image4|

Changing Linux Shell to Bash
----------------------------

Run the following command to check whether bash is used as the shell:

::

   ls -l /bin/sh

If **/bin/sh -> bash** is not displayed, do as follows to change shell
to bash.

**Method 1:** Run the following command on the device and then click
**No**.

::

   sudo dpkg-reconfigure dash

**Method 2:** Run the **rm -rf /bin/sh** command to delete sh and then
run the sudo **ln -s /bin/bash /bin/sh** command to create a new soft
link.

::

   sudo rm -rf /bin/sh
   sudo ln -s /bin/bash /bin/sh

Installing a Python Environment
-------------------------------

1. Start a Linux server.

2. Run the following command to check the Python version (Python 3.7 or
   later is required):

   ::

      python3 --version

   Do as follows to install Python, for example, Python 3.8.

   1. Run the following command to check the Ubuntu version:

   ::

      cat /etc/issue

   1. Install Python based on the Ubuntu version.

      -  If the Ubuntu version is 18 or later, run the following
         command:

         ::

            sudo apt-get install python3.8

      -  If the Ubuntu version is 16, download the installation package
         and install Python.

         1. Run the following command to install Python environment
            dependencies (gcc, g++, make, zlib, libffi):

         ::

            sudo apt-get install gcc && sudo apt-get install g++ && sudo apt-get install make && sudo apt-get install zlib* && sudo apt-get install libffi-dev

         1. Obtain the `Python3.8.5 installation
            package <https://www.python.org/ftp/python/3.8.5/Python-3.8.5.tgz>`__,
            save it to the Linux server, and run the following command:

         ::

            tar -xvzf Python-3.8.5.tgz && cd Python-3.8.5 && sudo ./configure && sudo make && sudo make install

3. After Python is installed, run the following command to link the
   Python path to **/usr/bin/python**:

   ::

      which python3.8
      cd /usr/bin && sudo rm python && sudo ln -s /usr/local/bin/python3.8 python && python --version

4. Install and upgrade the Python package management tool (pip3) using
   either of the following methods:

   -  **Command line:**

      ::

         sudo apt-get install python3-setuptools python3-pip -y
         sudo pip3 install --upgrade pip

   -  **Installation package:**

      ::

         curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
         python get-pip.py

5. Run the following command to install setuptools:

   ::

      pip3 install setuptools

6. Install the GUI menuconfig tool (Kconfiglib). You are advised to
   install Kconfiglib 13.2.0 or later.

   -  **Command line:**

      ::

         sudo pip3 install kconfiglib

   -  **Installation package:**

      1. Download the .whl file (for example,
         **kconfiglib-13.2.0-py2.py3-none-any.whl**).

         Download path: https://pypi.org/project/kconfiglib#files

      2. Run the following command to install the .whl file:

         ::

            sudo pip3 install kconfiglib-13.2.0-py2.py3-none-any.whl

7. Install **pycryptodome** using either of the following methods:

   Install the Python component packages on which the file signature
   depends, including pycryptodome, six, and ecdsa. As the installation
   of **ecdsa** depends on that of **six**, install **six** first.

   -  **Command line:**

      ::

         sudo pip3 install pycryptodome

   -  **Installation package:**

      1. Download the .whl file, for example,
         **pycryptodome-3.7.3-cp37-cp37m-manylinux1_x86_64.whl** from
         https://pypi.org/project/pycryptodome/#files.

      2. Run the following command to install the .whl file:

         ::

            sudo pip3 install pycryptodome-3.7.3-cp37-cp37m-manylinux1_x86_64.whl

8. Install **six** using either of the following methods:

   -  **Command line:**

      ::

         sudo pip3 install six --upgrade --ignore-installed six

   -  **Installation package:**

      1. Download the .whl file, for example,
         **six-1.12.0-py2.py3-none-any.whl** from
         https://pypi.org/project/six/#files.

      2. Run the following command to install the .whl file:

         ::

            sudo pip3 install six-1.12.0-py2.py3-none-any.whl

9. Install **ecdsa** using either of the following methods:

   -  **Command line:**

      ::

         sudo pip3 install ecdsa

   -  **Installation package:**

      1. Download the .whl file, for example,
         **ecdsa-0.14.1-py2.py3-none-any.whl** from
         https://pypi.org/project/ecdsa/#files.

      2. Run the following command to install the .whl file:

         ::

            sudo pip3 install ecdsa-0.14.1-py2.py3-none-any.whl

Installing Scons
----------------

1. Start a Linux server.

2. Run the following command to install the SCons installation package:

   ::

      sudo apt-get install scons -y

   If the installation package cannot be found in the software source,
   do as follows:

   1. Download the source code package from
      https://scons.org/pages/download.html. The recommended SCons
      version is 3.0.4 or later.

   2. Decompress the source code package to any directory.

   3. Go to the source code directory and run the following command to
      install the source code package:

      ::

         sudo python3 setup.py install

3. Run the following command to check whether the installation is
   successful.

   ::

      scons -v

   | **Figure 5** Successful installation
   | |image5|

Installing Compilation Tools
----------------------------

   |image6| **NOTICE:** - If you acquire the source code using an HPM
   component or HPM CLI tool, compilation tools like **gn**, **ninja**,
   **gcc_riscv32** are not required. - (Recommended) If you obtain the
   source code via the mirror site or code repository, install
   compilation tools such as **gn**, **ninja**, and **gcc_riscv32**.
   Ensure that only **gn**, **ninja**, and **gcc_riscv32** are used for
   the compilation environment of Hi3861 WLAN module.

Installing gn
-------------

1. Start a Linux server.

2. Download
   `gn <https://repo.huaweicloud.com/harmonyos/compiler/gn/1523/linux/gn.1523.tar>`__.

3. Run the following command to decompress the gn installation package
   to **~/gn**.

   ::

      tar -xvf gn.1523.tar -C ~/

4. Set an environment variable by performing the following steps. Open
   the **~/.bashrc** file in Vim first.

   ::

      vim ~/.bashrc

   Copy the following command to the last line of the **.bashrc** file,
   save the file, and exit.

   ::

      export PATH=~/gn:$PATH

5. Run the following command to validate the environment variable.

   ::

      source ~/.bashrc

Installing ninjah
-----------------

1. Start a Linux server.

2. Download
   `ninja <https://repo.huaweicloud.com/harmonyos/compiler/ninja/1.9.0/linux/ninja.1.9.0.tar>`__.

3. Run the following command to decompress the ninja installation
   package to **~/ninja**.

   ::

      tar -xvf ninja.1.9.0.tar -C ~/

4. Set an environment variable by performing the following steps. Open
   the **~/.bashrc** file in Vim first.

   ::

      vim ~/.bashrc

   Copy the following command to the last line of the **.bashrc** file,
   save the file, and exit.

   ::

      export PATH=~/ninja:$PATH

5. Run the following command to validate the environment variable.

   ::

      source ~/.bashrc

Installing gcc_riscv32 (Compilation Toolchain for WLAN Module)
--------------------------------------------------------------

   |image7| **NOTICE:** The Hi3861 platform supports only the static
   link of the libgcc library. **The dynamic link is not recommended
   because version 3 of the GNU General Public License (GPLv3) will be
   polluted during commercial distribution.**

1. Start a Linux server.

2. Download
   `gcc_riscv32 <https://repo.huaweicloud.com/harmonyos/compiler/gcc_riscv32/7.3.0/linux/gcc_riscv32-linux-7.3.0.tar.gz>`__.

3. Run the following command to decompress the gcc_riscv32 installation
   package to **~/gcc_riscv32**.

   ::

      tar -xvf gcc_riscv32-linux-7.3.0.tar.gz -C ~/

4. Set an environment variable by performing the following steps. Open
   the **~/.bashrc** file in Vim first.

   ::

      vim ~/.bashrc

   Copy the following command to the last line of the **.bashrc** file,
   save the file, and exit.

   ::

      export PATH=~/gcc_riscv32/bin:$PATH

5. Run the following command to validate the environment variable.

   ::

      source ~/.bashrc

6. Enter the following command to check whether the compiler is
   successfully installed. If the compiler version number is correctly
   displayed, the installation is successful.

   ::

      riscv32-unknown-elf-gcc -v

.. |image1| image:: figures/hardware-connections.png
.. |image2| image:: figures/putty-configuration.png
.. |image3| image:: figures/login.png
.. |image4| image:: figures/successful-login.png
.. |image5| image:: figures/successful-installation.png
.. |image6| image:: public_sys-resources/icon-notice.gif
.. |image7| image:: public_sys-resources/icon-notice.gif
