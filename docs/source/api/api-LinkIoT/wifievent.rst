WifiEvent
=========

**Overview**\ 
--------------

**Related Modules:**

`Wifiservice <wifiservice.md>`__

**Description:**

Represents the pointer to a Wi-Fi event callback for station and hotspot
connection, disconnection, or scan.

If you do not need a callback, set the value of its pointer to **NULL**.

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

   <tr id="row2022726937191903">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p408354200191903">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p554385714191903">

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

   <tr id="row1673695053191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1615342085191903">

OnWifiConnectionChanged )(int state, WifiLinkedInfo \*info)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1870805406191903">

void(\*

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row319933265191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1584772054191903">

OnWifiScanStateChanged )(int state, int size)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1360801749191903">

void(\*

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row435678488191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1996972561191903">

OnHotspotStateChanged )(int state)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p194840352191903">

void(\*

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2070324101191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p257841525191903">

OnHotspotStaJoin )(StationInfo \*info)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p84422114191903">

void(\*

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row710680967191903">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p876359313191903">

OnHotspotStaLeave )(StationInfo \*info)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1139423777191903">

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

OnHotspotStaJoin
----------------

::

   void(* WifiEvent::OnHotspotStaJoin) ([StationInfo](stationinfo.md) *info)

**Description:**

Station connected

OnHotspotStaLeave
-----------------

::

   void(* WifiEvent::OnHotspotStaLeave) ([StationInfo](stationinfo.md) *info)

**Description:**

Station disconnected

OnHotspotStateChanged
---------------------

::

   void(* WifiEvent::OnHotspotStateChanged) (int state)

**Description:**

Hotspot state change

OnWifiConnectionChanged
-----------------------

::

   void(* WifiEvent::OnWifiConnectionChanged) (int state, [WifiLinkedInfo](wifilinkedinfo.md) *info)

**Description:**

Connection state change

OnWifiScanStateChanged
----------------------

::

   void(* WifiEvent::OnWifiScanStateChanged) (int state, int size)

**Description:**

Scan state change
