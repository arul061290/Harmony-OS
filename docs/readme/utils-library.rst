Utils Library
=============

Overview
--------

The Utils library stores basic components of OpenHarmony. These basic
components are used by OpenHarmony service subsystems and upper-layer
applications.

The Utils library provides the following capabilities on different
platforms:

-  LiteOS Cortex-M (Hi3861 platform): KV stores, file operations,
   timers, and IoT peripheral control
-  LiteOS Cortex-A (Hi3516 and Hi3518 platforms): KV stores, timers, and
   ACE JavaScript APIs

Directory Structure
-------------------

::

   utils/native/lite/                 # Root directory of the Utils library
   ├── file                        # Implementation of the file interface
   ├── hals                        # HAL directory
   │   └── file                   # Header files of the hardware abstraction layer for file operations
   ├── include                     # Files of external interfaces provided by the Utils library
   ├── js                          # ACE JavaScript API directory                 
   │   └── builtin                 
   │       ├── common
   │       ├── deviceinfokit       # Device information kit
   │       ├── filekit             # File kit
   │       └── kvstorekit          # KV store kit
   ├── kal                          # KAL directory
   │   └── timer                   # KAL implementation of the timer
   ├── kv_store                        # KV store implementation
   │   ├── innerkits               # Internal KV store interfaces
   │   └── src                     # KV store source file
   └── timer_task                   # Timer implementation

   base/iot_hardware                   # IoT peripheral control
   ├── frameworks          
   │   └── wifiiot_lite            # Implementation of the IoT peripheral control module
   ├── hals
   │   └── wifiiot_lite            # HAL interfaces
   └── interfaces
       └── kits                     # Interfaces of the IoT peripheral control module

   vendor/hisi/hi3861/hi3861_adapter/hals/iot_hardware  # HAL for IoT peripheral control
   └── wifiiot_lite                 # Implementation of the interfaces at the HAL

Constraints
-----------

The Utils library is developed using the C language.

**Table 1** Capabilities and constraints of the Utils library

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1661115214112">

.. raw:: html

   <th class="cellrowborder" valign="top" width="12.659999999999998%" id="mcps1.2.5.1.1">

.. raw:: html

   <p id="p1261115231118">

Component

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="14.78%" id="mcps1.2.5.1.2">

.. raw:: html

   <p id="p11611825118">

Platform

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="32.22%" id="mcps1.2.5.1.3">

.. raw:: html

   <p id="p1336312010465">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="40.339999999999996%" id="mcps1.2.5.1.4">

.. raw:: html

   <p id="p1833742934815">

Constraint

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

   <tr id="row10455841151112">

.. raw:: html

   <td class="cellrowborder" valign="top" width="12.659999999999998%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1945511415113">

KV store

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.78%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p668274310317">

LiteOS Cortex-M and LiteOS Cortex-A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="32.22%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p193638017460">

Provides KV storage for applications.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="40.339999999999996%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p1733717294484">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row540314384111">

.. raw:: html

   <td class="cellrowborder" valign="top" width="12.659999999999998%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p134041038141112">

File operation

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.78%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1766172113197">

LiteOS Cortex-M

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="32.22%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p113646084618">

Provides unified file operation interfaces that can be used on different
underlying chip components.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="40.339999999999996%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p83372029154819">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row175322121218">

.. raw:: html

   <td class="cellrowborder" valign="top" width="12.659999999999998%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1053219131219">

Timer

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.78%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p5406226171912">

LiteOS Cortex-M and LiteOS Cortex-A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="32.22%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p15364170194610">

Provides unified timer operation interfaces that can be used on
different underlying chip components.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="40.339999999999996%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p633742915481">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1821629675">

.. raw:: html

   <td class="cellrowborder" valign="top" width="12.659999999999998%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p198212291879">

IoT peripheral control

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.78%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p4214123191912">

LiteOS Cortex-M

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="32.22%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p4822295710">

Provides the capability of performing operations for peripherals.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="40.339999999999996%" headers="mcps1.2.5.1.4 ">

  

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

Usage
-----

-  **KV store**

   ::

      Obtaining an interface
      char key1[] = "rw.sys.version";
      char value1[32] = {0};
      int ret = UtilsGetValue(key1, value1, 32);

      Setting the interface
      char key14[] = "key_14";
      ret = UtilsSetValue(key14, defValue);

-  **File operation**

   ::

      // open && write
      char fileName[] = "testfile";
      int fd = UtilsFileOpen(fileName, O_RDWR_FS | O_CREAT_FS | O_TRUNC_FS, 0);
      printf("file handle = %d\n", fd);
      int ret = UtilsFileWrite(fd, def, strlen(def));
      printf("write ret = %d\n", ret);

      // stat
      int fileLen = 0;
      ret = UtilsFileStat(fileName, &fileLen);
      printf("file size = %d\n", fileLen);

      // seek
      int fd1 = UtilsFileOpen(fileName, O_RDWR_FS, 0);
      ret = UtilsFileSeek(fd1, 5, SEEK_SET_FS);
      printf("lseek ret = %d\n", ret);
      char buf[32] = {0};
      int readLen = UtilsFileRead(fd1, buf, 32);
      ret = UtilsFileClose(fd1);
      printf("read len = %d : buf = %s\n", readLen, buf);

      // delete
      ret = UtilsFileDelete(fileName);
      printf("delete ret = %d\n", ret);

Repositories Involved
---------------------

iothardware_frameworks_wifiiot_lite

iothardware_hals_wifiiot_lite

iothardware_interfaces_kits_wifiiot_lite

utils_native_lite
