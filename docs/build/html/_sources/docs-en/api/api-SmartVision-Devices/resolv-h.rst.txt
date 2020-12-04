resolv.h
========

**Overview**\ 
--------------

**Related Modules:**

`NET <net.md>`__

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

   <tr id="row1206933154084832">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1303850846084832">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2117307153084832">

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

   <tr id="row1327861180084832">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1934256015084832">

dn_comp (const char *src, unsigned char*\ dst, int space, unsigned char
**dnptrs, unsigned char**\ lastdnptr)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p628871895084832">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1223790885084832">

Compresses a network domain name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1285912204084832">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p249277312084832">

dn_expand (const unsigned char *base, const unsigned char*\ end, const
unsigned char *src, char*\ dest, int space)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p842897270084832">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p596949304084832">

Expands a compressed domain name to a full domain name.

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
