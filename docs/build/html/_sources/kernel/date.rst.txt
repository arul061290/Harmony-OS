date
====

Command Function
----------------

This command is used to query and set the system date and time.

Syntax
------

date

date –help

date +[*Format*]

date -s\_ \_[*YY/MM/DD*]

date\_ *-s* \_[*hh:mm:ss*]_\_

date -r [*Filename*]

Parameter Description
---------------------

**Table 1** Parameters

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row3831mcpsimp">

.. raw:: html

   <th class="cellrowborder" valign="top" width="21%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p3833mcpsimp">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p3835mcpsimp">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="28.999999999999996%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p3837mcpsimp">

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

   <tr id="row3838mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p3840mcpsimp">

–help

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p3842mcpsimp">

Uses the help.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p3844mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row3845mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p3847mcpsimp">

+Format

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p3849mcpsimp">

Prints the date and time based on Format.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p3852mcpsimp">

Placeholders listed in –help.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row3853mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p3855mcpsimp">

-s YY/MM/DD

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p3857mcpsimp">

Sets the system date and separates the year, month, and day by slashes
(/).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p3859mcpsimp">

>= 1970/01/01

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row3860mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p3862mcpsimp">

-s hh:mm:ss

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p3864mcpsimp">

Sets the system time and separates the hour, minute, and second by
colons (:).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p3866mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row3867mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p3869mcpsimp">

-r Filename

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p3871mcpsimp">

Queries the modification time of the Filename file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p3873mcpsimp">

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

-  If the **date** parameter is not specified, the current system date
   and time are displayed by default.
-  The **–help**, **+Format**, **-s**, and **-r** parameters are
   mutually exclusive.

Example
-------

Enter **date +%Y–%m–%d**.

Output
------

| **Figure 1** System date printed based on the specified format
| |image1|

.. |image1| image:: figures/system-date-printed-based-on-the-specified-format.png
