touch
=====

Command Function
----------------

-  This command is used to create an empty file in a specified
   directory.
-  If this command is executed to create an existing file, the execution
   will be successful but the timestamp will not be updated.

Syntax
------

touch [*filename*]

Parameter Description
---------------------

**Table 1** Parameters

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1642mcpsimp">

.. raw:: html

   <th class="cellrowborder" valign="top" width="20.73%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p1653mcpsimp">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="52.44%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p1655mcpsimp">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="26.83%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p1657mcpsimp">

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

   <tr id="row1684mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.73%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1686mcpsimp">

filename

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52.44%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1688mcpsimp">

Indicates the name of the file to be created.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="26.83%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1690mcpsimp">

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

-  The **touch** command creates a read-write empty file.

-  The **touch** command creates only one file at a time.

      |image1| **NOTICE:** If you run the **touch** command to create a
      file in a path storing important system resources, unexpected
      results such as a system breakdown may occur. For example, if you
      run the **touch uartdev-0** command in the **/dev** path, the
      system may stop responding.

Example
-------

Enter **touch file.c**.

Output
------

| **Figure 1** Creating **file.c**\ 
| |image2|

.. |image1| image:: public_sys-resources/icon-notice.gif
.. |image2| image:: figures/creating-file-c.png
