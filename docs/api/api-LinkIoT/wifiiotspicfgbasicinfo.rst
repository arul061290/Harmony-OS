WifiIotSpiCfgBasicInfo
======================

**Overview**\ 
--------------

**Related Modules:**

`Wifiiot <wifiiot.rst>`__

**Description:**

Defines data communication parameters.

**Summary**\ 
-------------

Data Fields
-----------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row117606363191905">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2133411790191905">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1081893289191905">

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

   <tr id="row498786598191905">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p972785714191905">

cpol: 1

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p771379326191905">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1241766551191905">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1955867353191905">

cpha: 1

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1846646689191905">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row403381680191905">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p652122748191905">

framMode: 2

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1261359504191905">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2005489690191905">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1341777967191905">

dataWidth: 4

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p549091007191905">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row754329516191905">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1402130474191905">

endian: 1

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1943431731191905">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row79840177191905">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1669435409191905">

pad: 23

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1650210543191905">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row219048437191905">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p185530808191905">

freq

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1824710688191905">

unsigned int

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

cpha
----

::

   unsigned int WifiIotSpiCfgBasicInfo::cpha

**Description:**

Communication phase. For details about available values, see
`WifiIotSpiCfgClockCpha <wifiiot.rst#ga1eb13cffbbdec9da1d57c766763b94e5>`__.

cpol
----

::

   unsigned int WifiIotSpiCfgBasicInfo::cpol

**Description:**

Communication polarity. For details about available values, see
`WifiIotSpiCfgClockCpol <wifiiot.rst#gad6674c8b0989b6a329d5fd5ff0d5d750>`__.

dataWidth
---------

::

   unsigned int WifiIotSpiCfgBasicInfo::dataWidth

**Description:**

Communication data width. For details about available values, see
`WifiIotSpiCfgDataWidth <wifiiot.rst#ga6f2e44db2698c33b81bd6caa438a55ea>`__.

endian
------

::

   unsigned int WifiIotSpiCfgBasicInfo::endian

**Description:**

Endian mode. For details about available values, see
`WifiIotSpiCfgEndian <wifiiot.rst#ga31924085df23a024413fa6e63e13c41e>`__.

framMode
--------

::

   unsigned int WifiIotSpiCfgBasicInfo::framMode

**Description:**

Communication protocol. For details about available values, see
`WifiIotSpiCfgFramMode <wifiiot.rst#gaef7c192e049db14e2326c0bfba181670>`__.

freq
----

::

   unsigned int WifiIotSpiCfgBasicInfo::freq

**Description:**

Communication frequency. The value ranges from 2460 Hz to 40 MHz.

pad
---

::

   unsigned int WifiIotSpiCfgBasicInfo::pad

**Description:**

Padding bit
