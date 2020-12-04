ls
==

Command Function
----------------

This command is used to display the content of a specified directory.

Syntax
------

ls [*path*]

Parameter Description
---------------------

**Table 1** Parameters

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1250mcpsimp">

.. raw:: html

   <th class="cellrowborder" valign="top" width="21%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p1252mcpsimp">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="52%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p1254mcpsimp">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="27%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p1256mcpsimp">

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

   <tr id="row1257mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1259mcpsimp">

path

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1261mcpsimp">

If path is left blank, the content of the current directory is
displayed.

.. raw:: html

   </p>

.. raw:: html

   <p id="p1262mcpsimp">

If the path value is an invalid file name, the following failure message
is displayed:

.. raw:: html

   </p>

.. raw:: html

   <p id="p1263mcpsimp">

ls error: No such directory

.. raw:: html

   </p>

.. raw:: html

   <p id="p1264mcpsimp">

If the path value is a valid directory, the content of this directory is
displayed.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <ul id="ul103920301451">

.. raw:: html

   <li>

Left blank

.. raw:: html

   </li>

.. raw:: html

   <li>

A valid directory

.. raw:: html

   </li>

.. raw:: html

   </ul>

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

-  This command can be used to display the content of the current
   directory.
-  This command can also display the size of a file.
-  The **ls** command with the **proc** directory passed cannot
   calculate the file size and **0** is displayed in the command output.

Example
-------

Enter **ls**.

Output
------

| **Figure 1** Viewing content of the current directory
| |image1|

.. |image1| image:: figures/viewing-content-of-the-current-directory.png
