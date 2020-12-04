rm
==

Command Function
----------------

This command is used to delete a file or folder.

Syntax
------

rm [*-r*] [*dirname / filename*]

Parameter Description
---------------------

**Table 1** Parameters

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1513mcpsimp">

.. raw:: html

   <th class="cellrowborder" valign="top" width="22.220000000000002%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p1515mcpsimp">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="51.519999999999996%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p1517mcpsimp">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="26.26%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p1519mcpsimp">

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

   <tr id="row1520mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.220000000000002%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1522mcpsimp">

-r

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="51.519999999999996%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1524mcpsimp">

Deletes a directory. This parameter is optional. It is required if a
directory is to be deleted.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="26.26%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1526mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1527mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.220000000000002%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1529mcpsimp">

dirname/filename

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="51.519999999999996%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1531mcpsimp">

Indicates the name of the file or directory to be deleted. The value can
be a path.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="26.26%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1533mcpsimp">

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

-  The **rm** command deletes only one file or directory at a time.
-  The **rm -r** command can be used to delete a non-empty directory.

Example
-------

Example:

1. Enter **rm log1.txt**.
2. Enter **rm -r sd**.

Output
------

| **Figure 1** Deleting the **log1.txt** file
| |image1|

| **Figure 2** Deleting the **sd** directory
| |image2|

.. |image1| image:: figures/deleting-the-log1-txt-file.png
.. |image2| image:: figures/deleting-the-sd-directory.png
