ether.h
=======

**Overview**\ 
--------------

**Related Modules:**

`NET <net.rst>`__

**Description:**

Provides functions and data structures related to network operations.
For example, you can use the functions to send and receive network data,
manage network addresses, and convert bytes.

**Since:**

1.0

**Version:**

1.0

**Summary**\ 
-------------

Functions
---------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1953245232084829">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2067996324084829">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1466511907084829">

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

   <tr id="row1709509553084829">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p711783456084829">

ether_ntoa (const struct ether_addr \*p_a)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1305652762084829">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1579897422084829">

Converts binary data in network byte order into a standard 48-bit
Ethernet host address in the colon hexadecimal notation.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row184993163084829">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1393436889084829">

ether_aton (const char \*x)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p994921515084829">

struct ether_addr \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1873866681084829">

Converts a standard 48-bit Ethernet host address in the colon
hexadecimal notation into binary data in network byte order.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row334136274084829">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p716382259084829">

ether_ntoa_r (const struct ether_addr *p_a, char*\ x)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p931209957084829">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1793424847084829">

Converts binary data in network byte order into a standard 48-bit
Ethernet host address in the colon hexadecimal notation. This function
is reentrant.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row144813171084829">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1247050141084829">

ether_aton_r (const char *x, struct ether_addr*\ p_a)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p284852490084829">

struct ether_addr \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1469125427084829">

Converts a standard 48-bit Ethernet host address in the colon
hexadecimal notation into binary data in network byte order. This
function is reentrant.

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
