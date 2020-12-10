Kernel Subsystem
================

Overview
--------

The OpenHarmony kernel is a real-time OS kernel developed by Huawei for
IoT devices. It is as lightweight as RTOS and as easy-to-use as Linux.

The OpenHarmony kernel includes basic kernel functions such as process
and thread scheduling, memory management, IPC mechanism, and timer
management.

The source code of the OpenHarmony kernel consists of two repositories:
the
```kernel_liteos_a`` <https://gitee.com/openharmony/kernel_liteos_a>`__
repository for Cortex-A processors and the
```kernel_liteos_m`` <https://gitee.com/openharmony/kernel_liteos_m>`__
repository for Cortex-M processors. The directory structures of the two
repositories are similar. The following describes the directory
structure of kernel_liteos_a.

Directory Structure
-------------------

**Table 1** Directory structure of the OpenHarmony kernel source code

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row7977610131417">

.. raw:: html

   <th class="cellrowborder" valign="top" width="30.34%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p18792459121314">

Directory

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="69.66%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p77921459191317">

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

   <tr id="row17977171010144">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p2793159171311">

apps

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p879375920132">

User-space init and shell application program

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row6978161091412">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p37931659101311">

arch

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p6793059171318">

System architecture, such as ARM

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row6978201031415">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p117935599130">

bsd

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p0793185971316">

Code of the driver and adaptation layer module related to the FreeBSD,
such as the USB module

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row113263612392">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p2133163611390">

compat

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1913313364399">

Compatibility with the kernel POSIX interfaces

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row15700172218399">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p10701622113920">

fs

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p270110222398">

File system module, which mainly derives from the NuttX open-source
project

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1897841071415">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p16793185961315">

kernel

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p14793959161317">

Kernel modules including the process, memory, and IPC modules

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row172848480398">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p728414485392">

lib

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p12284154818399">

Kernel library

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row5827141194012">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p48272110403">

net

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p28272119406">

Network module, which mainly derives from the lwip open-source project

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row980916239407">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p080910232403">

platform

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p11809202324018">

Code for supporting different systems on a chip (SOCs), such as
Hi3516DV300

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row194244440402">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p0424124412401">

security

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p442410448409">

Code related to security features, including process permission
management and virtual ID mapping management

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row674312515406">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1274395114012">

syscall

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1374365134011">

System calls

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row343553564120">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p54351735114113">

tools

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p17435635114116">

Building tool as well as related configuration and code

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

Constraints
-----------

Hi3518EV300 uses the JFFS2 file system by default, and Hi3516DV300 uses
the VFAT file system by default. If other file systems need to be used,
the configurations of the file systems must be added accordingly.

Usage
-----

For details, see `Kernel Usage Guidelines <../kernel/Readme-EN.rst>`__.

Repositories Involved
---------------------

`drivers_liteos <https://gitee.com/openharmony/drivers_liteos>`__

`kernel_liteos_a <https://gitee.com/openharmony/kernel_liteos_a>`__

`kernel_liteos_a_huawei_proprietary_fs_proc <https://gitee.com/openharmony/kernel_liteos_a_huawei_proprietary_fs_proc>`__

`kernel_liteos_m <https://gitee.com/openharmony/kernel_liteos_m>`__
