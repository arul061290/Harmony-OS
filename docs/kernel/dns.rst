dns
===

Command Function
----------------

This command is used to query and set the IP address of a DNS server on
a board.

Syntax
------

dns <*1-2*> <*IP*>

dns *-a*

Parameter Description
---------------------

**Table 1** Parameters

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1948mcpsimp">

.. raw:: html

   <th class="cellrowborder" valign="top" width="20.79%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p1950mcpsimp">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="52.480000000000004%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p1952mcpsimp">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="26.729999999999997%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p1954mcpsimp">

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

   <tr id="row1955mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.79%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1957mcpsimp">

<1-2>

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52.480000000000004%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1959mcpsimp">

Indicates the DNS server to set the IP address.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="26.729999999999997%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1961mcpsimp">

1 or 2

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1962mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.79%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1964mcpsimp">

<IP>

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52.480000000000004%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1966mcpsimp">

Indicates the IP address of the server.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="26.729999999999997%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="entry1967mcpsimpp0">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1968mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.79%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1970mcpsimp">

-a

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52.480000000000004%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1972mcpsimp">

Displays the current settings.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="26.729999999999997%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="entry1973mcpsimpp0">

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

None

Example
-------

Example:

1. Check the current DNS settings.
2. Set the IP address of the second DNS server.
3. Verify the setting.

Output
------

1. Checking the current DNS settings:

   ::

      OHOS # dns -a
      dns1: 208.61.222.222
      dns2: 0.0.0.0

2. Setting the IP address of the second DNS server:

   ::

      OHOS # dns 2 192.168.1.2

3. Verifying the setting:

   ::

      OHOS # dns -a
      dns1: 208.61.222.222
      dns2: 192.168.1.2
