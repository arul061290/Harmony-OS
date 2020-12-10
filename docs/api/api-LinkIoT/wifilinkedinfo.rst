WifiLinkedInfo
==============

**Overview**\ 
--------------

**Related Modules:**

`Wifiservice <wifiservice.rst>`__

**Description:**

Represents the Wi-Fi connection information.

This refers to the information about the hotspot connected to this
station. The information is obtained using
`GetLinkedInfo <wifiservice.rst#gaa8f07a31b01761da44f0fe90d461c168>`__.

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

   <tr id="row1776022147191903">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1082144124191903">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1352008501191903">

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

   <tr id="row1794995029191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2091125967191903">

ssid [WIFI_MAX_SSID_LEN]

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1870972992191903">

char

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2088356068191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2089675624191903">

bssid [WIFI_MAC_LEN]

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1765801702191903">

unsigned char

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row191883499191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p515543670191903">

rssi

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1158292429191903">

int

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1439919605191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p121049426191903">

connState

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1737321150191903">

WifiConnState

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row348556927191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p315077612191903">

disconnectedReason

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1760285191903">

unsigned short

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

bssid
-----

::

   unsigned char WifiLinkedInfo::bssid[[WIFI_MAC_LEN](wifiservice.rst#gabc871a0934ad71ec71b29de3f9bc4815)]

**Description:**

Basic service set ID (BSSID). For its length, see
`WIFI_MAC_LEN <wifiservice.rst#gabc871a0934ad71ec71b29de3f9bc4815>`__.

connState
---------

::

   [WifiConnState](wifiservice.rst#ga970b7d5373775b1c7f3b31074bae50e1) WifiLinkedInfo::connState

**Description:**

Wi-Fi connection state, which is defined in
`WifiConnState <wifiservice.rst#ga970b7d5373775b1c7f3b31074bae50e1>`__

disconnectedReason
------------------

::

   unsigned short WifiLinkedInfo::disconnectedReason

**Description:**

Reason for Wi-Fi disconnection

rssi
----

::

   int WifiLinkedInfo::rssi

**Description:**

Received signal strength indicator (RSSI)

ssid
----

::

   char WifiLinkedInfo::ssid[[WIFI_MAX_SSID_LEN](wifiservice.rst#ga7e01d8c5079081de486637b4482c937a)]

**Description:**

`Service <service.rst>`__ set ID (SSID). For its length, see
`WIFI_MAX_SSID_LEN <wifiservice.rst#ga7e01d8c5079081de486637b4482c937a>`__.
