arp
===

Command Function
----------------

On an Ethernet, hosts communicate with each other using MAC addresses
(non-IP addresses). Therefore, IP addresses must be converted into MAC
addresses so that hosts can communicate with each other on a LAN
(Ethernet). To resolve this issue, the host stores a table containing
the mapping between IP addresses and MAC addresses, that is, the ARP
cache table. When the host needs to send an IP packet to the destination
IP address on a LAN, the host can query the destination MAC address from
the ARP cache table. The ARP cache table is maintained by the TCP/IP
protocol stack. You can run the **arp** command to view and modify the
ARP cache table.

Syntax
------

arp

arp [*-i IF*] -s *IPADDR HWADDR*

arp [*-i IF*] -d *IPADDR*

Parameter Description
---------------------

**Table 1** Parameters

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1851mcpsimp">

.. raw:: html

   <th class="cellrowborder" valign="top" width="21%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p1853mcpsimp">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="52%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p1855mcpsimp">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="27%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p1857mcpsimp">

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

   <tr id="row1858mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1860mcpsimp">

No parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1862mcpsimp">

Prints the content of the entire ARP cache table.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1864mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1865mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1867mcpsimp">

-i IF

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1869mcpsimp">

Indicates the network interface. This parameter is optional.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1871mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1872mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1874mcpsimp">

-s IPADDR

.. raw:: html

   </p>

.. raw:: html

   <p id="p1875mcpsimp">

HWADDR

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1877mcpsimp">

Adds an ARP entry. The second parameter is the IP address and MAC
address of the other host on the LAN.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1879mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1880mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1882mcpsimp">

-d IPADDR

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1884mcpsimp">

Deletes an ARP entry.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1886mcpsimp">

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

-  The **arp** command is used to query and modify the ARP cache table
   of the TCP/IP protocol stack. If ARP entries for IP addresses on
   different subnets are added, the protocol stack returns a failure
   message.
-  This command can be used only after the TCP/IP protocol stack is
   enabled.

Example
-------

Example:

1. Enter **arp**.

   | **Figure 1** Printing the entire ARP cache table
   | |image1|

   **Table 2** Output description

   .. raw:: html

      <table>

   .. raw:: html

      <thead align="left">

   .. raw:: html

      <tr id="row1906mcpsimp">

   .. raw:: html

      <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1">

   .. raw:: html

      <p id="p1908mcpsimp">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </th>

   .. raw:: html

      <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2">

   .. raw:: html

      <p id="p1910mcpsimp">

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

      <tr id="row1911mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p1913mcpsimp">

   Address

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p1915mcpsimp">

   Indicates the IPv4 address of a network device.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row1916mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p1918mcpsimp">

   HWaddress

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p1920mcpsimp">

   Indicates the MAC address of a network device.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row1921mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p1923mcpsimp">

   Iface

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p1925mcpsimp">

   Indicates the name of the interface used by the ARP entry.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row1926mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p1928mcpsimp">

   Type

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p1930mcpsimp">

   Indicates whether the ARP entry is dynamic or static. A dynamic ARP
   entry is automatically created by the protocol stack, and a static
   ARP entry is added by the user.

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

.. |image1| image:: figures/printing-the-entire-arp-cache-table.png
