LayerFuncs
==========

**Overview**\ 
--------------

**Related Modules:**

`Display <display.md>`__

**Description:**

Defines pointers to the layer driver functions.

**Summary**\ 
-------------

Data Fields
-----------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1801789020093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p580584264093531">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1447025685093531">

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

   <tr id="row1290209619093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1761511737093531">

InitDisplay )(uint32_t devId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p854108477093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p858279981093531">

Initializes a display device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row705927014093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1325594315093531">

DeinitDisplay )(uint32_t devId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p642152892093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1941568498093531">

Deinitializes a display device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1375052931093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1619603363093531">

GetDisplayInfo )(uint32_t devId, DisplayInfo \*dispInfo)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p969801017093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p571383769093531">

Obtains information about a display device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row657199072093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p529170825093531">

OpenLayer )(uint32_t devId, const LayerInfo *layerInfo,
uint32_t*\ layerId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2115517563093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1321274281093531">

Opens a layer on a specified display device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row484321565093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1003638687093531">

CloseLayer )(uint32_t devId, uint32_t layerId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p308821775093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1426803714093531">

Closes a layer that is no longer required on a specified display device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1101309460093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1712191943093531">

SetLayerVisible )(uint32_t devId, uint32_t layerId, bool visible)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p363999925093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p709852316093531">

Sets whether a layer is visible.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row944841608093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1689743827093531">

GetLayerVisibleState )(uint32_t devId, uint32_t layerId, bool \*visible)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p291167239093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1074825475093531">

Checks whether a layer is visible.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row57270837093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p790845491093531">

SetLayerSize )(uint32_t devId, uint32_t layerId, IRect \*rect)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1090797462093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1773045931093531">

Sets the size of a layer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1511842937093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p311479173093531">

GetLayerSize )(uint32_t devId, uint32_t layerId, IRect \*rect)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1709282148093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p185929585093531">

Obtains the size of a layer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1204712439093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p88960164093531">

SetLayerCrop )(uint32_t devId, uint32_t layerId, IRect \*rect)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2074544270093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p193713054093531">

Sets the rectangular area to crop for a layer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row4319023093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1777642484093531">

SetLayerZorder )(uint32_t devId, uint32_t layerId, uint32_t zorder)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p184143524093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1181114921093531">

Sets the z-order for a layer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1874075351093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p486334247093531">

GetLayerZorder )(uint32_t devId, uint32_t layerId, uint32_t \*zorder)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p271904733093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1476215370093531">

Obtains the z-order of a layer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1847792393093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p695525281093531">

SetLayerPreMulti )(uint32_t devId, uint32_t layerId, bool preMul)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p759922950093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p267696715093531">

Sets layer premultiplication.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row194655880093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1845156226093531">

GetLayerPreMulti )(uint32_t devId, uint32_t layerId, bool \*preMul)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1003022766093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p927666764093531">

Obtains the premultiplication flag of a layer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row400547406093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p265279476093531">

SetLayerAlpha )(uint32_t devId, uint32_t layerid, LayerAlpha \*alpha)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1439542188093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1019388064093531">

Sets the alpha value for a layer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1294561651093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p721242077093531">

GetLayerAlpha )(uint32_t devId, uint32_t layerId, LayerAlpha \*alpha)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1979044114093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p910903822093531">

Obtains the alpha value of a layer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1184821856093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p601005063093531">

SetLayerColorKey )(uint32_t devId, uint32_t layerId, bool enable,
uint32_t key)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p155517740093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1736270720093531">

Sets the color key for a layer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1888941624093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1748335140093531">

GetLayerColorKey )(uint32_t devId, uint32_t layerId, bool *enable,
uint32_t*\ key)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2140044781093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p927857568093531">

Obtains the color key of a layer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1901687058093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1699717131093531">

SetLayerPalette )(uint32_t devId, uint32_t layerId, uint32_t \*palette,
uint32_t len)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p13040619093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p450376859093531">

Sets the palette for a layer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1761515508093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p695796286093531">

GetLayerPalette )(uint32_t devId, uint32_t layerId, uint32_t \*palette,
uint32_t len)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1420431936093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p329947031093531">

Obtains the palette of a layer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1382141007093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2050664918093531">

SetTransformMode )(uint32_t devId, uint32_t layerId, TransformType type)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p70591593093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p977437106093531">

Sets the transform mode for a layer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row977558620093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p295434907093531">

SetLayerCompression )(uint32_t devId, uint32_t layerId, int32_t
compType)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1158110644093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1485653205093531">

Sets the compression feature for a layer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row290541066093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p138006922093531">

GetLayerCompression )(uint32_t devId, uint32_t layerId, int32_t
\*compType)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1246865172093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p2090539520093531">

Checks whether the compression feature is enabled for a layer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1975661216093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p903415271093531">

SetLayerDirtyRegion )(uint32_t devId, uint32_t layerId, IRect \*region)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p66636054093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1065423353093531">

Sets the flushing area for a layer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1724532702093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p574167614093531">

GetLayerBuffer )(uint32_t devId, uint32_t layerId, LayerBuffer \*buffer)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2089235664093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1211231736093531">

Obtains the buffer of a layer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1347494713093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1849440551093531">

Flush )(uint32_t devId, uint32_t layerId, LayerBuffer \*buffer)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p262609741093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p2038692562093531">

Flushes a layer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1337367313093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2102945464093531">

WaitForVBlank )(uint32_t devId, uint32_t layerId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1248161901093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1129923339093531">

Waits for the arrival of vertical blanking.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1961747558093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p468466593093531">

SnapShot )(uint32_t devId, LayerBuffer \*buffer)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p527839475093531">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p294871108093531">

Implements the snapshot feature.

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

**Field Documentation**\ 
-------------------------

CloseLayer
----------

::

   int32_t(* LayerFuncs::CloseLayer) (uint32_t devId, uint32_t layerId)

**Description:**

Closes a layer that is no longer required on a specified display device.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1326945359093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p395676765093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2109815906093531">

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

   <tr id="row120617066093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row388381540093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`OpenLayer <layerfuncs.md#a795f4e168d5b284a9c33f636c278207f>`__

DeinitDisplay
-------------

::

   int32_t(* LayerFuncs::DeinitDisplay) (uint32_t devId)

**Description:**

Deinitializes a display device.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row758924228093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1798225751093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p602934640093531">

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

   <tr id="row417296870093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`InitDisplay <layerfuncs.md#a0641c3b48542646daa80386122bed46a>`__

Flush
-----

::

   int32_t(* LayerFuncs::Flush) (uint32_t devId, uint32_t layerId, [LayerBuffer](layerbuffer.md) *buffer)

**Description:**

Flushes a layer.

Display data in the buffer is flushed to a specified layer so that the
image data is displayed on the screen.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row675629429093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p54443304093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1361074167093531">

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

   <tr id="row1108364237093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row194761284093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row873215645093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

buffer

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the buffer in which the display data is to
flush.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

GetDisplayInfo
--------------

::

   int32_t(* LayerFuncs::GetDisplayInfo) (uint32_t devId, [DisplayInfo](displayinfo.md) *dispInfo)

**Description:**

Obtains information about a display device.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1252037398093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1708419097093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p102499992093531">

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

   <tr id="row1053371586093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row408036878093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

dispInfo

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the display device information obtained.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

GetLayerAlpha
-------------

::

   int32_t(* LayerFuncs::GetLayerAlpha) (uint32_t devId, uint32_t layerId, [LayerAlpha](layeralpha.md) *alpha)

**Description:**

Obtains the alpha value of a layer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1869068225093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1225363482093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1626018140093531">

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

   <tr id="row1828275366093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row130095139093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1321886392093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

alpha

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the obtained alpha value.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`SetLayerAlpha <layerfuncs.md#a20e554afa2f7b1015fd23ce240344b13>`__

GetLayerBuffer
--------------

::

   int32_t(* LayerFuncs::GetLayerBuffer) (uint32_t devId, uint32_t layerId, [LayerBuffer](layerbuffer.md) *buffer)

**Description:**

Obtains the buffer of a layer.

After drawing a picture in the buffer, the application calls the
`Flush <layerfuncs.md#abb480bf2b85e93841c49fdc9800bd1e7>`__ function to
display the picture on the screen.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1085262865093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p944703234093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p482414576093531">

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

   <tr id="row1858301275093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2006096958093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1375174231093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

buffer

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the obtained buffer.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`Flush <layerfuncs.md#abb480bf2b85e93841c49fdc9800bd1e7>`__

GetLayerColorKey
----------------

::

   int32_t(* LayerFuncs::GetLayerColorKey) (uint32_t devId, uint32_t layerId, bool *enable, uint32_t *key)

**Description:**

Obtains the color key of a layer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row81899739093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p830941648093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2110619386093531">

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

   <tr id="row206914393093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row532574434093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1828372537093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

enable

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the color key enable bit.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row761109968093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

key

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the color key.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`SetLayerColorKey <layerfuncs.md#a5701fe1e0e2414de577aa5329bd873c9>`__

GetLayerCompression
-------------------

::

   int32_t(* LayerFuncs::GetLayerCompression) (uint32_t devId, uint32_t layerId, int32_t *compType)

**Description:**

Checks whether the compression feature is enabled for a layer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1959725322093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1279781375093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p895211156093531">

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

   <tr id="row342222990093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1022257881093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1171134176093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

compType

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the variable specifying whether the compression
feature is enabled.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`SetLayerCompression <layerfuncs.md#a46c9750d8615dc874b66ac4b10796b24>`__

GetLayerPalette
---------------

::

   int32_t(* LayerFuncs::GetLayerPalette) (uint32_t devId, uint32_t layerId, uint32_t *palette, uint32_t len)

**Description:**

Obtains the palette of a layer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1576036959093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p899160420093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2039609593093531">

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

   <tr id="row865245955093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1674406385093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1626074369093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

palette

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the obtained palette.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1010174164093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

len

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the length of the palette.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`SetLayerPalette <layerfuncs.md#a3982c76e093852ef386fc372581be4af>`__

GetLayerPreMulti
----------------

::

   int32_t(* LayerFuncs::GetLayerPreMulti) (uint32_t devId, uint32_t layerId, bool *preMul)

**Description:**

Obtains the premultiplication flag of a layer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1991316039093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1887410458093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p660237536093531">

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

   <tr id="row1030127948093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1770627252093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1729116278093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

preMul

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the obtained layer premultiplication flag.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`SetLayerPreMulti <layerfuncs.md#a456aa01ca3ffa81d2e49c0a9487f816f>`__

GetLayerSize
------------

::

   int32_t(* LayerFuncs::GetLayerSize) (uint32_t devId, uint32_t layerId, [IRect](irect.md) *rect)

**Description:**

Obtains the size of a layer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1179113461093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p929921090093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p509335603093531">

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

   <tr id="row1056608761093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1083453896093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row601771995093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

rect

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the obtained layer size.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`SetLayerSize <layerfuncs.md#ab58e66b0676b1baa1662c175d43bf219>`__

GetLayerVisibleState
--------------------

::

   int32_t(* LayerFuncs::GetLayerVisibleState) (uint32_t devId, uint32_t layerId, bool *visible)

**Description:**

Checks whether a layer is visible.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row179301628093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p61508176093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2078522371093531">

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

   <tr id="row924584418093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row892464969093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row421385068093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

visible

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the obtained layer visibility. The value true
indicates that the layer is visible, and false indicates that the layer
is invisible.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`SetLayerVisible <layerfuncs.md#aaa5bf7f98e8dc47510a4f26fb38094b6>`__

GetLayerZorder
--------------

::

   int32_t(* LayerFuncs::GetLayerZorder) (uint32_t devId, uint32_t layerId, uint32_t *zorder)

**Description:**

Obtains the z-order of a layer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1637367783093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1556493325093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p319004314093531">

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

   <tr id="row1710790864093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row310381938093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row105963335093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

zorder

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the obtained z-order. The value is an integer
ranging from 0 to 255. A larger z-order value indicates a higher layer.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`SetLayerZorder <layerfuncs.md#aa3803c2a6395651d1538ffb62d29733d>`__

InitDisplay
-----------

::

   int32_t(* LayerFuncs::InitDisplay) (uint32_t devId)

**Description:**

Initializes a display device.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row17384343093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p832253932093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2140304851093531">

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

   <tr id="row734618597093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`DeinitDisplay <layerfuncs.md#a8d7a715d7d2b4bd5ab0db92c2a1eec93>`__

OpenLayer
---------

::

   int32_t(* LayerFuncs::OpenLayer) (uint32_t devId, const [LayerInfo](layerinfo.md) *layerInfo, uint32_t *layerId)

**Description:**

Opens a layer on a specified display device.

Before using a layer on the GUI, you must open the layer based on the
layer information. After the layer is opened, you can obtain the layer
ID and then use other functions based on the layer ID.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row106611282093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p324761645093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p200308706093531">

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

   <tr id="row1405462089093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2584690093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerInfo

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the layer information passed to open a layer,
including the layer type, layer size, and pixel format.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row139559933093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the layer ID, which identifies a unique layer.
The layer ID is returned to the GUI after the layer is successfully
opened.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`CloseLayer <layerfuncs.md#a2e375f75209da329f131b914377e9616>`__

SetLayerAlpha
-------------

::

   int32_t(* LayerFuncs::SetLayerAlpha) (uint32_t devId, uint32_t layerid, [LayerAlpha](layeralpha.md) *alpha)

**Description:**

Sets the alpha value for a layer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1100759469093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1196420401093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1674907026093531">

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

   <tr id="row1833544359093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1757367915093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2025273889093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

alpha

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the alpha value to set.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`GetLayerAlpha <layerfuncs.md#acf1e01338eeb0fd957f53ed0d2551394>`__

SetLayerColorKey
----------------

::

   int32_t(* LayerFuncs::SetLayerColorKey) (uint32_t devId, uint32_t layerId, bool enable, uint32_t key)

**Description:**

Sets the color key for a layer.

The color key is used during layer overlay.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row988694115093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2041875825093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p175497064093531">

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

   <tr id="row860406182093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row162588810093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row508898727093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

enable

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Specify whether to enable the color key.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1728112134093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

key

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the color key.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`GetLayerColorKey <layerfuncs.md#aea882232b6279b8be82c45e889187b24>`__

SetLayerCompression
-------------------

::

   int32_t(* LayerFuncs::SetLayerCompression) (uint32_t devId, uint32_t layerId, int32_t compType)

**Description:**

Sets the compression feature for a layer.

In specific scenarios, images need to be compressed. You can set whether
to enable layer compression.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1529493241093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1406223806093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1821647985093531">

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

   <tr id="row69655650093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row864443729093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row632304956093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

compType

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Specifies whether to enable the compression feature. The value true>/b>
means to enable compression, and false> means the opposite.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

\***\* Returns **0** if the operation is successful; returns an error
code defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise. \***\*

**See also:**

\***\*
`GetLayerCompression <layerfuncs.md#ab0b5855ea4ee5228516303cba84907ce>`__
\***\*

SetLayerCrop
------------

::

   int32_t(* LayerFuncs::SetLayerCrop) (uint32_t devId, uint32_t layerId, [IRect](irect.md) *rect)

**Description:**

Sets the rectangular area to crop for a layer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row145522317093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p417430236093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1251325215093531">

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

   <tr id="row672930651093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1617062420093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row879691193093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

rect

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the rectangular area to crop.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

SetLayerDirtyRegion
-------------------

::

   int32_t(* LayerFuncs::SetLayerDirtyRegion) (uint32_t devId, uint32_t layerId, [IRect](irect.md) *region)

**Description:**

Sets the flushing area for a layer.

After the GUI draws an image, you must set the layer flushing area
before calling the
`Flush <layerfuncs.md#abb480bf2b85e93841c49fdc9800bd1e7>`__ function to
flush the screen.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2060333437093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2054333734093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1904335617093531">

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

   <tr id="row1636357435093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row290451342093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row7325443093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

region

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the flushing area to set.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

SetLayerPalette
---------------

::

   int32_t(* LayerFuncs::SetLayerPalette) (uint32_t devId, uint32_t layerId, uint32_t *palette, uint32_t len)

**Description:**

Sets the palette for a layer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1126292470093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p938597574093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p221293482093531">

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

   <tr id="row1704166952093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row653753729093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1400954845093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

palette

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the palette to set.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1705217419093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

len

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the length of the palette.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`GetLayerPalette <layerfuncs.md#af713bc39e51dc8168c278e2f126bf4e3>`__

SetLayerPreMulti
----------------

::

   int32_t(* LayerFuncs::SetLayerPreMulti) (uint32_t devId, uint32_t layerId, bool preMul)

**Description:**

Sets layer premultiplication.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2008335903093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2020796955093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p36368346093531">

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

   <tr id="row293165169093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1232136311093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row55797100093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

preMul

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Specifies whether to enable layer premultiplication. The value 1 means
to enable layer premultiplication, and 0 means the opposite.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`GetLayerPreMulti <layerfuncs.md#a4a0e26f8401da1232f03bb37502ff4bd>`__

SetLayerSize
------------

::

   int32_t(* LayerFuncs::SetLayerSize) (uint32_t devId, uint32_t layerId, [IRect](irect.md) *rect)

**Description:**

Sets the size of a layer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row480762880093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1315234625093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p806382432093531">

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

   <tr id="row1469557999093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row396094898093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1004138495093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

rect

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the layer size to set, in pixels.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`GetLayerSize <layerfuncs.md#a56be84be25eba64497b2a842c1f68b26>`__

SetLayerVisible
---------------

::

   int32_t(* LayerFuncs::SetLayerVisible) (uint32_t devId, uint32_t layerId, bool visible)

**Description:**

Sets whether a layer is visible.

A visible layer is displayed on the screen, whereas an invisible layer
is not displayed on the screen.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1820877154093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p447177618093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p603092946093531">

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

   <tr id="row1255658259093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2005245510093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row777897011093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

visible

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the visibility to set for the layer. The value true means to
set the layer to be visible, and false means the opposite.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`GetLayerVisibleState <layerfuncs.md#a6bbff71bb4f17eb84a4db4857a0b0985>`__

SetLayerZorder
--------------

::

   int32_t(* LayerFuncs::SetLayerZorder) (uint32_t devId, uint32_t layerId, uint32_t zorder)

**Description:**

Sets the z-order for a layer.

A larger z-order value indicates a higher layer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2131634649093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1946247641093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p725176743093531">

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

   <tr id="row792333034093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1252891266093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row606847427093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

zorder

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the z-order to set. The value is an integer ranging from 0 to
255.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

**See also:**

`GetLayerZorder <layerfuncs.md#a5644645442e1d6943b55ce0a6a801b8c>`__

SetTransformMode
----------------

::

   int32_t(* LayerFuncs::SetTransformMode) (uint32_t devId, uint32_t layerId, [TransformType](display.md#gaa65f3b21a9a92ff022e435a7304126d2) type)

**Description:**

Sets the transform mode for a layer.

Using this function, you can rotate, scale, and move the layer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1784814313093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p949541882093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1601894993093531">

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

   <tr id="row619059072093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row134464179093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row317716929093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

type

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the transformation mode to set.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

SnapShot
--------

::

   int32_t(* LayerFuncs::SnapShot) (uint32_t devId, [LayerBuffer](layerbuffer.md) *buffer)

**Description:**

Implements the snapshot feature.

This function saves the screenshot of image data on the display device
to the buffer for debugging or as requested by applications.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1618470585093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p818370175093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1883261800093531">

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

   <tr id="row1315996068093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row823216927093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

buffer

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the buffer for saving screenshots.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.

WaitForVBlank
-------------

::

   int32_t(* LayerFuncs::WaitForVBlank) (uint32_t devId, uint32_t layerId)

**Description:**

Waits for the arrival of vertical blanking.

This function blocks the process until vertical blanking arrives,
implementing the synchronization between software and hardware.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row533202272093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1570369132093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p6749341093531">

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

   <tr id="row712612358093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

devId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of a display device. The value ranges from 0 to 4,
where 0 indicates the first display device and 4 indicates the last
display device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1440376428093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

layerId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the layer ID, which identifies a unique layer. You can perform
operations on the layer with the specified layer ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row964608140093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

timeOut

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the maximum duration that the process waits for the arrival of
vertical blanking.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns an error code
defined in
`DispErrCode <display.md#ga12a925dadef7573cd74d63d06824f9b0>`__
otherwise.
