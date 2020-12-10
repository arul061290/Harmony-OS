StationInfo
===========

**Overview**\ 
--------------

**Related Modules:**

`Wifiservice <wifiservice.rst>`__

**Description:**

Represents the station information.

The station information is returned when **OnHotspotStaJoin** or
**OnHotspotStaLeave** is called.

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

   <tr id="row361059977191902">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p899118172191902">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p175351191191902">

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

   <tr id="row1254853063191902">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p430421032191902">

macAddress [WIFI_MAC_LEN]

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1935378264191902">

unsigned char

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

macAddress
----------

::

   unsigned char StationInfo::macAddress[[WIFI_MAC_LEN](wifiservice.rst#gabc871a0934ad71ec71b29de3f9bc4815)]

**Description:**

MAC address. For its length, see
`WIFI_MAC_LEN <wifiservice.rst#gabc871a0934ad71ec71b29de3f9bc4815>`__.
