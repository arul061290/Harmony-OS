OHOS::EasingEquation
====================

**Overview**\ 
--------------

**Related Modules:**

`Graphic <graphic.rst>`__

**Description:**

Defines functions for specifying the velocity of an animation.

**Since:**

1.0

**Version:**

1.0

**Summary**\ 
-------------

Static Public Member Functions
------------------------------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row991524357093533">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2008444026093533">

Static Public Member Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2011007768093533">

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

   <tr id="row204898760093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1129395481093533">

SetBackOvershoot (double overshoot)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p444352841093533">

static void

.. raw:: html

   </p>

.. raw:: html

   <p id="p620162213093533">

Sets the parameter s in the equation (s+1)\ *t^3 - s*\ t^2 for a back
easing.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1902060137093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p907441044093533">

BackEaseIn (int16_t startPos, int16_t endPos, uint16_t curTime, uint16_t
durationTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1743250192093533">

static int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2008280688093533">

Eases in with an overshoot.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row504697082093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p549717496093533">

BackEaseOut (int16_t startPos, int16_t endPos, uint16_t curTime,
uint16_t durationTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p741740474093533">

static int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p833695393093533">

Eases out with an overshoot.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row942741922093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p534371203093533">

BackEaseInOut (int16_t startPos, int16_t endPos, uint16_t curTime,
uint16_t durationTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1112901168093533">

static int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1799190930093533">

Eases in and then out with an overshoot.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row774523206093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p467081677093533">

CircEaseIn (int16_t startPos, int16_t endPos, uint16_t curTime, uint16_t
durationTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p496789381093533">

static int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1874975606093533">

Eases in shaping like a circular curve.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1021254518093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1982570402093533">

CircEaseOut (int16_t startPos, int16_t endPos, uint16_t curTime,
uint16_t durationTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2046459365093533">

static int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2048142985093533">

Eases out shaping like a circular curve.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1727523982093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1755638171093533">

CircEaseInOut (int16_t startPos, int16_t endPos, uint16_t curTime,
uint16_t durationTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p448185095093533">

static int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p171176698093533">

Eases in and then out shaping like a circular curve.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1871257105093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1784747575093533">

CubicEaseIn (int16_t startPos, int16_t endPos, uint16_t curTime,
uint16_t durationTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1204757406093533">

static int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p609416028093533">

Eases in shaping like a cubic curve.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1386508581093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1981189917093533">

CubicEaseOut (int16_t startPos, int16_t endPos, uint16_t curTime,
uint16_t durationTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1646317608093533">

static int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1683034723093533">

Eases out shaping like a cubic curve.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row435766193093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p530102783093533">

CubicEaseInOut (int16_t startPos, int16_t endPos, uint16_t curTime,
uint16_t durationTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1991775330093533">

static int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2069513610093533">

Eases in and then out shaping like a cubic curve.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row645313754093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p829946937093533">

LinearEaseNone (int16_t startPos, int16_t endPos, uint16_t curTime,
uint16_t durationTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p582746442093533">

static int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1952031933093533">

Displays no linear easing effects.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row989246393093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p570709307093533">

QuadEaseIn (int16_t startPos, int16_t endPos, uint16_t curTime, uint16_t
durationTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p298303116093533">

static int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p558262387093533">

Eases in shaping like a quadratic curve.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1032865340093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p412189524093533">

QuadEaseOut (int16_t startPos, int16_t endPos, uint16_t curTime,
uint16_t durationTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1452577025093533">

static int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1892708567093533">

Eases out shaping like a quadratic curve.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row847933444093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1930100882093533">

QuadEaseInOut (int16_t startPos, int16_t endPos, uint16_t curTime,
uint16_t durationTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p420090946093533">

static int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p435408388093533">

Eases in and then out shaping like a quadratic curve.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1461737789093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1494433378093533">

QuintEaseIn (int16_t startPos, int16_t endPos, uint16_t curTime,
uint16_t durationTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1152170870093533">

static int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p713319109093533">

Eases in shaping like a quintic curve.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1776786608093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p238399955093533">

QuintEaseOut (int16_t startPos, int16_t endPos, uint16_t curTime,
uint16_t durationTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1829590545093533">

static int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p601659680093533">

Eases out shaping like a quintic curve.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1189723147093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p980334108093533">

QuintEaseInOut (int16_t startPos, int16_t endPos, uint16_t curTime,
uint16_t durationTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p927303082093533">

static int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1794618440093533">

Eases in and then out shaping like a quintic curve.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2034493118093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p485100019093533">

SineEaseIn (int16_t startPos, int16_t endPos, uint16_t curTime, uint16_t
durationTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p395411423093533">

static int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1737802756093533">

Eases in shaping like a sinusoidal curve.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row607443015093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1030121554093533">

SineEaseOut (int16_t startPos, int16_t endPos, uint16_t curTime,
uint16_t durationTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p764805566093533">

static int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p806772214093533">

Eases out shaping like a sinusoidal curve.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row849106029093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1936727108093533">

SineEaseInOut (int16_t startPos, int16_t endPos, uint16_t curTime,
uint16_t durationTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1575999461093533">

static int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2129678497093533">

Eases in and then out shaping like a sinusoidal curve.

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

Additional Inherited Members
----------------------------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1276867051093533">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1062985684093533">

Additional Inherited Member Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1899048598093533">

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

   <tr id="row446105983093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1563445849093533">

operator new (size_t size)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1052944979093533">

Overrides the new function.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1749025114093533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p670367464093533">

operator delete (void \*p)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1837644458093533">

Overrides the delete function.

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
