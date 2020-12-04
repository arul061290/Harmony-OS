tftp
====

Command Function
----------------

Trivial File Transfer Protocol (TFTP) is a protocol in the TCP/IP
protocol suite for transferring files between clients and servers. TFTP
provides simple and low-overhead file transfer services. The port number
is 69.

The **tftp** command is used to download files from the TFTP server.

Syntax
------

tftp *<-g/-p>* *-l* *[FullPathLocalFile] -r [RemoteFile] [Host]*

Parameter Description
---------------------

**Table 1** Parameters

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2900mcpsimp">

.. raw:: html

   <th class="cellrowborder" valign="top" width="20.79%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p2902mcpsimp">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="52.480000000000004%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p2904mcpsimp">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="26.729999999999997%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p2906mcpsimp">

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

   <tr id="row2907mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.79%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2909mcpsimp">

-g/-p

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52.480000000000004%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2911mcpsimp">

Indicates the file transfer direction.

.. raw:: html

   </p>

.. raw:: html

   <ul id="ul73571240131312">

.. raw:: html

   <li>

-g: downloads files from the TFTP server.

.. raw:: html

   </li>

.. raw:: html

   <li>

-p: uploads files to the TFTP server.

.. raw:: html

   </li>

.. raw:: html

   </ul>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="26.729999999999997%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p14399194271310">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2921mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.79%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2923mcpsimp">

-l FullPathLocalFile

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52.480000000000004%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2925mcpsimp">

Indicates the complete path of a local file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="26.729999999999997%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="entry2926mcpsimpp0">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2927mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.79%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2929mcpsimp">

-r RemoteFile

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52.480000000000004%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2931mcpsimp">

Indicates the file name on the server.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="26.729999999999997%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="entry2932mcpsimpp0">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2933mcpsimp">

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.79%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2935mcpsimp">

Host

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="52.480000000000004%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2937mcpsimp">

Indicates the server IP address.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="26.729999999999997%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="entry2938mcpsimpp0">

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

1. Deploy a TFTP server on the server and configure the TFTP server
   correctly.

2. Use the **tftp** command to upload and download files on the
   OpenHarmony board.

3. The size of the file to be transferred cannot exceed 32 MB.

      |image1| **NOTICE:** TFTP is under debugging and disabled by
      default. Do not use it in formal products.

Example
-------

Download the **out** file from the server.

Output
------

::

   OHOS # tftp -g -l /nfs/out -r out 192.168.1.2
   TFTP transfer finish

After the **tftp** command is executed, **TFTP transfer finish** is
displayed if the file transfer is complete. If the file transfer fails,
other information is displayed to help locate the fault.

.. |image1| image:: public_sys-resources/icon-notice.gif
