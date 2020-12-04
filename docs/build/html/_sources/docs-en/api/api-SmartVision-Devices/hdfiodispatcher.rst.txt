HdfIoDispatcher
===============

**Overview**\ 
--------------

**Related Modules:**

`Core <core.md>`__

**Description:**

Defines a driver service call dispatcher.

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

   <tr id="row544230642093530">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1850233226093530">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1192978743093530">

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

   <tr id="row1738720333093530">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p223041841093530">

Dispatch )(struct HdfObject *service, int cmdId, struct HdfSBuf*\ data,
struct HdfSBuf \*reply)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1827517979093530">

int(\*

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

Dispatch
--------

::

   int(* HdfIoDispatcher::Dispatch) (struct [HdfObject](hdfobject.md) *service, int cmdId, struct [HdfSBuf](hdfsbuf.md) *data, struct [HdfSBuf](hdfsbuf.md) *reply)

**Description:**

Dispatches a driver service call. **service** indicates the pointer to
the driver service object, **id** indicates the command word of the
function, **data** indicates the pointer to the data you want to pass to
the driver, and **reply** indicates the pointer to the data returned by
the driver.
