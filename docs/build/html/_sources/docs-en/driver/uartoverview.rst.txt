UART Overview
=============

Introduction
------------

-  The Universal Asynchronous Receiver/Transmitter (UART) is a universal
   serial data bus used for asynchronous communication. It enables
   bi-directional communication between devices in full-duplex mode.
-  UART is widely used to print information for debugging or to connect
   to various external modules such as GPS and Bluetooth.
-  A UART is connected to other modules through two wires (as shown in
   `Figure 1 <#fig209936401896>`__) or four wires (as shown in `Figure
   2 <#fig1435614171015>`__).

   1. TX: TX pin of the transmitting UART. It is connected to the RX pin
      of the peer UART.

   2. RX: RX pin of the receiving UART. It is connected to the TX pin of
      the peer UART.

   3. RTS: Request to Send signal pin. It is connected to the CTS pin of
      the peer UART and is used to indicate whether the local UART is
      ready to receive data.

   4. CTS: Clear to Send signal pin. It is connected to the RTS pin of
      the peer UART and is used to indicate whether the local UART is
      allowed to send data to the peer end.

      **Figure 1** 2-wire UART communication

      |image1|

      **Figure 2** 4-wire UART communication

      |image2|

-  The transmitting and receiving UARTs must ensure that they have the
   same settings on particular attributes such as the baud rate and data
   format (start bit, data bit, parity bit, and stop bit) before they
   start to communicate. During data transmission, a UART sends data to
   the peer end over the TX pin and receives data from the peer end over
   the RX pin. When the size of the buffer used by a UART for storing
   received data reaches the preset threshold, the RTS signal of the
   UART changes to **1** (data cannot be received), and the peer UART
   stops sending data to it because its CTS signal does not allow it to
   send data.
-  The UART interface defines a set of common functions for operating a
   UART port, including obtaining and releasing device handles, reading
   and writing data of a specified length, and obtaining and setting the
   baud rate, as well as the device attributes.

Available APIs
--------------

**Table 1** APIs for the UART driver

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1223152681611">

.. raw:: html

   <th class="cellrowborder" valign="top" width="26.619999999999997%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p210413571619">

Capability

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="31.369999999999997%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p810403511614">

Function

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="42.01%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p110418354161">

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

   <tr id="row1638573613415">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="26.619999999999997%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p917154316414">

Obtaining and releasing device handles

.. raw:: html

   </p>

.. raw:: html

   <p id="p9596111154212">

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="31.369999999999997%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p20385163614412">

UartOpen

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="42.01%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p12101135184213">

Obtains the UART device handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row5950143316415">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p149501733134113">

UartClose

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p371073520422">

Releases a specified UART device handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row34145016535">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="26.619999999999997%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p229610227124">

Reading and writing data

.. raw:: html

   </p>

.. raw:: html

   <p id="p131072201215">

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="31.369999999999997%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p8296182221219">

UartRead

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="42.01%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p16297172213125">

Reads data of a specified length from a UART device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row11585016539">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1095722493616">

UartWrite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p15297162215122">

Writes data of a specified length into a UART device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row8687115843715">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="26.619999999999997%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p196317143813">

Obtaining and setting the baud rate

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="31.369999999999997%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p166885582375">

UartGetBaud

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="42.01%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p13688358183716">

Obtains the UART baud rate.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row18987529382">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p698719214383">

UartSetBaud

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1398712123810">

Sets the UART baud rate.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1551850115317">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="26.619999999999997%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1629782201218">

Obtaining and setting device attributes

.. raw:: html

   </p>

.. raw:: html

   <p id="p10308192211216">

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="31.369999999999997%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p32972022151218">

UartGetAttribute

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="42.01%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p13297122216123">

Obtains the UART device attributes.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row7545065311">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p102974224120">

UartSetAttribute

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p152971322111219">

Sets the UART device attributes.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row14614115403">

.. raw:: html

   <td class="cellrowborder" valign="top" width="26.619999999999997%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1746281144010">

Setting the transmission mode

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="31.369999999999997%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1146215112405">

UartSetTransMode

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="42.01%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p11303181216414">

Sets the UART transmission mode.

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

   |image3| **NOTE:** All functions provided in this document can be
   called only in kernel space.

.. |image1| image:: figures/en-us_image_0000001053926237.png
.. |image2| image:: figures/en-us_image_0000001054007499.png
.. |image3| image:: public_sys-resources/icon-note.gif
