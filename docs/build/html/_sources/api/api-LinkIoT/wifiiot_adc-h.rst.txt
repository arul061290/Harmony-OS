wifiiot_adc.h
=============

**Overview**\ 
--------------

**Related Modules:**

`Wifiiot <wifiiot.md>`__

**Description:**

Declares the ADC interface functions for you to read data.

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

   <tr id="row204622648191854">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p608306791191854">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1968974614191854">

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

   <tr id="row1887911635191854">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1859368802191854">

WifiIotAdcChannelIndex { WIFI_IOT_ADC_CHANNEL_0, WIFI_IOT_ADC_CHANNEL_1,
WIFI_IOT_ADC_CHANNEL_2, WIFI_IOT_ADC_CHANNEL_3, WIFI_IOT_ADC_CHANNEL_4,
WIFI_IOT_ADC_CHANNEL_5, WIFI_IOT_ADC_CHANNEL_6, WIFI_IOT_ADC_CHANNEL_7,
WIFI_IOT_ADC_CHANNEL_BUTT }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1075408095191854">

Enumerates ADC channel indexes.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1215506408191854">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1517257063191854">

WifiIotAdcCurBais { WIFI_IOT_ADC_CUR_BAIS_DEFAULT,
WIFI_IOT_ADC_CUR_BAIS_AUTO, WIFI_IOT_ADC_CUR_BAIS_1P8V,
WIFI_IOT_ADC_CUR_BAIS_3P3V, WIFI_IOT_ADC_CUR_BAIS_BUTT }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p490616047191854">

Enumerates analog power control modes.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row578226971191854">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1754310665191854">

WifiIotAdcEquModelSel { WIFI_IOT_ADC_EQU_MODEL_1,
WIFI_IOT_ADC_EQU_MODEL_2, WIFI_IOT_ADC_EQU_MODEL_4,
WIFI_IOT_ADC_EQU_MODEL_8, WIFI_IOT_ADC_EQU_MODEL_BUTT }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1332022793191854">

Enumerates equation models.

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

   <tr id="row919310821191854">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1293845767191854">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p272062378191854">

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

   <tr id="row873072958191854">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1896691631191854">

AdcRead (WifiIotAdcChannelIndex channel, unsigned short \*data,
WifiIotAdcEquModelSel equModel, WifiIotAdcCurBais curBais, unsigned
short rstCnt)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p562999549191854">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1376349906191854">

Reads a piece of sampled data from a specified ADC channel based on the
input parameters.

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
