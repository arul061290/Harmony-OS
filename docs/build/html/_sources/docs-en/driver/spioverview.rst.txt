SPI Overview
============

Introduction
------------

-  Serial Peripheral Interface (SPI) is a serial bus specification used
   for high-speed, full-duplex, and synchronous communication.
-  SPI is developed by Motorola. It is commonly used for communication
   with flash memory, real-time clocks, sensors, and analog-to-digital
   (A/D) converters.
-  SPI works in controller/device mode. Generally, there is one SPI
   controller that controls one or more SPI devices. They are connected
   via four wires:

   -  SCLK: clock signals output from the SPI controller
   -  MOSI: data output from the SPI controller and input into a SPI
      device
   -  MISO: data output from a SPI device and input into the SPI
      controller
   -  CS: signals enabled by a SPI device and controlled by the SPI
      controller

-  `Figure 1 <#fig15227181812587>`__ shows the connection between one
   SPI controller and two SPI devices (Device A and Device B). In this
   figure, Device A and Device B share three pins (SCLK, MISO, and MOSI)
   of the controller. CS0 of Device A and CS1 of Device B are connected
   to CS0 and CS1 of the controller, respectively.

**Figure 1** SPI controller/device connection

|image1|

-  SPI communication is usually initiated by a controller and is
   operated as follows:

1. A single SPI device is selected at a time via the CS to communicate
   with the SPI controller.
2. Clock signals are provided for the selected SPI device via the SCLK.
3. SPI controller sends data to SPI devices via the MOSI, and receives
   data from SPI devices via the MISO.

-  SPI can work in one of the following four modes, equivalent to one of
   the four possible states for Clock Polarity (CPOL) and Clock Phase
   (CPHA):

   -  When both CPOL and CPHA are **0**, the clock signal level is low
      in the idle state and data is sampled on the first clock edge.
   -  When CPOL is **0** and CPHA is **1**, the clock signal level is
      low in the idle state and data is sampled on the second clock
      edge.
   -  When CPOL is **1** and CPHA is **0**, the clock signal level is
      high in the idle state and data is sampled on the first clock
      edge.
   -  When both CPOL and CPHA are **1**, the clock signal level is high
      in the idle state and data is sampled on the second clock edge.

-  SPI defines a set of common functions for operating an SPI device,
   including those for:

   -  Obtaining and releasing the handle of an SPI device.
   -  Reading or writing data of a specified length from or into an SPI
      device.
   -  Customizing data reading or writing via **SpiMsg**.
   -  Obtaining and setting SPI device configuration parameters.

..

   |image2| **NOTE:** Currently, these functions are only applicable in
   the communication initiated by the SPI controller.

Available APIs
--------------

**Table 1** APIs for the SPI driver

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row4419501537">

.. raw:: html

   <th class="cellrowborder" align="left" valign="top" width="20.857914208579142%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p641050105320">

Capability

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" align="left" valign="top" width="23.36766323367663%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p54150165315">

Function

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" align="left" valign="top" width="55.77442255774422%" id="mcps1.2.4.1.3">

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

   <tr id="row1651292212306">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="20.857914208579142%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1387414255305">

SPI device handle obtaining/releasing

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="23.36766323367663%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p8874825143014">

SpiOpen

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.77442255774422%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1087432513307">

Obtains an SPI device handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1429083612305">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1956614106311">

SpiClose

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p829111362306">

Releases an SPI device handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row34145016535">

.. raw:: html

   <td class="cellrowborder" rowspan="3" valign="top" width="20.857914208579142%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p229610227124">

SPI reading/writing

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="23.36766323367663%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p19389143041518">

SpiRead

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.77442255774422%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p8738101941716">

Reads data of a specified length from an SPI device.

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

SpiWrite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p573815197171">

Writes data of a specified length into an SPI device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1766145611414">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p183904373018">

SpiTransfer

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1639011313303">

Transfers SPI data.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1020919129159">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="20.857914208579142%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p82092126154">

SPI device configuration

.. raw:: html

   </p>

.. raw:: html

   <p id="p6794153701111">

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="23.36766323367663%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1739013012154">

SpiSetCfg

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.77442255774422%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p073910197173">

Sets configuration parameters for an SPI device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row379443710118">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p4333154919111">

SpiGetCfg

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p11333649171117">

Obtains configuration parameters of an SPI device.

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

.. |image1| image:: figures/en-us_image_0000001054142582.png
.. |image2| image:: public_sys-resources/icon-note.gif
.. |image3| image:: public_sys-resources/icon-note.gif
