hdf_base.h
==========

**Overview**\ 
--------------

**Related Modules:**

`DriverUtils <driverutils.md>`__

**Description:**

Declares driver common types, including the enumerated values returned
by the function and the macro for obtaining the array size.

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

   <tr id="row2118604838093525">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1322089123093525">

Macro Name and Value

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p635166416093525">

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

   <tr id="row1393879724093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p496276738093525">

HDF_BSP_ERR_START (-100)

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

   <tr id="row827781206093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p730909232093525">

HDF_BSP_ERR_NUM(v) (HDF_BSP_ERR_START + (v))

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

   <tr id="row566130850093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1875782812093525">

HDF_DEV_ERR_START (-200)

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

   <tr id="row988444295093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p328098433093525">

HDF_DEV_ERR_NUM(v) (HDF_DEV_ERR_START + (v))

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

   <tr id="row636327610093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1037030001093525">

HDF_WAIT_FOREVER 0xFFFFFFFF

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p756235527093525">

Indicates that the function keeps waiting to obtain a semaphore or
mutex.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1557370852093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2124546032093525">

HDF_ARRAY_SIZE(a) (sizeof(a) / sizeof((a)[0]))

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1865018801093525">

Defines the array size.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1541401837093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1286312222093525">

HDF_KILO_UNIT 1000

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2105498480093525">

Defines a time conversion unit, for example, the unit for converting
from second to millisecond.

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

Enumerations
------------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1069882028093525">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1523920182093525">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1621099188093525">

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

   <tr id="row1073408598093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p894603558093525">

HDF_STATUS { HDF_SUCCESS = 0, HDF_FAILURE = -1, HDF_ERR_NOT_SUPPORT =
-2, HDF_ERR_INVALID_PARAM = -3, HDF_ERR_INVALID_OBJECT = -4,
HDF_ERR_MALLOC_FAIL = -6, HDF_ERR_TIMEOUT = -7,
HDF_ERR_THREAD_CREATE_FAIL = -10, HDF_ERR_QUEUE_FULL = -15,
HDF_ERR_DEVICE_BUSY = -16, HDF_ERR_IO = -17, HDF_ERR_BAD_FD = -18,
HDF_BSP_ERR_OP = HDF_BSP_ERR_NUM(-1), HDF_ERR_BSP_PLT_API_ERR =
HDF_BSP_ERR_NUM(-2), HDF_PAL_ERR_DEV_CREATE = HDF_BSP_ERR_NUM(-3),
HDF_PAL_ERR_INNER = HDF_BSP_ERR_NUM(-4), HDF_DEV_ERR_NO_MEMORY =
HDF_DEV_ERR_NUM(-1), HDF_DEV_ERR_NO_DEVICE = HDF_DEV_ERR_NUM(-2),
HDF_DEV_ERR_NO_DEVICE_SERVICE = HDF_DEV_ERR_NUM(-3),
HDF_DEV_ERR_DEV_INIT_FAIL = HDF_DEV_ERR_NUM(-4),
HDF_DEV_ERR_PUBLISH_FAIL = HDF_DEV_ERR_NUM(-5),
HDF_DEV_ERR_ATTACHDEV_FAIL = HDF_DEV_ERR_NUM(-6), HDF_DEV_ERR_NODATA =
HDF_DEV_ERR_NUM(-7), HDF_DEV_ERR_NORANGE = HDF_DEV_ERR_NUM(-8),
HDF_DEV_ERR_OP = HDF_DEV_ERR_NUM(-10) }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1950238103093525">

Enumerates HDF return value types.

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

**Details**\ 
-------------

**Macro Definition Documentation**\ 
------------------------------------

HDF_BSP_ERR_NUM
---------------

::

   #define HDF_BSP_ERR_NUM( v)   ([HDF_BSP_ERR_START](hdf_base-h.md#aa6370acad4a8ca2031370c833f2ff51f) + (v))

**Description:**

Defines the BSP module error codes.

HDF_BSP_ERR_START
-----------------

::

   #define HDF_BSP_ERR_START   (-100)

**Description:**

Defines the start of the Board Support Package (BSP) module error codes.

HDF_DEV_ERR_NUM
---------------

::

   #define HDF_DEV_ERR_NUM( v)   ([HDF_DEV_ERR_START](hdf_base-h.md#afdce96b5c938acadb74cdcb09d53cfaf) + (v))

**Description:**

Defines the device module error codes.

HDF_DEV_ERR_START
-----------------

::

   #define HDF_DEV_ERR_START   (-200)

**Description:**

Defines the start of the device module error codes.
