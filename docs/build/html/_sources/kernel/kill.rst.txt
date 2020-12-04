kill
====

Command Function
----------------

This command is used to send a specific signal to a specified process.

Syntax
------

kill [*signo* \| *-signo*] [*pid*]

Parameter Description
---------------------

**Table 1** Parameters

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row444mcpsimp">

.. raw:: html

   <th class="cellrowborder" valign="top" width="21%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p446mcpsimp">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="51.92%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p448mcpsimp">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="27.08%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p450mcpsimp">

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

   <tr id="row451mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2500105121818">

signo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="51.92%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1149945111817">

Indicates the signal ID.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27.08%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p749810571812">

[1, 30]

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row113001232165611">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p18301173213562">

pid

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="51.92%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1730143212569">

Indicates the process ID.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="27.08%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1301193275618">

[1, MAX_INT]

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

..

   |image1| **NOTICE:** The valid range of the **signo** value is [0,
   64], and the recommended value range is [1, 30]. Other values in the
   valid range are reserved.

Usage
-----

The **signo** and **pid** parameters are mandatory.

The **pid** value range varies depending on the system configuration.
For example, if the maximum **pid** value supported by the system is
**256**, this value range is [1-256].

Example
-------

1. Query the current process list and determine the PID (7) of the
   process to be killed.

| **Figure 1** Querying PIDs
| |image2|

2. Run **kill 14 7** to send signal 14 (the default behavior of
   **SIGALRM** is to terminate the process) to process 7
   **helloworld_d** (user-space). Then query the current process list.
   Process 7 has been terminated. The result of the **kill 14 7**
   command is the same as that of the **kill -14 7** command.

| **Figure 2** Command output
| |image3|

Output
------

The command output is as follows:

| **Figure 3** Sending a signal to a specified process
| |image4|

The signal is successfully sent if no error is reported.

| **Figure 4** Signal sending failure
| |image5|

The preceding figure shows a signal sending failure caused by invalid
parameters. In this case, check that the signal ID and PID are valid.

.. |image1| image:: public_sys-resources/icon-notice.gif
.. |image2| image:: figures/querying-pids.png
.. |image3| image:: figures/command-output.png
.. |image4| image:: figures/sending-a-signal-to-a-specified-process.png
.. |image5| image:: figures/signal-sending-failure.png
