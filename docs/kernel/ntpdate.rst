ntpdate
=======

Command Function
----------------

This command is used to synchronize system time from the server.

Syntax
------

ntpdate [*SERVER_IP1*] [*SERVER_IP2*]…

Parameter Description
---------------------

**Table 1** Parameters

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2622mcpsimp">

.. raw:: html

   <th class="cellrowborder" valign="top" width="20.79%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p2624mcpsimp">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="52.480000000000004%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p2626mcpsimp">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="26.729999999999997%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p2628mcpsimp">

Value Range

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

   <tr id="row2629mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.79%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2631mcpsimp">

SERVER_IP

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52.480000000000004%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2633mcpsimp">

Indicates the IP address of the NTP server.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="26.729999999999997%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="entry2634mcpsimpp0">

N/A

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

Usage
-----

Run the **ntpdate**\ [*SERVER_IP1*] [*SERVER_IP2*]… command. **ntpdate**
obtains and displays the time of the first server with a valid IP
address.

Example
-------

To update the system time, run **ntpdate 192.168.1.3**.

Output
------

::

   OHOS # ntpdate 192.168.1.3
   time server 192.168.1.3: Mon Jun 13 09:24:25 2016

The time zone of the board is different from that of the server.
Therefore, the displayed time may be several hours different from the
obtained server time.
