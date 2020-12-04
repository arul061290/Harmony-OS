wifiiot_gpio_ex.h
=================

**Overview**\ 
--------------

**Related Modules:**

`Wifiiot <wifiiot.md>`__

**Description:**

Declares the extended GPIO interface functions.

These functions are used for settings GPIO pulls and driver strength.

**Since:**

1.0

**Version:**

1.0

**Summary**\ 
-------------

Enumerations
------------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1923223240191855">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p463847437191855">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1541683396191855">

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

   <tr id="row941234300191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p227114784191855">

WifiIotIoName { WIFI_IOT_IO_NAME_GPIO_0, WIFI_IOT_IO_NAME_GPIO_1,
WIFI_IOT_IO_NAME_GPIO_2, WIFI_IOT_IO_NAME_GPIO_3,
WIFI_IOT_IO_NAME_GPIO_4, WIFI_IOT_IO_NAME_GPIO_5,
WIFI_IOT_IO_NAME_GPIO_6, WIFI_IOT_IO_NAME_GPIO_7,
WIFI_IOT_IO_NAME_GPIO_8, WIFI_IOT_IO_NAME_GPIO_9,
WIFI_IOT_IO_NAME_GPIO_10, WIFI_IOT_IO_NAME_GPIO_11,
WIFI_IOT_IO_NAME_GPIO_12, WIFI_IOT_IO_NAME_GPIO_13,
WIFI_IOT_IO_NAME_GPIO_14, WIFI_IOT_IO_NAME_MAX }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1827688024191855">

Enumerates GPIO hardware pin IDs.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row748543777191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p672095043191855">

WifiIotIoFuncGpio0 { WIFI_IOT_IO_FUNC_GPIO_0_GPIO,
WIFI_IOT_IO_FUNC_GPIO_0_UART1_TXD = 2, WIFI_IOT_IO_FUNC_GPIO_0_SPI1_CK,
WIFI_IOT_IO_FUNC_GPIO_0_JTAG_TDO, WIFI_IOT_IO_FUNC_GPIO_0_PWM3_OUT,
WIFI_IOT_IO_FUNC_GPIO_0_I2C1_SDA }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p931018453191855">

Enumerates the functions of GPIO hardware pin 0.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row818982764191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2099804926191855">

WifiiIotIoFuncGpio1 { WIFI_IOT_IO_FUNC_GPIO_1_GPIO }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2129370089191855">

Enumerates the functions of GPIO hardware pin 1.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row754706440191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1378806986191855">

WifiIotIoFuncGpio2 { WIFI_IOT_IO_FUNC_GPIO_2_GPIO,
WIFI_IOT_IO_FUNC_GPIO_2_UART1_RTS_N = 2,
WIFI_IOT_IO_FUNC_GPIO_2_SPI1_TXD, WIFI_IOT_IO_FUNC_GPIO_2_JTAG_TRSTN,
WIFI_IOT_IO_FUNC_GPIO_2_PWM2_OUT, WIFI_IOT_IO_FUNC_GPIO_2_SSI_CLK = 7 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1306968485191855">

Enumerates the functions of GPIO hardware pin 2.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1204772861191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p243258400191855">

WifiIotIoFuncGpio3 { WIFI_IOT_IO_FUNC_GPIO_3_GPIO,
WIFI_IOT_IO_FUNC_GPIO_3_UART0_TXD, WIFI_IOT_IO_FUNC_GPIO_3_UART1_CTS_N,
WIFI_IOT_IO_FUNC_GPIO_3_SPI1_CSN, WIFI_IOT_IO_FUNC_GPIO_3_JTAG_TDI,
WIFI_IOT_IO_FUNC_GPIO_3_PWM5_OUT, WIFI_IOT_IO_FUNC_GPIO_3_I2C1_SDA,
WIFI_IOT_IO_FUNC_GPIO_3_SSI_DATA }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1141988592191855">

Enumerates the functions of GPIO hardware pin 3.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1874411640191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p832690429191855">

WifiIotIoFuncGpio4 { WIFI_IOT_IO_FUNC_GPIO_4_GPIO,
WIFI_IOT_IO_FUNC_GPIO_4_UART0_RXD = 2, WIFI_IOT_IO_FUNC_GPIO_4_JTAG_TMS
= 4, WIFI_IOT_IO_FUNC_GPIO_4_PWM1_OUT, WIFI_IOT_IO_FUNC_GPIO_4_I2C1_SCL
}

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1413819347191855">

Enumerates the functions of GPIO hardware pin 4.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2043658420191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2116967066191855">

WifiIotIoFuncGpio5 { WIFI_IOT_IO_FUNC_GPIO_5_GPIO,
WIFI_IOT_IO_FUNC_GPIO_5_UART1_RXD = 2, WIFI_IOT_IO_FUNC_GPIO_5_SPI0_CSN,
WIFI_IOT_IO_FUNC_GPIO_5_PWM2_OUT = 5, WIFI_IOT_IO_FUNC_GPIO_5_I2S0_MCLK,
WIFI_IOT_IO_FUNC_GPIO_5_BT_STATUS }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1221900176191855">

Enumerates the functions of GPIO hardware pin 5.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2125104688191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1248045812191855">

WifiIotIoFuncGpio6 { WIFI_IOT_IO_FUNC_GPIO_6_GPIO,
WIFI_IOT_IO_FUNC_GPIO_6_UART1_TXD = 2, WIFI_IOT_IO_FUNC_GPIO_6_SPI0_CK,
WIFI_IOT_IO_FUNC_GPIO_6_PWM3_OUT = 5, WIFI_IOT_IO_FUNC_GPIO_6_I2S0_TX,
WIFI_IOT_IO_FUNC_GPIO_6_COEX_SWITCH }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1903805650191855">

Enumerates the functions of GPIO hardware pin 6.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row394032662191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1901842529191855">

WifiIotIoFuncGpio7 { WIFI_IOT_IO_FUNC_GPIO_7_GPIO,
WIFI_IOT_IO_FUNC_GPIO_7_UART1_CTS_N = 2,
WIFI_IOT_IO_FUNC_GPIO_7_SPI0_RXD, WIFI_IOT_IO_FUNC_GPIO_7_PWM0_OUT = 5,
WIFI_IOT_IO_FUNC_GPIO_7_I2S0_BCLK, WIFI_IOT_IO_FUNC_GPIO_7_BT_ACTIVE }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1673206689191855">

Enumerates the functions of GPIO hardware pin 7.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1131072795191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1527128916191855">

WifiIotIoFuncGpio8 { WIFI_IOT_IO_FUNC_GPIO_8_GPIO,
WIFI_IOT_IO_FUNC_GPIO_8_UART1_RTS_N = 2,
WIFI_IOT_IO_FUNC_GPIO_8_SPI0_TXD, WIFI_IOT_IO_FUNC_GPIO_8_PWM1_OUT = 5,
WIFI_IOT_IO_FUNC_GPIO_8_I2S0_WS, WIFI_IOT_IO_FUNC_GPIO_8_WLAN_ACTIVE }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p298400775191855">

Enumerates the functions of GPIO hardware pin 8.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1263273151191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1396515134191855">

WifiIotIoFuncGpio9 { WIFI_IOT_IO_FUNC_GPIO_9_GPIO,
WIFI_IOT_IO_FUNC_GPIO_9_I2C0_SCL, WIFI_IOT_IO_FUNC_GPIO_9_UART2_RTS_N,
WIFI_IOT_IO_FUNC_GPIO_9_SDIO_D2, WIFI_IOT_IO_FUNC_GPIO_9_SPI0_TXD,
WIFI_IOT_IO_FUNC_GPIO_9_PWM0_OUT, WIFI_IOT_IO_FUNC_GPIO_9_I2S0_MCLK = 7
}

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1327261295191855">

Enumerates the functions of GPIO hardware pin 9.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row671900722191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p347001875191855">

WifiIotIoFuncGpio10 { WIFI_IOT_IO_FUNC_GPIO_10_GPIO,
WIFI_IOT_IO_FUNC_GPIO_10_I2C0_SDA, WIFI_IOT_IO_FUNC_GPIO_10_UART2_CTS_N,
WIFI_IOT_IO_FUNC_GPIO_10_SDIO_D3, WIFI_IOT_IO_FUNC_GPIO_10_SPI0_CK,
WIFI_IOT_IO_FUNC_GPIO_10_PWM1_OUT, WIFI_IOT_IO_FUNC_GPIO_10_I2S0_TX = 7
}

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1139072309191855">

Enumerates the functions of GPIO hardware pin 10.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1161784794191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1916899317191855">

WifiIotIoFuncGpio11 { WIFI_IOT_IO_FUNC_GPIO_11_GPIO,
WIFI_IOT_IO_FUNC_GPIO_11_UART2_TXD = 2,
WIFI_IOT_IO_FUNC_GPIO_11_SDIO_CMD, WIFI_IOT_IO_FUNC_GPIO_11_SPI0_RXD,
WIFI_IOT_IO_FUNC_GPIO_11_PWM2_OUT,
WIFI_IOT_IO_FUNC_GPIO_11_RF_TX_EN_EXT, WIFI_IOT_IO_FUNC_GPIO_11_I2S0_RX
}

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1910803656191855">

Enumerates the functions of GPIO hardware pin 11.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row71608615191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1059426275191855">

WifiIotIoFuncGpio12 { WIFI_IOT_IO_FUNC_GPIO_12_GPIO,
WIFI_IOT_IO_FUNC_GPIO_12_UART2_RXD = 2,
WIFI_IOT_IO_FUNC_GPIO_12_SDIO_CLK, WIFI_IOT_IO_FUNC_GPIO_12_SPI0_CSN,
WIFI_IOT_IO_FUNC_GPIO_12_PWM3_OUT,
WIFI_IOT_IO_FUNC_GPIO_12_RF_RX_EN_EXT,
WIFI_IOT_IO_FUNC_GPIO_12_I2S0_BCLK }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p358111920191855">

Enumerates the functions of GPIO hardware pin 12.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1265377075191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p14034757191855">

WifiIotIoFuncGpio13 { WIFI_IOT_IO_FUNC_GPIO_13_SSI_DATA,
WIFI_IOT_IO_FUNC_GPIO_13_UART0_TXD,
WIFI_IOT_IO_FUNC_GPIO_13_UART2_RTS_N, WIFI_IOT_IO_FUNC_GPIO_13_SDIO_D0,
WIFI_IOT_IO_FUNC_GPIO_13_GPIO, WIFI_IOT_IO_FUNC_GPIO_13_PWM4_OUT,
WIFI_IOT_IO_FUNC_GPIO_13_I2C0_SDA, WIFI_IOT_IO_FUNC_GPIO_13_I2S0_WS }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1338189786191855">

Enumerates the functions of GPIO hardware pin 13.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1693674190191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1611461836191855">

WifiIotIoFuncGpio14 { WIFI_IOT_IO_FUNC_GPIO_14_SSI_CLK,
WIFI_IOT_IO_FUNC_GPIO_14_UART0_RXD,
WIFI_IOT_IO_FUNC_GPIO_14_UART2_CTS_N, WIFI_IOT_IO_FUNC_GPIO_14_SDIO_D1,
WIFI_IOT_IO_FUNC_GPIO_14_GPIO, WIFI_IOT_IO_FUNC_GPIO_14_PWM5_OUT,
WIFI_IOT_IO_FUNC_GPIO_14_I2C0_SCL }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p696172478191855">

Enumerates the functions of GPIO hardware pin 14.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row493352952191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p733664900191855">

WifiIotIoDriverStrength { WIFI_IOT_IO_DRIVER_STRENGTH_0 = 0,
WIFI_IOT_IO_DRIVER_STRENGTH_1, WIFI_IOT_IO_DRIVER_STRENGTH_2,
WIFI_IOT_IO_DRIVER_STRENGTH_3, WIFI_IOT_IO_DRIVER_STRENGTH_4,
WIFI_IOT_IO_DRIVER_STRENGTH_5, WIFI_IOT_IO_DRIVER_STRENGTH_6,
WIFI_IOT_IO_DRIVER_STRENGTH_7, WIFI_IOT_IO_DRIVER_STRENGTH_MAX }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1940553004191855">

Enumerates I/O driver strength levels.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row188735532191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1929724730191855">

WifiIotIoPull { WIFI_IOT_IO_PULL_NONE, WIFI_IOT_IO_PULL_UP,
WIFI_IOT_IO_PULL_DOWN, WIFI_IOT_IO_PULL_MAX }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1626436920191855">

Enumerates GPIO pull-up or pull-down settings.

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

   <tr id="row1135034810191855">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1705089723191855">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1557842670191855">

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

   <tr id="row1431638042191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1436768789191855">

IoSetPull (WifiIotIoName id, WifiIotIoPull val)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1212835318191855">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p143088046191855">

Sets the pull for a GPIO pin.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1214420909191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1986833851191855">

IoSetFunc (WifiIotIoName id, unsigned char val)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p749841875191855">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p953474949191855">

Sets the multiplexing function for a GPIO pin.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1808513915191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1973366603191855">

IoGetPull (WifiIotIoName id, WifiIotIoPull \*val)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1327149614191855">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p38986411191855">

Obtains the pull type of a GPIO pin.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row279108655191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p847359784191855">

IoGetFunc (WifiIotIoName id, unsigned char \*val)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p240121022191855">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p283154257191855">

Obtains the multiplexing function for a GPIO pin.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row716609789191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1677140020191855">

IOGetDriverStrength (WifiIotIoName id, WifiIotIoDriverStrength \*val)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p785812322191855">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p717161299191855">

Obtains the driver strength of a GPIO pin.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row802220655191855">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p114466196191855">

IOSetDriverStrength (WifiIotIoName id, WifiIotIoDriverStrength val)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1970081170191855">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1172105982191855">

Sets the driver strength of a GPIO pin.

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
