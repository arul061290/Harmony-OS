HotspotConfig
=============

**Overview**\ 
--------------

**Related Modules:**

`Wifiservice <wifiservice.md>`__

**Description:**

Represents the hotspot configuration.

A hotspot configuration must contain the SSID (or BSSID), security type,
and key (if the security type is open).

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

   <tr id="row595248689191859">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1511519306191859">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p261841042191859">

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

   <tr id="row1872769404191859">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p177570576191859">

ssid [WIFI_MAX_SSID_LEN]

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2020436859191859">

char

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1818297573191859">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1841136542191859">

securityType

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p280427230191859">

int

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1736352202191859">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1625275169191859">

band

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p134904083191859">

int

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row249655207191859">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1308846415191859">

channelNum

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p650171445191859">

int

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1845241973191859">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1516661205191859">

preSharedKey [WIFI_MAX_KEY_LEN]

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1628209720191859">

char

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

   int HotspotConfig::band

**Description:**

Frequency band

channelNum
----------

::

   int HotspotConfig::channelNum

**Description:**

Channel number

preSharedKey
------------

::

   char HotspotConfig::preSharedKey[[WIFI_MAX_KEY_LEN](wifiservice.md#ga6017e2d011b6cffcd3663db81a2b52d8)]

**Description:**

Key. For its length, see
`WIFI_MAX_SSID_LEN <wifiservice.md#ga7e01d8c5079081de486637b4482c937a>`__.

securityType
------------

::

   int HotspotConfig::securityType

**Description:**

Security type

ssid
----

::

   char HotspotConfig::ssid[[WIFI_MAX_SSID_LEN](wifiservice.md#ga7e01d8c5079081de486637b4482c937a)]

**Description:**

`Service <service.md>`__ set ID (SSID). For its length, see
`WIFI_MAX_SSID_LEN <wifiservice.md#ga7e01d8c5079081de486637b4482c937a>`__.
