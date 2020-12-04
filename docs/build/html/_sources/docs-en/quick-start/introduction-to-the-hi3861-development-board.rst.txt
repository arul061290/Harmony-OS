Introduction to the Hi3861 Development Board
============================================

This document describes how to quickly start with the Hi3861 WLAN
module, including the development environment setup, version compiling
and building, device burning, source code modification, debugging and
verification. Following this guide, you can start developing services
with the basic understanding of the Hi3861 WLAN module.

Hi3861
------

The Hi3861 WLAN module is a development board with 2 x 5 cm form factor.
It contains a 2.4 GHz WLAN SoC that highly integrates the IEEE
802.11b/g/n baseband and radio frequency (RF) circuit. This module
provides open and easy-to-use development and debugging environments for
running OpenHarmony.

| **Figure 1** Appearance of Hi3861 WLAN module
| |image1|

The Hi3861 WLAN module can also be connected to the Hi3861 mother board
to expand its peripheral capabilities. The following figure shows the
Hi3861 mother board.

| **Figure 2** Appearance of the Hi3861 mother board
| |image2|

-  The RF circuit includes modules such as the power amplifier (PA), low
   noise amplifier (LNA), RF Balun, antenna switch, and power
   management. It supports a standard bandwidth of 20 MHz and a narrow
   bandwidth of 5 MHz or 10 MHz, and provides a maximum rate of 72.2
   Mbit/s at the physical layer.

-  The Hi3861 WLAN baseband supports the orthogonal frequency division
   multiplexing (OFDM) technology and is backward compatible with the
   direct sequence spread spectrum (DSSS) and complementary code keying
   (CCK) technologies. In addition, the Hi3861 WLAN baseband supports
   various data rates specified in the IEEE 802.11 b/g/n protocol.

-  The Hi3861 chip integrates the high-performance 32-bit
   microprocessor, hardware security engine, and various peripheral
   interfaces. The peripheral interfaces include the Synchronous
   Peripheral Interface (SPI), Universal Asynchronous Receiver &
   Transmitter (UART), the Inter Integrated Circuit (I2C), Pulse Width
   Modulation (PWM), General Purpose Input/Output (GPIO) interface, and
   Analog to Digital Converter (ADC). The Hi3861 chip also supports the
   high-speed Secure Digital Input/Output (SDIO) 2.0 interface, with a
   maximum clock frequency of 50 MHz. This chip has a built-in static
   random access memory (SRAM) and flash memory, so that programs can
   run independently or run from a flash drive.

-  The Hi3861 chip applies to Internet of Things (IoT) devices such as
   smart home appliances.

   **Figure 3** Hi3861 functions

   |image3|

Resources and Constraints
-------------------------

As the Hi3861 only offers 2 MB Flash and 352 KB RAM, use them
efficiently when compiling code.

Development Board Specifications
--------------------------------

**Table 1** Hi3861 WLAN module specifications

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="r54b3810e43d24e1887c1d6a41394996b">

.. raw:: html

   <th class="cellrowborder" valign="top" width="18.060000000000002%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="a2b235e9ed55f4338886788f140e648a0">

Type

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="81.94%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="a95c4ba2e404f4a45b65984746aaa56ab">

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

   <tr id="r71f534ea66af4191b020408df5978f41">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="a0531f1bb62d5443880576cc5de23f2e6">

General specifications

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="81.94%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <ul id="u2a0d06f28d454d30818ced9a0432211b">

.. raw:: html

   <li>

Operates over 1×1 2.4 GHz frequency band (ch1-ch14).

.. raw:: html

   </li>

.. raw:: html

   <li>

The physical layer (PHY) complies with the IEEE 802.11b/g/n protocol.

.. raw:: html

   </li>

.. raw:: html

   <li>

The media access control (MAC) layer complies with the IEEE802.11
d/e/h/i/k/v/w protocol.

.. raw:: html

   </li>

.. raw:: html

   </ul>

.. raw:: html

   <ul id="u8f31d142d92147789195a18b50836d2c">

.. raw:: html

   <li>

Includes the built-in public address (PA) and local area network (LAN);
integrates transmit-receive (Tx/Rx) switch and Balun.

.. raw:: html

   </li>

.. raw:: html

   <li>

Supports the station (STA) and access point (AP) modes. When the Hi3861
WLAN module functions as an AP, a maximum of six STAs are supported.

.. raw:: html

   </li>

.. raw:: html

   <li>

Supports WFA WPA, WFA WPA2 personal, and WPS2.0.

.. raw:: html

   </li>

.. raw:: html

   <li>

Supports three kinds of packet traffic arbiter (PTA) (2- , 3- , or
4-wire PTA), each of which coexists with the BT or BLE chip.

.. raw:: html

   </li>

.. raw:: html

   <li>

The input voltage ranges from 2.3 V to 3.6 V.

.. raw:: html

   </li>

.. raw:: html

   </ul>

.. raw:: html

   <ul id="ul114549122110">

.. raw:: html

   <li>

The input/output (I/O) power voltage can be 1.8 V or 3.3 V.

.. raw:: html

   </li>

.. raw:: html

   </ul>

.. raw:: html

   <ul id="ue044275c53b84dd29dda674e16e72823">

.. raw:: html

   <li>

Supports self-calibration for RF hardware.

.. raw:: html

   </li>

.. raw:: html

   <li>

Performs with low power consumption:

.. raw:: html

   <ul id="ul0879143622219">

.. raw:: html

   <li>

Ultra deep sleep mode: 5 μA @ 3.3 V

.. raw:: html

   </li>

.. raw:: html

   <li>

DTIM1: 1.5 mA @ 3.3 V

.. raw:: html

   </li>

.. raw:: html

   <li>

DTIM3: 0.8 mA @ 3.3 V

.. raw:: html

   </li>

.. raw:: html

   </ul>

.. raw:: html

   </li>

.. raw:: html

   </ul>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="rd9b56e759af34950b6887ca1bf5bb7cf">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="a0aed3860a78a4b50bedf60699afd3996">

PHY features

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="81.94%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <ul id="u6568aa052152432aa1f44372445ca634">

.. raw:: html

   <li>

Supports all data rates of the single antenna required by the
IEEE802.11b/g/n protocol.

.. raw:: html

   </li>

.. raw:: html

   <li>

Supports a maximum rate of 72.2 Mbps@HT20 MCS7

.. raw:: html

   </li>

.. raw:: html

   <li>

Supports the standard bandwidth (20 MHz) and narrow bandwidth (5 MHz or
10 MHz).

.. raw:: html

   </li>

.. raw:: html

   <li>

Supports space-time block coding (STBC).

.. raw:: html

   </li>

.. raw:: html

   <li>

Supports short guard interval (Short-GI).

.. raw:: html

   </li>

.. raw:: html

   </ul>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="r3563f9df9759486794952d46c5d2d03f">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="afd48a2d879dc4aada8b60bebb96523c7">

MAC features

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="81.94%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <ul id="uca57d799e7814925a5bf1b891335bd79">

.. raw:: html

   <li>

Supports aggregate MAC service data unit (A-MPDU) and aggregate MAC
protocol data unit (A-MSDU).

.. raw:: html

   </li>

.. raw:: html

   <li>

Supports block acknowledgment (Blk-ACK).

.. raw:: html

   </li>

.. raw:: html

   <li>

Supports quality of service (QoS), meeting customer’s service
requirements.

.. raw:: html

   </li>

.. raw:: html

   </ul>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="r3e1c86e5f6cd4df0a1b30a08fb8481a2">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="a57086ea97a1b46cdb21953bf0fc22d94">

CPU subsystem

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="81.94%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <ul id="u612cc2cd0cfe40229263c4f506c0c69c">

.. raw:: html

   <li>

Integrates a high-performance 32-bit microprocessor with a maximum
operating frequency of 160 MHz.

.. raw:: html

   </li>

.. raw:: html

   <li>

Includes built-in 352 KB SRAM and 288 KB ROM.

.. raw:: html

   </li>

.. raw:: html

   <li>

Includes a built-in 2 MB flash memory.

.. raw:: html

   </li>

.. raw:: html

   </ul>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="rae93c5236b084cd2a2c0d5c29027b40e">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="a9b14a9e95b3849278c332259d8add1b2">

Peripheral interfaces

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="81.94%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <ul id="u7c73ebffd89e4092bd65f0d878d59b22">

.. raw:: html

   <li>

Include one SDIO interface, two SPI interfaces, two I2C interfaces,
three UART interfaces, 15 GPIO interfaces, seven ADC inputs, six PWM
interfaces, and one I2S interface (Note: These interfaces are all
multiplexed.)

.. raw:: html

   </li>

.. raw:: html

   <li>

The frequency of the external primary crystal oscillator is 40 MHz or 24
MHz.

.. raw:: html

   </li>

.. raw:: html

   </ul>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="r18810701aafe42ad8d9a7d882730c210">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="ae8f47db913724e458c265e858409950b">

Other information

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="81.94%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <ul id="u25f28919a3b044c5af50f9f5f5616083">

.. raw:: html

   <li>

Package: QFN-32, 5 mm x 5 mm

.. raw:: html

   </li>

.. raw:: html

   <li>

Operating temperature: –40°C to +85°C

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

Key Features
------------

OpenHarmony provides a series of available capabilities based on the
Hi3861 platform. The following table describes the available key
components.

**Table 2** Key components

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1368918486512">

.. raw:: html

   <th class="cellrowborder" valign="top" width="22.56%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p668914812516">

Component

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="77.44%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p9689154855115">

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

   <tr id="row868910487517">

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.56%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p13689248165114">

wlan

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="77.44%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p11689144816511">

Provides WLAN service, such as connecting to or disconnecting from a
station or hotspot, and querying the state of a station or hotspot.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row568964819514">

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.56%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p5689548175113">

iot controller

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="77.44%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p176893480517">

Provides the capability of operating peripherals, including the I2C,
I2S, ADC, UART, SPI, SDIO, GPIO, PWM and FLASH.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row143420119366">

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.56%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1737117331480">

soft bus

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="77.44%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1037123314485">

Provides the capabilities of device discovery and data transmission in
the distributed network.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1383559163617">

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.56%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p2379233113914">

hichainsdk

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="77.44%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p5809349205012">

Provides the capability of securely transferring data between devices
when they are interconnected.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row54428163612">

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.56%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p3775133619587">

huks

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="77.44%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p11304151710555">

Provides capabilities of key management, encryption, and decryption.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row12690548135110">

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.56%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p176901648115111">

system ability manager

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="77.44%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1181353173111">

Provides a unified OpenHarmony service development framework based on
the service-oriented architecture.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1657310121587">

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.56%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p730664220114">

bootstrap

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="77.44%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p39689262310">

Provides the entry identifier for starting a system service. When the
system service management is started, the function identified by
bootstrap is called to start a system service.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row15763812165616">

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.56%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p17171118128">

syspara

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="77.44%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p12763912125617">

Provides capabilities of obtaining and setting system attributes.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row121911343566">

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.56%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1097517270361">

utils

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="77.44%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p6848159569">

Provides basic and public capabilities, such as file operations and
key-value (KV) storage management.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row144219192579">

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.56%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p8333104843714">

DFX

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="77.44%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p65111025155711">

Provides the DFX capabilities, such as logging and printing.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row16159522125710">

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.56%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p18835202765718">

XTS

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="77.44%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p3835192795717">

Provides a set of OpenHarmony certification test suites.

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

.. |image1| image:: figures/appearance-of-hi3861-wlan-module.png
.. |image2| image:: figures/appearance-of-the-hi3861-mother-board.png
.. |image3| image:: figures/en-us_image_0000001055187339.png
