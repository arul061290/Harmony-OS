WifiDeviceConfig
================

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

   <tr id="row1002206906191903">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p380703197191903">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1598813006191903">

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

   <tr id="row350617302191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p70915236191903">

ssid [WIFI_MAX_SSID_LEN]

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1828550615191903">

char

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1960674038191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1898658796191903">

bssid [WIFI_MAC_LEN]

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p428876637191903">

unsigned char

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2082652590191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p492952589191903">

preSharedKey [WIFI_MAX_KEY_LEN]

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1182861002191903">

char

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row547775743191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p409339088191903">

securityType

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1331417719191903">

int

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1291587731191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p582973978191903">

netId

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2124659733191903">

int

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1978830716191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p438399985191903">

freq

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p689365236191903">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row264341955191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1679131359191903">

wapiPskType

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2073684517191903">

int

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

   unsigned char WifiDeviceConfig::bssid[[WIFI_MAC_LEN](wifiservice.md#gabc871a0934ad71ec71b29de3f9bc4815)]

**Description:**

Basic service set ID (BSSID). For its length, see
`WIFI_MAC_LEN <wifiservice.md#gabc871a0934ad71ec71b29de3f9bc4815>`__.

freq
----

::

   unsigned int WifiDeviceConfig::freq

**Description:**

Frequency

netId
-----

::

   int WifiDeviceConfig::netId

**Description:**

Allocated **networkId**

preSharedKey
------------

::

   char WifiDeviceConfig::preSharedKey[[WIFI_MAX_KEY_LEN](wifiservice.md#ga6017e2d011b6cffcd3663db81a2b52d8)]

**Description:**

Key. For its length, see
`WIFI_MAX_KEY_LEN <wifiservice.md#ga6017e2d011b6cffcd3663db81a2b52d8>`__.

securityType
------------

::

   int WifiDeviceConfig::securityType

**Description:**

Security type. It is defined in
`WifiSecurityType <wifiservice.md#ga97c133f7db7c1234babcde03c4ce1b05>`__.

ssid
----

::

   char WifiDeviceConfig::ssid[[WIFI_MAX_SSID_LEN](wifiservice.md#ga7e01d8c5079081de486637b4482c937a)]

**Description:**

`Service <service.md>`__ set ID (SSID). For its length, see
`WIFI_MAX_SSID_LEN <wifiservice.md#ga7e01d8c5079081de486637b4482c937a>`__.

wapiPskType
-----------

::

   int WifiDeviceConfig::wapiPskType

**Description:**

PSK type, see
`WifiPskType <wifiservice.md#gaa1a44d23b8478232f14d2adfc82cee77>`__.
