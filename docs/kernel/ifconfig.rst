ifconfig
========

Command Function
----------------

This command is used to query and set parameters of a NIC, such as the
IP address, subnet mask, gateway, and MAC address, and enable or disable
the NIC.

Syntax
------

ifconfig

[*-a*]

<*interface*> <*address*> [*netmask <mask>*] [*gateway <address>*]

[*hw ether <address>*] [*mtu <size>*]

[*inet6 add <address>*]

[*inet6 del <address>*]

[*up|down*]

Parameter Description
---------------------

**Table 1** Parameters

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2011mcpsimp">

.. raw:: html

   <th class="cellrowborder" valign="top" width="21%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p2013mcpsimp">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="52%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p2015mcpsimp">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="27%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p2017mcpsimp">

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

   <tr id="row2018mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2020mcpsimp">

No parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2022mcpsimp">

Displays information about all NICs, including the IP addresses, subnet
masks, gateways, MAC addresses, maximum transmission units (MTUs), and
running statuses.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2025mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2026mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2028mcpsimp">

-a

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2030mcpsimp">

Displays data sent and received by the protocol stack.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2032mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2033mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2035mcpsimp">

interface

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2037mcpsimp">

Indicates the NIC name, for example, eth0.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2039mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2040mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2042mcpsimp">

address

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2044mcpsimp">

Indicates the IP address, for example, 192.168.1.10. The NIC name must
be specified.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2046mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2047mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2049mcpsimp">

netmask

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2051mcpsimp">

Indicates the subnet mask, for example, 255.255.255.0.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2054mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2055mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2057mcpsimp">

gateway

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2059mcpsimp">

Indicates the gateway, for example, 192.168.1.1.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2062mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2063mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2065mcpsimp">

hw ether

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2067mcpsimp">

Indicates the MAC address, for example, 00:11:22:33:44:55. Currently,
only the ether hardware type is supported.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2071mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2072mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2074mcpsimp">

mtu

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2076mcpsimp">

Indicates the MTU size, for example, 1000.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <ul id="ul10290630142713">

.. raw:: html

   <li>

For IPv4:

.. raw:: html

   <p id="p7324133522720">

[68,1500]

.. raw:: html

   </p>

.. raw:: html

   </li>

.. raw:: html

   <li>

For IPv6:

.. raw:: html

   <p id="p15794114813278">

[1280, 1500]

.. raw:: html

   </p>

.. raw:: html

   </li>

.. raw:: html

   </ul>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2079mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2081mcpsimp">

add

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2083mcpsimp">

Indicates the IPv6 address, for example, 2001:a:b:c:d:e:f:d. The NIC
name and inet6 must be specified.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2085mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2086mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2088mcpsimp">

del

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2090mcpsimp">

Deletes an IPv6 address. The NIC name and inet6 must be specified.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2092mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2100mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2102mcpsimp">

up

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2104mcpsimp">

Enables the data processing function of the NIC. The NIC name must be
specified.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2106mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2107mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2109mcpsimp">

down

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2111mcpsimp">

Disables the data processing function of the NIC. The NIC name must be
specified.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2113mcpsimp">

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

-  This command can be used only after the TCP/IP protocol stack is
   enabled.
-  Detecting the IP address conflict takes a period of time. Each time
   you run the **ifconfig** command to set an IP address, there is a
   delay of about 2 seconds.

Example
-------

1. ifconfig eth0 192.168.100.31 netmask 255.255.255.0 gateway
   192.168.100.1 hw ether 00:49:cb:6c:a1:31
2. ifconfig -a
3. ifconfig eth0 inet6 add 2001:a:b:c:d:e:f:d
4. ifconfig eth0 inet6 del 2001:a:b:c:d:e:f:d

Output
------

1. Setting network parameters:

   ::

      OHOS # ifconfig eth0 192.168.100.31 netmask 255.255.255.0 gateway 192.168.100.1 hw ether 00:49:cb:6c:a1:31
      OHOS # ifconfig
      eth0     ip:192.168.100.31 netmask:255.255.255.0 gateway:192.168.100.1
      HWaddr 00:49:cb:6c:a1:31 MTU:1500 Running Default Link UP
      lo         ip:127.0.0.1 netmask:255.0.0.0 gateway:127.0.0.1
      ip6: ::1/64
      HWaddr 00 MTU:0 Running Link UP

   The following table describes the output parameters.

   **Table 2** Output description

   .. raw:: html

      <table>

   .. raw:: html

      <thead align="left">

   .. raw:: html

      <tr id="row2152mcpsimp">

   .. raw:: html

      <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1">

   .. raw:: html

      <p id="p2154mcpsimp">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </th>

   .. raw:: html

      <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2">

   .. raw:: html

      <p id="p2156mcpsimp">

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

      <tr id="row2157mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2159mcpsimp">

   ip

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p2161mcpsimp">

   Indicates the IP address of the board.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row2162mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2164mcpsimp">

   netmask

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p2166mcpsimp">

   Indicates the subnet mask.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row2167mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2169mcpsimp">

   gateway

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p2171mcpsimp">

   Indicates the gateway.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row2177mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2179mcpsimp">

   HWaddr

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p2181mcpsimp">

   Indicates the MAC address of the board.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row2182mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2184mcpsimp">

   MTU

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p2186mcpsimp">

   Indicates the MTU.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row2187mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2189mcpsimp">

   Running/Stop

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p2191mcpsimp">

   Indicates whether the NIC is running.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row2192mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2194mcpsimp">

   Default

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p2196mcpsimp">

   Indicates that the NIC is connected to the default gateway.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row2197mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2199mcpsimp">

   Link UP/Down

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p2201mcpsimp">

   Indicates the connection status of the NIC.

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

2. Obtaining protocol stack statistics:

   ::

      OHOS # ifconfig -a
      RX packets:6922  errors:0        ip dropped:4312         link dropped:67         overrun:0       bytes:0 (0.0 B)
      RX packets(ip6):3     errors:0        dropped:0       overrun:0       bytes:0 (0.0 B)
      TX packets:1394  errors:0        link dropped:67         overrun:0       bytes:0(0.0 B)
      TX packets(ip6):3     errors:0        overrun:0       bytes:0(0.0 B)

   The following table describes the output parameters.

   **Table 3** ifconfig -a output description

   .. raw:: html

      <table>

   .. raw:: html

      <thead align="left">

   .. raw:: html

      <tr id="row2214mcpsimp">

   .. raw:: html

      <th class="cellrowborder" valign="top" width="28.999999999999996%" id="mcps1.2.3.1.1">

   .. raw:: html

      <p id="p2216mcpsimp">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </th>

   .. raw:: html

      <th class="cellrowborder" valign="top" width="71%" id="mcps1.2.3.1.2">

   .. raw:: html

      <p id="p2218mcpsimp">

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

      <tr id="row2219mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2221mcpsimp">

   RX packets

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p2223mcpsimp">

   Indicates the number of normal packets that have been received at the
   IP layer.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row2224mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2226mcpsimp">

   RX error

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p2228mcpsimp">

   Indicates the number of error packets that have been received at the
   IP layer. The errors include the length, verification, IP option, and
   IP header protocol errors.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row2229mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2231mcpsimp">

   RX dropped

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p2233mcpsimp">

   Indicates the number of packets that have been discarded at the IP
   layer. Packets may be discarded due to packet errors, packet
   forwarding failures, and disabled local NICs.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row2234mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2236mcpsimp">

   RX overrun

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p2238mcpsimp">

   Indicates the number of packets that the MAC layer fails to deliver
   to the upper-layer protocol stack. The failure is mainly caused by
   resource insufficiency at the protocol stack.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row2239mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2241mcpsimp">

   RX bytes

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p2243mcpsimp">

   Indicates the total length of normal packets that have been received
   at the IP layer, excluding the length of the fragments that are not
   reassembled.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row2244mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2246mcpsimp">

   TX packets

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p2248mcpsimp">

   Indicates the number of packets that have been normally sent or
   forwarded at the IP layer.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row2249mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2251mcpsimp">

   TX error

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p2253mcpsimp">

   Indicates the number of packets that the IP layer fails to send.
   Packets may fail to be sent because the packets cannot be routed or
   the packets fail to be processed in the protocol stack.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row2254mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2256mcpsimp">

   TX dropped

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p2258mcpsimp">

   Indicates the number of packets that the MAC layer discards due to
   sending failures, for example, the NIC driver fails to process the
   packets.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row2259mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2261mcpsimp">

   TX overrun

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p2263mcpsimp">

   Reserved.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row2264mcpsimp">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2266mcpsimp">

   TX bytes

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p2268mcpsimp">

   Indicates the total length of the packets that the IP layer has
   successfully sent or forwarded.

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

3. Setting the IPv6 address information:

   ::

      OHOS # ifconfig eth0 inet6 add 2001:a:b:c:d:e:f:d
      OHOS # ifconfig
      eth1    ip:192.168.3.60 netmask:255.255.255.0 gateway:0.0.0.0
      HWaddr 00:0e:c6:a8:5a:c2 MTU:1500 Running Link UP
      eth0    ip:192.168.2.60 netmask:255.255.255.0 gateway:0.0.0.0
      ip6: 2001:A:B:C:D:E:F:D/64
      HWaddr 46:44:02:02:03:03 MTU:1500 Running Link UP
      lo        ip:127.0.0.1 netmask:255.0.0.0 gateway:127.0.0.1
      ip6: ::1/64
      HWaddr 00 MTU:16436 Running Link UP

4. Deleting the IPv6 address information:

   ::

      OHOS # ifconfig eth0 inet6 del 2001:a:b:c:d:e:f:d
      OHOS # ifconfig
      eth1    ip:192.168.3.60 netmask:255.255.255.0 gateway:0.0.0.0
      HWaddr 00:0e:c6:a8:5a:c2 MTU:1500 Running Link UP
      eth0    ip:192.168.2.60 netmask:255.255.255.0 gateway:0.0.0.0
      HWaddr 46:44:02:02:03:03 MTU:1500 Running Link UP
      lo        ip:127.0.0.1 netmask:255.0.0.0 gateway:127.0.0.1
      ip6: ::1/64
      HWaddr 00 MTU:16436 Running Link UP
