GPIO Overview
=============

Introduction
------------

GPIO is short for general-purpose input/output. Generally, a GPIO
controller manages all GPIO pins by group. Each group of GPIO pins is
associated with one or more registers. The GPIO pins are operated by
reading data from and writing data to the registers.

The GPIO APIs define a set of standard functions for performing
operations on GPIO pins, including:

-  Setting the pin direction, which can be input or output (High
   impedance is not supported currently.)

-  Reading and writing level values, which can be low or high

-  Setting an interrupt service routine (ISR) function and interrupt
   trigger mode for a pin

-  Enabling or disabling a pin interrupt

Available APIs
--------------

**Table 1** APIs available for the GPIO driver

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row4419501537">

.. raw:: html

   <th class="cellrowborder" valign="top" width="19.74%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p641050105320">

Capability

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="32.36%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p54150165315">

Function

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="47.9%" id="mcps1.2.4.1.3">

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

   <td class="cellrowborder" rowspan="2" valign="top" width="19.74%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p229610227124">

GPIO read/write

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="32.36%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p19389143041518">

GpioRead

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.9%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p8738101941716">

Reads the level value of a GPIO pin.

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

GpioWrite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p67306152404">

Writes the level value of a GPIO pin.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row17493124814141">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="19.74%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p321814526178">

GPIO settings

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="32.36%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p16390153015156">

GpioSetDir

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.9%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1873761519408">

Sets the direction for a GPIO pin.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row10681146181417">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p15390153014151">

GpioGetDir

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p974061515406">

Obtains the direction for a GPIO pin.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row10288191441518">

.. raw:: html

   <td class="cellrowborder" rowspan="4" valign="top" width="19.74%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p13927416134716">

GPIO interrupt settings

.. raw:: html

   </p>

.. raw:: html

   <p id="p738165912472">

.. raw:: html

   </p>

.. raw:: html

   <p id="p151691515483">

.. raw:: html

   </p>

.. raw:: html

   <p id="p6742119204820">

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="32.36%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p17390113013158">

GpioSetIrq

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.9%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p10314104354416">

Sets the ISR function for a GPIO pin.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row163795912473">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p523618345323">

GpioUnSetIrq

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1138195912478">

Cancels the setting of the ISR function for a GPIO pin.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row155161515124816">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p657344273218">

GpioEnableIrq

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p115163154488">

Enables a GPIO interrupt.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1742119174820">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1865114616324">

GpioDisableIrq

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p97421219174820">

Disables a GPIO interrupt.

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

   |image1| **NOTE:** All functions provided in this document can be
   called only in kernel mode.

.. |image1| image:: public_sys-resources/icon-note.gif
