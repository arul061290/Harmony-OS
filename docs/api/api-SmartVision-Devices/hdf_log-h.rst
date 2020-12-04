hdf_log.h
=========

**Overview**\ 
--------------

**Related Modules:**

`DriverUtils <driverutils.md>`__

**Description:**

Declares log printing functions of the driver module. This module
provides functions for printing logs at the verbose, debug, information,
warning, and error levels.

To use these functions, you must define **HDF_LOG_TAG**, for example,
#define HDF_LOG_TAG evt.

**Since:**

1.0

**Version:**

1.0

**Summary**\ 
-------------

Macros
------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1540299786093525">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1375405289093525">

Macro Name and Value

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p831903220093525">

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

   <tr id="row2016145204093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1567601529093525">

LOG_TAG_MARK_EXTEND(HDF_TAG) #HDF_TAG

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

 

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2052661276093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1717711828093525">

HDF_LOGV(fmt, arg…) printf(“[HDF:V/" LOG_TAG "]” fmt
“:raw-latex:`\r\n`”, ##arg)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1201297239093525">

Prints logs at the verbose level.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1026030118093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1571404864093525">

HDF_LOGD(fmt, arg…) printf(“[HDF:D/" LOG_TAG "]” fmt
“:raw-latex:`\r\n`”, ##arg)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1903141057093525">

Prints logs at the debug level.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1310544128093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p656632918093525">

HDF_LOGI(fmt, arg…) printf(“[HDF:I/" LOG_TAG "]” fmt
“:raw-latex:`\r\n`”, ##arg)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2142371427093525">

Prints logs at the information level.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1863126406093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p256499208093525">

HDF_LOGW(fmt, arg…) printf(“[HDF:W/" LOG_TAG "]” fmt
“:raw-latex:`\r\n`”, ##arg)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p508076966093525">

Prints logs at the warning level.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1258814462093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1898504596093525">

HDF_LOGE(fmt, arg…) printf(“[HDF:E/" LOG_TAG "]” fmt
“:raw-latex:`\r\n`”, ##arg)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1443792214093525">

Prints logs at the error level.

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
