cpup
====

Command Function
----------------

This command is used to query the CPU usage of the system.

Syntax
------

cpup [*mode*] [*taskID*]

Parameter Description
---------------------

**Table 1** Parameters

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row3780mcpsimp">

.. raw:: html

   <th class="cellrowborder" valign="top" width="16%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p3782mcpsimp">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="56.99999999999999%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p3784mcpsimp">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="27%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p3786mcpsimp">

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

   <tr id="row3787mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p3789mcpsimp">

mode

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="56.99999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p168830912393">

Indicates the period in which the CPU usage is to be queried. By
default, the CPU usage within the last 10 seconds is displayed.

.. raw:: html

   </p>

.. raw:: html

   <ul id="ul115118371817">

.. raw:: html

   <li>

0: displays the CPU usage of the system within the last 10 seconds.

.. raw:: html

   </li>

.. raw:: html

   <li>

1: displays the CPU usage of the system within the last 1 second.

.. raw:: html

   </li>

.. raw:: html

   <li>

Other value: displays the total CPU usage since the system is started.

.. raw:: html

   </li>

.. raw:: html

   </ul>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p3794mcpsimp">

[0, 0xFFFFFFFF]

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row3795mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p3797mcpsimp">

taskID

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="56.99999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p3799mcpsimp">

Indicates the task ID.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p3802mcpsimp">

[0, 0xFFFFFFFF]

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

-  If the parameters are not specified, the CPU usage within the last 10
   seconds is displayed.
-  If only the **mode** parameter is specified, the CPU usage within the
   specified period is displayed.
-  If both the **mode** and **taskID** parameters are specified, the CPU
   usage of the specified task within the given period is displayed.

Example
-------

Enter **cpup 1 5**.

Output
------

| **Figure 1** CPU usage
| |image1|

.. |image1| image:: figures/cpu-usage.png
