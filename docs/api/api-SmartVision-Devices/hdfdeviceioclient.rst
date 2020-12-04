HdfDeviceIoClient
=================

**Overview**\ 
--------------

**Related Modules:**

`Core <core.md>`__

**Description:**

Defines the client object structure of the I/O service.

This structure describes the invoker information of the I/O servcie.

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

   <tr id="row1906562505093530">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p667230729093530">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p110881848093530">

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

   <tr id="row1932942023093530">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p541284460093530">

device

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p921367322093530">

struct HdfDeviceObject \*

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row160462647093530">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1087352196093530">

priv

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p558418362093530">

void \*

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

device
------

::

   struct [HdfDeviceObject](hdfdeviceobject.md)* HdfDeviceIoClient::device

**Description:**

Device object corresponding to the client object

priv
----

::

   void* HdfDeviceIoClient::priv

**Description:**

Private data of the client object. The driver can use **priv** to bind
the internal data with the client.
