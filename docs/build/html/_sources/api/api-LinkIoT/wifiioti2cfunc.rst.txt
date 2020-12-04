WifiIotI2cFunc
==============

**Overview**\ 
--------------

**Related Modules:**

`Wifiiot <wifiiot.md>`__

**Description:**

Defines I2C callbacks.

**Since:**

1.0

**Version:**

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

   <tr id="row859032302191904">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1617706074191904">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p405715202191904">

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

   <tr id="row2056659251191904">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p15652808191904">

resetFunc

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1578824082191904">

I2CResetFunc

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1962659888191904">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p173329721191904">

prepareFunc

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1653220426191904">

I2cPrepareFunc

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1817164142191904">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1259874849191904">

restoreFunc

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1011946177191904">

I2cRestoreFunc

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

prepareFunc
-----------

::

   [I2cPrepareFunc](wifiiot.md#ga1f0c8fe1deb1cf1fc8b19d69c2fca729) WifiIotI2cFunc::prepareFunc

**Description:**

Callback invoked for data preparation

resetFunc
---------

::

   [I2CResetFunc](wifiiot.md#ga1176c2c06eca906f3e662027df156109) WifiIotI2cFunc::resetFunc

**Description:**

Callback invoked upon an I2C device exception

restoreFunc
-----------

::

   [I2cRestoreFunc](wifiiot.md#ga16779c755404f2ec8543452268a9fb3b) WifiIotI2cFunc::restoreFunc

**Description:**

Callback invoked for data recovery
