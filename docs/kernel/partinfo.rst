partinfo
========

Command Function
----------------

This command is used to query information about multiple partitions of a
hard disk or SD card identified by the system.

Syntax
------

partinfo <*dev_inodename*>

Parameter Description
---------------------

**Table 1** Parameters

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1396mcpsimp">

.. raw:: html

   <th class="cellrowborder" valign="top" width="22%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p1398mcpsimp">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="51%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p1400mcpsimp">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="27%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p1402mcpsimp">

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

   <tr id="row1403mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="22%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1405mcpsimp">

dev_inodename

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1407mcpsimp">

Indicates the name of the partition to be queried.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1409mcpsimp">

A valid partition name

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

Enter **partinfo /dev/mmcblk0p0**.

Output
------

|image1|

.. |image1| image:: figures/en-us_image_0000001052370303.png
