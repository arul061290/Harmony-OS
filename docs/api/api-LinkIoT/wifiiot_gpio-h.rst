wifiiot_gpio.h
==============

**Overview**\ 
--------------

**Related Modules:**

`Wifiiot <wifiiot.rst>`__

**Description:**

Declares the GPIO interface functions.

These functions are used for GPIO initialization, input/output settings,
and level settings.

**Since:**

1.0

**Version:**

1.0

**Summary**\ 
-------------

Typedefs
--------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row26631136090254">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2014337425090254">

Typedef Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1808429966090254">

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

   <tr id="row1915468740090254">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p952521528090254">

GpioIsrCallbackFunc) (char \*arg)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p936383860090254">

typedef void(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1358194646090254">

Indicates the GPIO interrupt callback.

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

   <tr id="row133310045090254">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1935380932090254">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1519810347090254">

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

   <tr id="row1406436292090254">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p791366284090254">

WifiIotGpioIdx { WIFI_IOT_GPIO_IDX_0, WIFI_IOT_GPIO_IDX_1,
WIFI_IOT_GPIO_IDX_2, WIFI_IOT_GPIO_IDX_3, WIFI_IOT_GPIO_IDX_4,
WIFI_IOT_GPIO_IDX_5, WIFI_IOT_GPIO_IDX_6, WIFI_IOT_GPIO_IDX_7,
WIFI_IOT_GPIO_IDX_8, WIFI_IOT_GPIO_IDX_9, WIFI_IOT_GPIO_IDX_10,
WIFI_IOT_GPIO_IDX_11, WIFI_IOT_GPIO_IDX_12, WIFI_IOT_GPIO_IDX_13,
WIFI_IOT_GPIO_IDX_14, WIFI_IOT_GPIO_IDX_MAX }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p186481113090254">

Enumerates GPIO pin IDs.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1370304482090254">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p766414750090254">

WifiIotGpioValue { WIFI_IOT_GPIO_VALUE0 = 0, WIFI_IOT_GPIO_VALUE1 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p504066823090254">

Enumerates GPIO level values.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1355282876090254">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2026015515090254">

WifiIotGpioDir { WIFI_IOT_GPIO_DIR_IN = 0, WIFI_IOT_GPIO_DIR_OUT }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1102993096090254">

Enumerates GPIO directions.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1093809338090254">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p201204979090254">

WifiIotGpioIntType { WIFI_IOT_INT_TYPE_LEVEL = 0, WIFI_IOT_INT_TYPE_EDGE
}

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p152585455090254">

Enumerates GPIO interrupt trigger modes.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1316922068090254">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1871372736090254">

WifiIotGpioIntPolarity { WIFI_IOT_GPIO_EDGE_FALL_LEVEL_LOW = 0,
WIFI_IOT_GPIO_EDGE_RISE_LEVEL_HIGH }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p764042903090254">

Enumerates I/O interrupt polarities.

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

   <tr id="row746943002090254">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1228854830090254">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1121677929090254">

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

   <tr id="row1877745666090254">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1366045778090254">

GpioInit (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1132903766090254">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1017619052090254">

Initializes the GPIO device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2137327258090254">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p150500764090254">

GpioDeinit (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1813847013090254">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1765244765090254">

Deinitializes the GPIO device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1441452640090254">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1998396903090254">

GpioSetDir (WifiIotGpioIdx id, WifiIotGpioDir dir)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1421345736090254">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1030751011090254">

Sets the direction for a GPIO pin.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2060255365090254">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1978493145090254">

GpioGetDir (WifiIotGpioIdx id, WifiIotGpioDir \*dir)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1102045117090254">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p2012395084090254">

Obtains the direction for a GPIO pin.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row740134336090254">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p530816021090254">

GpioSetOutputVal (WifiIotGpioIdx id, WifiIotGpioValue val)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1849944257090254">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1446602266090254">

Sets the output level value for a GPIO pin.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1412893519090254">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p784978477090254">

GpioGetOutputVal (WifiIotGpioIdx id, WifiIotGpioValue \*val)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p181595591090254">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p255447410090254">

Obtains the output level value of a GPIO pin.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row639271764090254">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p713259073090254">

GpioGetInputVal (WifiIotGpioIdx id, WifiIotGpioValue \*val)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1434138008090254">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1429757194090254">

Obtains the input level value of a GPIO pin.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row419595560090254">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p84399686090254">

GpioRegisterIsrFunc (WifiIotGpioIdx id, WifiIotGpioIntType intType,
WifiIotGpioIntPolarity intPolarity, GpioIsrCallbackFunc func, char
\*arg)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p411799188090254">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1644237183090254">

Enables the interrupt function for a GPIO pin.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1454933842090254">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p637877477090254">

GpioUnregisterIsrFunc (WifiIotGpioIdx id)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p587263959090254">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1048546097090254">

Disables the interrupt function for a GPIO pin.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2022922321090254">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p714383288090254">

GpioSetIsrMask (WifiIotGpioIdx id, unsigned char mask)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1975822543090254">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1983743039090254">

Masks the interrupt function for a GPIO pin.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row81988572090254">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p837411698090254">

GpioSetIsrMode (WifiIotGpioIdx id, WifiIotGpioIntType intType,
WifiIotGpioIntPolarity intPolarity)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1885265174090254">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p2018073552090254">

Sets the interrupt trigger mode of a GPIO pin.

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
