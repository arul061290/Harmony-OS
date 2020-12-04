watch
=====

Command Function
----------------

This command is used to periodically monitor the execution result of a
command.

Syntax
------

watch

watch [*-c/-n/-t/–count/–interval/-no-title/–over*] [*command*]

Parameter Description
---------------------

**Table 1** Parameters

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row973mcpsimp">

.. raw:: html

   <th class="cellrowborder" valign="top" width="19.801980198019802%" id="mcps1.2.5.1.1">

.. raw:: html

   <p id="p975mcpsimp">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="27.722772277227726%" id="mcps1.2.5.1.2">

.. raw:: html

   <p id="p977mcpsimp">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="23.762376237623766%" id="mcps1.2.5.1.3">

.. raw:: html

   <p id="p979mcpsimp">

Default Value

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="28.712871287128717%" id="mcps1.2.5.1.4">

.. raw:: html

   <p id="p981mcpsimp">

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

   <tr id="row982mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p984mcpsimp">

-c / –count

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p986mcpsimp">

Indicates the number of times that the command is executed.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="23.762376237623766%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p988mcpsimp">

0xFFFFFF

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.712871287128717%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p990mcpsimp">

(0, 0xFFFFFF]

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row991mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p993mcpsimp">

-n / –interval

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p995mcpsimp">

Indicates the interval for periodically running the command, in seconds.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="23.762376237623766%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p997mcpsimp">

1s

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.712871287128717%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p999mcpsimp">

(0, 0xFFFFFF]

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1000mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1002mcpsimp">

-t / -no-title

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1004mcpsimp">

Disables time display on the top.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="23.762376237623766%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p1006mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.712871287128717%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p1008mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1009mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1011mcpsimp">

command

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1013mcpsimp">

Indicates the command to be monitored.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="23.762376237623766%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p1015mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.712871287128717%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p1017mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1018mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1020mcpsimp">

–over

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1022mcpsimp">

Stops the current command monitoring.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="23.762376237623766%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p1024mcpsimp">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.712871287128717%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p1026mcpsimp">

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

You can run the **watch –over** command to stop the currently running
command monitoring.

Example
-------

Enter **watch -n 2 -c 6 task**.

Output
------

| **Figure 1** **task** command monitoring result
| |image1|

   |image2| **NOTE:** In this example, the **task** command has been
   executed every 2 seconds for six times, and the preceding figure
   shows the output of the last execution.

.. |image1| image:: figures/task-command-monitoring-result.png
.. |image2| image:: public_sys-resources/icon-note.gif
