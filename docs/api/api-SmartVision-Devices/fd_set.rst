fd_set
======

**Overview**\ 
--------------

**Related Modules:**

`IO <io.rst>`__

**Description:**

Defines a file descriptor set.

This structure is used to specify whether the file descriptor set
exists.

**Summary**\ 
-------------

Data Fields
-----------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row108201520084842">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p778114934084842">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2113486390084842">

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

   <tr id="row602092891084842">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1724468896084842">

fds_bits [FD_SETSIZE/8/sizeof(long)]

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1312313278084842">

unsigned long

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

fds_bits
--------

::

   unsigned long fd_set::fds_bits[[FD_SETSIZE](io.rst#ga86c5dbf5a99358e288f573d6a1e0873f)/8/sizeof(long)]

**Description:**

Whether the descriptor exists is indicated by each bit.
