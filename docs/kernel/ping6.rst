ping6
=====

Command Function
----------------

This command is used to test whether the IPv6 network connection is
normal.

Syntax
------

ping6 *[-c count] [-I interface / sourceAddress] destination*

Parameter Description
---------------------

**Table 1** Parameters

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2748mcpsimp">

.. raw:: html

   <th class="cellrowborder" valign="top" width="21%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p2750mcpsimp">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="52%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p2752mcpsimp">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="27%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p2754mcpsimp">

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

   <tr id="row2755mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2757mcpsimp">

-c count

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2759mcpsimp">

Indicates the number of execution times. If this parameter is not
specified, the default value is 4.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2761mcpsimp">

1~65535

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2762mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2764mcpsimp">

-I interface

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2766mcpsimp">

Performs an IPv6 ping operation for a specified NIC.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2768mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2769mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2771mcpsimp">

-I sourceAddress

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2773mcpsimp">

Indicates the source IPv6 address to be pinged.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2775mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row84173618410">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p141163619410">

destination

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p134111362417">

Indicates the IP address of the destination host.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p134173611412">

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

-  If the destination IPv6 address is unreachable, the system displays a
   message indicating that the request times out.
-  If no route is available to the destination IPv6 address, an error
   message is displayed.
-  This command can be used only after the TCP/IP protocol stack is
   enabled.

Example
-------

-  ping6 2001:a:b:c:d:e:f:b
-  ping6 -c 3 2001:a:b:c:d:e:f:b
-  ping6 -I eth0 2001:a:b:c:d:e:f:b
-  ping6 -I 2001:a:b:c:d:e:f:d 2001:a:b:c:d:e:f:b

Output
------

1. Output of **ping6 2001:a:b:c:d:e:f:b**:

   ::

      OHOS # ping6 2001:a:b:c:d:e:f:b PING 2001:A:B:C:D:E:F:B with 56 bytes of data.
      56 bytes from 2001:A:B:C:D:E:F:B : icmp_seq=1 time<1 ms
      56 bytes from 2001:A:B:C:D:E:F:B : icmp_seq=2 time<1 ms
      56 bytes from 2001:A:B:C:D:E:F:B : icmp_seq=3 time<1 ms
      56 bytes from 2001:A:B:C:D:E:F:B : icmp_seq=4 time<1 ms
      --- 2001:a:b:c:d:e:f:b/64 ping statistics ---
      4 packets transmitted, 4 received, 0.00% packet loss, time 20ms
      rtt min/avg/max = 0/0.00/0 ms

2. Output of **ping6 -c 3 2001:a:b:c:d:e:f:b**:

   ::

      OHOS # ping6 -c 3 2001:a:b:c:d:e:f:b    PING 2001:A:B:C:D:E:F:B with 56 bytes of data.
      56 bytes from 2001:A:B:C:D:E:F:B : icmp_seq=1 time<1 ms
      56 bytes from 2001:A:B:C:D:E:F:B : icmp_seq=2 time<1 ms
      56 bytes from 2001:A:B:C:D:E:F:B : icmp_seq=3 time<1 ms
      --- 2001:a:b:c:d:e:f:b/64 ping statistics ---
      3 packets transmitted, 3 received, 0.00% packet loss, time 20ms
      rtt min/avg/max = 0/0.00/0 ms

3. Output of **ping6 -I eth0 2001:a:b:c:d:e:f:b**:

   ::

      OHOS # ping6 -I eth0 2001:a:b:c:d:e:f:b PING 2001:A:B:C:D:E:F:B with 56 bytes of data.
      56 bytes from 2001:A:B:C:D:E:F:B : icmp_seq=1 time=10 ms
      56 bytes from 2001:A:B:C:D:E:F:B : icmp_seq=2 time<1 ms
      56 bytes from 2001:A:B:C:D:E:F:B : icmp_seq=3 time<1 ms
      56 bytes from 2001:A:B:C:D:E:F:B : icmp_seq=4 time<1 ms
      --- 2001:a:b:c:d:e:f:b/64 ping statistics ---
      4 packets transmitted, 4 received, 0.00% packet loss, time 30msrtt min/avg/max = 0/2.50/10 ms

4. Output of **ping6 -I 2001:a:b:c:d:e:f:d 2001:a:b:c:d:e:f:b**:

   ::

      OHOS # ping6 -I 2001:a:b:c:d:e:f:d 2001:a:b:c:d:e:f:b PING 2001:A:B:C:D:E:F:B with 56 bytes of data.
      56 bytes from 2001:A:B:C:D:E:F:B : icmp_seq=1 time<1 ms
      56 bytes from 2001:A:B:C:D:E:F:B : icmp_seq=2 time<1 ms
      56 bytes from 2001:A:B:C:D:E:F:B : icmp_seq=3 time<1 ms
      56 bytes from 2001:A:B:C:D:E:F:B : icmp_seq=4 time<1 ms
      --- 2001:a:b:c:d:e:f:b/64 ping statistics ---
      4 packets transmitted, 4 received, 0.00% packet loss, time 20msrtt min/avg/max = 0/0.00/0 ms
