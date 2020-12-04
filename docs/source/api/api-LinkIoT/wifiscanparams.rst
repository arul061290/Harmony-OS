WifiScanParams
==============

**Overview**\ 
--------------

**Related Modules:**

`Wifiservice <wifiservice.md>`__

**Description:**

Represents the Wi-Fi station configuration used to connect to a
specified Wi-Fi device.

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

   <tr id="row964003011191903">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p155400450191903">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1316231575191903">

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

   <tr id="row2102632087191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p811222075191903">

ssid [WIFI_MAX_SSID_LEN]

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p293427828191903">

char

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1585496189191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p512192033191903">

ssidLen

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p579307464191903">

char

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row665333700191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p516363752191903">

bssid [WIFI_MAC_LEN]

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1027370715191903">

char

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1275523228191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2139807557191903">

freqs

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1973844077191903">

int

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1116434499191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p659994741191903">

band

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1344509006191903">

int

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1244931885191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1685340360191903">

scanType

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p22686715191903">

WifiScanType

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

band
----

::

   int WifiScanParams::band

**Description:**

Frequency band.

bssid
-----

::

   char WifiScanParams::bssid[[WIFI_MAC_LEN](wifiservice.md#gabc871a0934ad71ec71b29de3f9bc4815)]

**Description:**

Basic service set ID (BSSID). Its length is defined by
`WIFI_MAC_LEN <wifiservice.md#gabc871a0934ad71ec71b29de3f9bc4815>`__.

freqs
-----

::

   int WifiScanParams::freqs

**Description:**

Frequency.

scanType
--------

::

   [WifiScanType](wifiservice.md#ga007bf5e22727debc02cad860e41a60a3) WifiScanParams::scanType

**Description:**

Wi-Fi scan type, which is defined by
`WifiScanType <wifiservice.md#ga007bf5e22727debc02cad860e41a60a3>`__.

ssid
----

::

   char WifiScanParams::ssid[[WIFI_MAX_SSID_LEN](wifiservice.md#ga7e01d8c5079081de486637b4482c937a)]

**Description:**

`Service <service.md>`__ set ID (SSID). Its maximum length is defined by
`WIFI_MAX_SSID_LEN <wifiservice.md#ga7e01d8c5079081de486637b4482c937a>`__.

ssidLen
-------

::

   char WifiScanParams::ssidLen

**Description:**

Length of the SSID.
