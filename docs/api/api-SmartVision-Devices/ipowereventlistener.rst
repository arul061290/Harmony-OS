IPowerEventListener
===================

**Overview**\ 
--------------

**Related Modules:**

`Core <core.rst>`__

**Description:**

Defines the power management functions provided by the HDF for the
driver.

To use the power management mechanism provided by the HDF, implement
operations of `IPowerEventListener <ipowereventlistener.rst>`__ and
invoke {@linkHdfDeviceRegisterPowerListener} to register the operations
with the HDF.

**Since:**

1.0

**Summary**\ 
-------------

Data Fields
-----------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2128190757084836">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p992424525084836">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2144368095084836">

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

   <tr id="row1538457787084836">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1723737934084836">

Resume )(struct HdfDeviceObject \*deviceObject)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p371636822084836">

void(\*

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1309463335084836">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1016947868084836">

Suspend )(struct HdfDeviceObject \*deviceObject)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p279061906084836">

void(\*

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

**Field Documentation**\ 
-------------------------

Resume
------

::

   void(* IPowerEventListener::Resume) (struct [HdfDeviceObject](hdfdeviceobject.rst) *deviceObject)

**Description:**

Wakes up the driver device. The driver developer implements the
operation.

Suspend
-------

::

   void(* IPowerEventListener::Suspend) (struct [HdfDeviceObject](hdfdeviceobject.rst) *deviceObject)

**Description:**

Hibernates the driver device. The driver developer implements the
operation.
