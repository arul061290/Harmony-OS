I2C Overview
============

Introduction
------------

-  The Inter-Integrated Circuit (I2C) is a simple, bidirectional, and
   synchronous serial bus that uses merely two wires.

-  In an I2C communication, one controller communicates with one or more
   devices through the serial data line (SDA) and serial clock line
   (SCL), as shown in `Figure 1 <#fig1135561232714>`__.

-  I2C data transfer must begin with a **START** condition and end with
   a **STOP** condition. Data is transmitted byte-by-byte from the most
   significant bit to the least significant bit.

-  Each I2C node is recognized by a unique address and can serve as
   either a controller or a device. When the controller needs to
   communicate with a device, it writes the device address to the bus
   through broadcast. A device matching this address sends a response to
   set up a data transfer channel.

-  The I2C APIs define a set of common functions for I2C data transfer,
   including:

   -  I2C controller management: opening or closing an I2C controller
   -  I2C message transfer: custom transfer by using a message array

   | **Figure 1** Physical connection diagram for I2C
   | |image1|

Available APIs
--------------

**Table 1** APIs available for the I2C driver

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row4419501537">

.. raw:: html

   <th class="cellrowborder" valign="top" width="18.63%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p641050105320">

Capability

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="28.03%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p54150165315">

Function

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="53.339999999999996%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p941150145313">

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

   <tr id="row34145016535">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="18.63%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p229610227124">

I2C controller management

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.03%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p19389143041518">

I2cOpen

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.339999999999996%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p8738101941716">

Opens an I2C controller.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row5632152611414">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p143890309153">

I2cClose

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p573815197171">

Closes an I2C controller.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row15108165391412">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.63%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p91084533141">

I2C message transfer

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.03%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p13901730101511">

I2cTransfer

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.339999999999996%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p12738111912171">

Performs a custom transfer.

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

   |image2| **NOTE:** All functions provided in this document can be
   called only in kernel mode.

.. |image1| image:: figures/physical-connection-diagram-for-i2c.png
.. |image2| image:: public_sys-resources/icon-note.gif
