uart_if.h
=========

**Overview**\ 
--------------

**Related Modules:**

`UART <uart.rst>`__

**Description:**

Declares standard UART APIs.

**Since:**

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

   <tr id="row1576081718093527">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p479694904093527">

Data Structure Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p305471414093527">

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

   <tr id="row195678275093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p430760983093527">

UartAttribute

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1590311422093527">

Defines basic attributes of the UART port.

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

Macros
------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1638574849093527">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1124319015093527">

Macro Name and Value

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p957128434093527">

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

   <tr id="row1637276026093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p479973437093527">

UART_ATTR_DATABIT_8 0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2111789724093527">

Indicates the UART word length, which is 8 data bits per frame.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row94414899093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1486986110093527">

UART_ATTR_DATABIT_7 1

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p547053454093527">

Indicates the UART word length, which is 7 data bits per frame.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row564913763093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1581206974093527">

UART_ATTR_DATABIT_6 2

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p43166249093527">

Indicates the UART word length, which is 6 data bits per frame.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1629846167093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p689691590093527">

UART_ATTR_DATABIT_5 3

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p656397699093527">

Indicates the UART word length, which is 5 data bits per frame.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1705425608093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1694761609093527">

UART_ATTR_PARITY_NONE 0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1417272971093527">

Indicates that the UART device has no parity bit.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1202301849093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1749969521093527">

UART_ATTR_PARITY_ODD 1

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p749088985093527">

Indicates that the UART device has an odd parity bit.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1589773847093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1369867932093527">

UART_ATTR_PARITY_EVEN 2

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1473693677093527">

Indicates that the UART device has an even parity bit.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1636289564093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p467521476093527">

UART_ATTR_PARITY_MARK 3

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p115952420093527">

Indicates that the parity bit is 1.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2027644398093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1705576967093527">

UART_ATTR_PARITY_SPACE 4

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p103653612093527">

Indicates that the parity bit is 0.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row139524069093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1169461258093527">

UART_ATTR_STOPBIT_1 0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p449616698093527">

Indicates that the UART device has 1 stop bit.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1648640070093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p190294640093527">

UART_ATTR_STOPBIT_1P5 1

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1258210614093527">

Indicates that the UART device has 1.5 stop bits.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row84668351093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p344126867093527">

UART_ATTR_STOPBIT_2 2

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1715701436093527">

Indicates that the UART device has 2 stop bits.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1779191568093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p984669101093527">

UART_ATTR_RTS_DIS 0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p602316918093527">

Indicates that Request To Send (RTS) is disabled for the UART device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row493967635093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p124292543093527">

UART_ATTR_RTS_EN 1

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p463896249093527">

Indicates that RTS is enabled for the UART device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1636343005093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1821060740093527">

UART_ATTR_CTS_DIS 0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1395162325093527">

Indicates that Clear To Send (CTS) is disabled for the UART device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1164868689093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p430270146093527">

UART_ATTR_CTS_EN 1

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1897449765093527">

Indicates that CTS is enabled for the UART device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row324196087093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p719333132093527">

UART_ATTR_RX_FIFO_DIS 0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p147045015093527">

Indicates that First In First Out (FIFO) is disabled for the receiving
UART.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1174770426093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p744747470093527">

UART_ATTR_RX_FIFO_EN 1

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p36875678093527">

Indicates that FIFO is enabled for the receiving UART.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1437956432093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1878985920093527">

UART_ATTR_TX_FIFO_DIS 0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p869002595093527">

Indicates that FIFO is disabled for the transmitting UART.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row188347080093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1673292556093527">

UART_ATTR_TX_FIFO_EN 1

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p53611762093527">

Indicates that FIFO is enabled for the transmitting UART.

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

   <tr id="row1557293483093527">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p356314504093527">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1433410403093527">

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

   <tr id="row1837651474093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p150175129093527">

UartTransMode { UART_MODE_RD_BLOCK = 0, UART_MODE_RD_NONBLOCK,
UART_MODE_DMA_RX_EN, UART_MODE_DMA_RX_DIS, UART_MODE_DMA_TX_EN,
UART_MODE_DMA_TX_DIS }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p963091240093527">

Enumerates UART transmission modes.

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

   <tr id="row1682636094093527">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1962704383093527">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p90383042093527">

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

   <tr id="row612414594093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p385950719093527">

UartOpen (uint32_t port)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p973745404093527">

struct DevHandle \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1160200787093527">

Obtains the UART device handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1464353367093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1273698839093527">

UartClose (struct DevHandle \*handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1669185606093527">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p669420015093527">

Releases the UART device handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row882401123093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p419485129093527">

UartRead (struct DevHandle *handle, uint8_t*\ data, uint32_t size)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p140534119093527">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1604485254093527">

Reads data of a specified size from a UART device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row478078031093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p545069818093527">

UartWrite (struct DevHandle *handle, uint8_t*\ data, uint32_t size)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p123306622093527">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p573421610093527">

Writes data of a specified size into a UART device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2087284478093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p788155434093527">

UartGetBaud (struct DevHandle *handle, uint32_t*\ baudRate)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p3049900093527">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p494579193093527">

Obtains the baud rate of the UART device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1915098509093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p415182898093527">

UartSetBaud (struct DevHandle \*handle, uint32_t baudRate)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1801096035093527">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1009914343093527">

Sets the baud rate for the UART device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row639563052093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p370485474093527">

UartGetAttribute (struct DevHandle *handle, struct
UartAttribute*\ attribute)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p846432300093527">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p776272685093527">

Obtains the UART attribute.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row496523685093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p256990546093527">

UartSetAttribute (struct DevHandle *handle, struct
UartAttribute*\ attribute)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1550688130093527">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p658680631093527">

Sets the UART attribute.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row264008761093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p657786213093527">

UartSetTransMode (struct DevHandle \*handle, enum UartTransMode mode)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1589458981093527">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1241233022093527">

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

**Details**\ 
-------------

**Macro Definition Documentation**\ 
------------------------------------

UART_ATTR_CTS_DIS
-----------------

::

   #define UART_ATTR_CTS_DIS   0

**Description:**

Indicates that Clear To Send (CTS) is disabled for the UART device.

UART_ATTR_CTS_EN
----------------

::

   #define UART_ATTR_CTS_EN   1

**Description:**

Indicates that CTS is enabled for the UART device.

UART_ATTR_DATABIT_5
-------------------

::

   #define UART_ATTR_DATABIT_5   3

**Description:**

Indicates the UART word length, which is 5 data bits per frame.

UART_ATTR_DATABIT_6
-------------------

::

   #define UART_ATTR_DATABIT_6   2

**Description:**

Indicates the UART word length, which is 6 data bits per frame.

UART_ATTR_DATABIT_7
-------------------

::

   #define UART_ATTR_DATABIT_7   1

**Description:**

Indicates the UART word length, which is 7 data bits per frame.

UART_ATTR_DATABIT_8
-------------------

::

   #define UART_ATTR_DATABIT_8   0

**Description:**

Indicates the UART word length, which is 8 data bits per frame.

UART_ATTR_PARITY_EVEN
---------------------

::

   #define UART_ATTR_PARITY_EVEN   2

**Description:**

Indicates that the UART device has an even parity bit.

UART_ATTR_PARITY_MARK
---------------------

::

   #define UART_ATTR_PARITY_MARK   3

**Description:**

Indicates that the parity bit is 1.

UART_ATTR_PARITY_NONE
---------------------

::

   #define UART_ATTR_PARITY_NONE   0

**Description:**

Indicates that the UART device has no parity bit.

UART_ATTR_PARITY_ODD
--------------------

::

   #define UART_ATTR_PARITY_ODD   1

**Description:**

Indicates that the UART device has an odd parity bit.

UART_ATTR_PARITY_SPACE
----------------------

::

   #define UART_ATTR_PARITY_SPACE   4

**Description:**

Indicates that the parity bit is 0.

UART_ATTR_RTS_DIS
-----------------

::

   #define UART_ATTR_RTS_DIS   0

**Description:**

Indicates that `Request <request.rst>`__ To Send (RTS) is disabled for
the UART device.

UART_ATTR_RTS_EN
----------------

::

   #define UART_ATTR_RTS_EN   1

**Description:**

Indicates that RTS is enabled for the UART device.

UART_ATTR_RX_FIFO_DIS
---------------------

::

   #define UART_ATTR_RX_FIFO_DIS   0

**Description:**

Indicates that First In First Out (FIFO) is disabled for the receiving
UART.

UART_ATTR_RX_FIFO_EN
--------------------

::

   #define UART_ATTR_RX_FIFO_EN   1

**Description:**

Indicates that FIFO is enabled for the receiving UART.

UART_ATTR_STOPBIT_1
-------------------

::

   #define UART_ATTR_STOPBIT_1   0

**Description:**

Indicates that the UART device has 1 stop bit.

UART_ATTR_STOPBIT_1P5
---------------------

::

   #define UART_ATTR_STOPBIT_1P5   1

**Description:**

Indicates that the UART device has 1.5 stop bits.

UART_ATTR_STOPBIT_2
-------------------

::

   #define UART_ATTR_STOPBIT_2   2

**Description:**

Indicates that the UART device has 2 stop bits.

UART_ATTR_TX_FIFO_DIS
---------------------

::

   #define UART_ATTR_TX_FIFO_DIS   0

**Description:**

Indicates that FIFO is disabled for the transmitting UART.

UART_ATTR_TX_FIFO_EN
--------------------

::

   #define UART_ATTR_TX_FIFO_EN   1

**Description:**

Indicates that FIFO is enabled for the transmitting UART.
