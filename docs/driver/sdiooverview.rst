
SDIO Overview
=============

Introduction
------------

-  Secure Digital Input/Output (SDIO) is a peripheral interface evolved
   from the Secure Digital (SD) memory card interface. The SDIO
   interface is compatible with SD memory cards and can be connected to
   devices that support the SDIO interface.

-  SDIO is widely used. Currently, many smartphones support SDIO, and
   many SDIO peripherals are developed for connections to smartphones.
   Common SDIO peripherals include WLAN, GPS, cameras, and Bluetooth.

-  The SDIO bus has two ends, named host and device. All communication
   starts when the host sends a command. The device can communicate with
   the host as long as it can parse the command of the host. An SDIO
   host can connect to multiple devices, as shown in the figure below.

   1. CLK signal: clock signal sent from the host to the device
   2. VDD signal: power signal
   3. VSS signal: ground signal
   4. D0-3 signal: four data lines. The DAT1 signal cable is multiplexed
      as the interrupt line. In 1-bit mode, DAT0 is used to transmit
      data. In 4-bit mode, DAT0 to DAT3 are used to transmit data.
   5. CMD signal: used by the host to send commands and the device to
      respond to commands.

   **Figure 1** Connections between the host and devices in SDIO

   |image1|

-  The SDIO interface defines a set of common methods for operating an
   SDIO device, including opening and closing an SDIO controller,
   exclusively claiming and releasing the host, enabling and disabling
   devices, claiming and releasing an SDIO IRQ, reading and writing data
   based on SDIO, and obtaining and setting common information.

Available APIs
--------------

**Table 1** APIs available for the SDIO driver

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1625342317507">

.. raw:: html

   <th class="cellrowborder" valign="top" width="21.07%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p1779183435016">

Capability

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="34.04%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p1879163417502">

Function

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="44.89%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p1379113410506">

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

   <tr id="row1351945135614">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="21.07%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p146755118566">

SDIO device opening/closing

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.04%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1151945185614">

SdioOpen

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.89%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p85110451565">

Opens an SDIO controller with a specified bus number.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1062610995616">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p136261793568">

SdioClose

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p062614919566">

Closes an SDIO controller.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row337105133315">

.. raw:: html

   <td class="cellrowborder" rowspan="6" valign="top" width="21.07%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p07631557153319">

SDIO reading/writing

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.04%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p34551320121416">

SdioReadBytes

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.89%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p748062291415">

Incrementally reads a given length of data from a specified SDIO
address.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row9317134301618">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p10345104001412">

SdioWriteBytes

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p113452040141418">

Incrementally writes a given length of data into a specified SDIO
address.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row131301734171616">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p713025410166">

SdioReadBytesFromFixedAddr

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p14130165418168">

Reads a given length of data from a fixed SDIO address.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1434434011147">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1913013546161">

SdioWriteBytesToFixedAddr

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p111301954131614">

Writes a given length of data into a fixed SDIO address.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row364393591410">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1851815711620">

SdioReadBytesFromFunc0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p751875761611">

Reads a given length of data from the address space of SDIO function 0.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row17455333175">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1645519318173">

SdioWriteBytesToFunc0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p114552320176">

Writes a given length of data into the address space of SDIO function 0.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row34145016535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.07%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p229610227124">

SDIO block size setting

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.04%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p74531720181413">

SdioSetBlockSize

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.89%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p247972241411">

Sets the block size.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row778816813238">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="21.07%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1578958142317">

SDIO common information retrieval/setting

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.04%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p378918842311">

SdioGetCommonInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.89%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1078919892313">

Obtains common information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row5667102342417">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2668623182411">

SdioSetCommonInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p14668192362419">

Sets common information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1165101111256">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.07%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p8166161192511">

SDIO data flushing

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.04%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p121662112256">

SdioFlushData

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.89%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p171661711112519">

Flushes data.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row17388101522515">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="21.07%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p53101413268">

SDIO host exclusively claiming or releasing

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.04%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1638881562520">

SdioClaimHost

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.89%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p143881715152517">

Claims a host exclusively.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row5352175517251">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p93537557259">

SdioReleaseHost

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1235355511254">

Releases the exclusively claimed host.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row8759125415269">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="21.07%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p272143815359">

SDIO device enablement

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.04%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p6760195452615">

SdioEnableFunc

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.89%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p9760135417263">

Enables an SDIO device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1166105762620">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p5662175782616">

SdioDisableFunc

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p3662135722618">

Disables an SDIO device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row12332331113517">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="21.07%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p188181849203614">

SDIO IRQ claiming/releasing

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.04%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p933383133517">

SdioClaimIrq

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.89%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p20333431203510">

Claims an SDIO IRQ.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row173103413357">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2073123413515">

SdioReleaseIrq

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1773634153518">

Releases an SDIO IRQ.

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

.. |image1| image:: figures/en-us_image_0000001054280608.png
.. |image2| image:: public_sys-resources/icon-note.gif
