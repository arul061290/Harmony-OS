strings.h
=========

**Overview**\ 
--------------

**Related Modules:**

`UTILS <utils.md>`__

**Description:**

Declares commonly used functions for byte sequence operations.

You can use the functions provided in this file to perform the
mathematical operations required during development. Example operations
include comparing, copying byte sequences, and setting a byte sequence
to 0. You must pay attention to memory management during function calls.

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

   <tr id="row1911916363084832">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p688273150084832">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1537088153084832">

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

   <tr id="row242551690084832">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1575842201084832">

bcmp (const void *s1, const void*\ s2, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1472603905084832">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p2102713996084832">

Compares byte sequences.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1320174572084832">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1576874659084832">

bcopy (const void *src, void*\ dest, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1944465668084832">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1516376167084832">

Copies byte sequences.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row980878942084832">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p541770467084832">

bzero (void \*s, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p269963347084832">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1348551160084832">

Sets byte sequences to zero.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row710577063084832">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p785575541084832">

index (const char \*s, int c)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1085695093084832">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1879986203084832">

Searches for the first position of the matched character in a string.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1031698880084832">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1627398737084832">

rindex (const char \*s, int c)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2028754578084832">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p630366338084832">

Searches for the last position of the matched character in a string.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row358127209084832">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p527746642084832">

ffs (int i)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p805049524084832">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p570223672084832">

Searches for the first bit in a word of the integer type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row506115753084832">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p364251180084832">

ffsl (long int i)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2082233150084832">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p162231411084832">

Searches for the first bit in a word of the long integer type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row838537570084832">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p771211862084832">

ffsll (long long int i)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p854233074084832">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p890822020084832">

Searches for the first bit in a word of the 8-byte long integer type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row249693188084832">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p138021983084832">

strcasecmp (const char \*_l, const char \*_r)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1401515019084832">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p588872970084832">

Compares two strings (string 1 and string 2), regardless of the letter
case.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row85985761084832">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1796172292084832">

strncasecmp (const char \*_l, const char \*_r, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p271578815084832">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p909487293084832">

Compares a specified length of two strings (string 1 and string 2),
regardless of the letter case.

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
