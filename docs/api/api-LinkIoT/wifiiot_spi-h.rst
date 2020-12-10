wifiiot_spi.h
=============

**Overview**\ 
--------------

**Related Modules:**

`Wifiiot <wifiiot.rst>`__

**Description:**

Declares the SPI interface functions.

These functions are used for SPI initialization, deinitialization, and
data transmission.

**Since:**

1.0

**Version:**

1.0

**Summary**\ 
-------------

Data Structures
---------------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1623926920191857">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p47083962191857">

Data Structure Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1960181420191857">

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

   <tr id="row192848201191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1842219091191857">

WifiIotSpiCfgBasicInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1283439341191857">

Defines data communication parameters.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1717925572191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1935028825191857">

WifiIotSpiCfgInitParam

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p912455580191857">

Specifies whether a device is a master or slave device.

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

Typedefs
--------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1020769595191857">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1430668881191857">

Typedef Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p875439481191857">

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

   <tr id="row712456426191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1358868276191857">

SpiIsrFunc) (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p496596547191857">

typedef void(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p916744108191857">

Indicates the SPI callback, which is used in SpiRegisterUsrFunc.

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

Enumerations
------------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1520132006191857">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1698695849191857">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p229732183191857">

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

   <tr id="row1490632918191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1065102588191857">

WifiIotSpiIdx { WIFI_IOT_SPI_ID_0 = 0, WIFI_IOT_SPI_ID_1 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p48207632191857">

Enumerates SPI channel IDs.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row592076863191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1580265225191857">

WifiIotSpiCfgClockCpol { WIFI_IOT_SPI_CFG_CLOCK_CPOL_0,
WIFI_IOT_SPI_CFG_CLOCK_CPOL_1 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1514729589191857">

Enumerates communication polarities.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1423288990191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1834718656191857">

WifiIotSpiCfgClockCpha { WIFI_IOT_SPI_CFG_CLOCK_CPHA_0,
WIFI_IOT_SPI_CFG_CLOCK_CPHA_1 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1723124806191857">

Enumerates communication phases.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row20197199191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1244377543191857">

WifiIotSpiCfgFramMode { WIFI_IOT_SPI_CFG_FRAM_MODE_MOTOROLA,
WIFI_IOT_SPI_CFG_FRAM_MODE_TI, WIFI_IOT_SPI_CFG_FRAM_MODE_MICROWIRE }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1245533784191857">

Enumerates communication protocols.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1233876120191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2014492231191857">

WifiIotSpiCfgDataWidth { WIFI_IOT_SPI_CFG_DATA_WIDTH_E_4BIT = 0x3,
WIFI_IOT_SPI_CFG_DATA_WIDTH_E_5BIT, WIFI_IOT_SPI_CFG_DATA_WIDTH_E_6BIT,
WIFI_IOT_SPI_CFG_DATA_WIDTH_E_7BIT, WIFI_IOT_SPI_CFG_DATA_WIDTH_E_8BIT,
WIFI_IOT_SPI_CFG_DATA_WIDTH_E_9BIT, WIFI_IOT_SPI_CFG_DATA_WIDTH_E_10BIT,
WIFI_IOT_SPI_CFG_DATA_WIDTH_E_11BIT,
WIFI_IOT_SPI_CFG_DATA_WIDTH_E_12BIT,
WIFI_IOT_SPI_CFG_DATA_WIDTH_E_13BIT,
WIFI_IOT_SPI_CFG_DATA_WIDTH_E_14BIT,
WIFI_IOT_SPI_CFG_DATA_WIDTH_E_15BIT, WIFI_IOT_SPI_CFG_DATA_WIDTH_E_16BIT
}

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1666434271191857">

Enumerates the communication data width, that is, the number of valid
bits in each frame.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1623822614191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2097137585191857">

WifiIotSpiCfgEndian { WIFI_IOT_SPI_CFG_ENDIAN_LITTLE,
WIFI_IOT_SPI_CFG_ENDIAN_BIG }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1695624044191857">

Enumerates the endian mode of each frame.

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

Functions
---------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2077268498191857">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p882557170191857">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1502852253191857">

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

   <tr id="row1017908223191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p544972471191857">

SpiSlaveWrite (WifiIotSpiIdx spiId, char \*writeData, unsigned int
byteLen, unsigned int timeOutMs)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p722013933191857">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1110194540191857">

Sends data in SPI slave mode.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row804667765191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1897092600191857">

SpiSlaveRead (WifiIotSpiIdx spiId, char \*readData, unsigned int
byteLen, unsigned int timeOutMs)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p864784018191857">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p25059782191857">

Reads data in SPI slave mode.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1250779572191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1683689026191857">

SpiHostWrite (WifiIotSpiIdx spiId, char \*writeData, unsigned int
byteLen)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1362424277191857">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1651188237191857">

Sends data in half-duplex SPI master mode.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1099711881191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1978895992191857">

SpiHostRead (WifiIotSpiIdx spiId, char \*readData, unsigned int byteLen)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1202009098191857">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1812199332191857">

Reads data in half-duplex SPI master mode.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row902396758191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1323903483191857">

SpiHostWriteread (WifiIotSpiIdx spiId, char *writeData, char*\ readData,
unsigned int byteLen)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2122862332191857">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p2142088501191857">

Sends and reads data in full-duplex SPI master mode.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1081814650191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2028095091191857">

SpiSetBasicInfo (WifiIotSpiIdx spiId, const WifiIotSpiCfgBasicInfo
\*param)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1080294335191857">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1714879284191857">

Sets the SPI channel parameter.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1735299844191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1141881984191857">

SpiInit (WifiIotSpiIdx spiId, WifiIotSpiCfgInitParam initParam, const
WifiIotSpiCfgBasicInfo \*param)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p267383664191857">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1078613680191857">

Initializes an SPI device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row617724963191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p332008562191857">

SpiDeinit (WifiIotSpiIdx spiId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1336967274191857">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p989409488191857">

Deinitializes an SPI device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row324605708191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1805653202191857">

SpiSetIrqMode (WifiIotSpiIdx spiId, unsigned char irqEn)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2117350838191857">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p237304231191857">

Sets whether to enable the interrupt request (IRQ) mode for an SPI
device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1432785067191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1155279580191857">

SpiSetDmaMode (WifiIotSpiIdx spiId, unsigned char dmaEn)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p745401202191857">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p579787806191857">

Sets whether to enable DMA to transfer data for an SPI device in slave
mode.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1674701607191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p153099255191857">

SpiRegisterUsrFunc (WifiIotSpiIdx spiId, SpiIsrFunc prepareF, SpiIsrFunc
restoreF)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1342436760191857">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p360544965191857">

Registers the data TX preparation/recovery function.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1795278142191857">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1620167226191857">

SpiSetLoopBackMode (WifiIotSpiIdx spiId, unsigned char lbEn)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1871245474191857">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1605215172191857">

Sets whether to enable loopback test for an SPI device.

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
