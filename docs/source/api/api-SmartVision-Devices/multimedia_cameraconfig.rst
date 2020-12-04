MultiMedia_CameraConfig
=======================

**Overview**\ 
--------------

Defines the **CameraConfig** class for operations on camera
configurations.

**Since:**

1.0

**Version:**

1.0

**Summary**\ 
-------------

Files
-----

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1226836154084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p267224960084827">

File Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p22340430084827">

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

   <tr id="row1310624425084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1072440167084827">

camera_config.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p27621879084827">

Declares functions in the CameraConfig class.

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

Data Structures
---------------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1604257412084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1387809056084827">

Data Structure Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2098853569084827">

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

   <tr id="row773803074084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p870179372084827">

OHOS::Media::CameraConfig

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1651535233084827">

Provides functions to configure camera parameters.

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

   <tr id="row158537118084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1625645276084827">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p477934866084827">

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

   <tr id="row925804857084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1065902135084827">

OHOS::Media::CameraConfig::~CameraConfig ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p16776385084827">

virtual

.. raw:: html

   </p>

.. raw:: html

   <p id="p1467157836084827">

A destructor used to delete the CameraAbility instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1577641454084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p584734280084827">

OHOS::Media::CameraConfig::CreateCameraConfig ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1847989033084827">

static CameraConfig \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p561520279084827">

Creates the CameraConfig instance of this singleton class to configure
and read the required parameters.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1156821085084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1288373410084827">

OHOS::Media::CameraConfig::SetFrameStateCallback (FrameStateCallback
*callback, EventHandler*\ handler)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1492603334084827">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1811954312084827">

Sets a frame state callback to responds to state changes.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row782651004084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1444855945084827">

OHOS::Media::CameraConfig::GetEventHandler () const

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1090826937084827">

virtual EventHandler \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p982317400084827">

Obtains the EventHandler object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row909311608084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p31463626084827">

OHOS::Media::CameraConfig::GetFrameStateCb () const

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1510514141084827">

virtual FrameStateCallback \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1595165756084827">

Obtains a FrameStateCallback object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1835173130084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1459313853084827">

OHOS::Media::CameraConfig::CameraConfig ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p436664204084827">

.. raw:: html

   </p>

.. raw:: html

   <p id="p2027514996084827">

A constructor used to create a CameraConfig instance.

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

**Function Documentation**\ 
----------------------------

CameraConfig()
--------------

::

   OHOS::Media::CameraConfig::CameraConfig ()

**Description:**

A constructor used to create a
`CameraConfig <ohos-media-cameraconfig.md>`__ instance.

CreateCameraConfig()
--------------------

::

   static [CameraConfig](ohos-media-cameraconfig.md)* OHOS::Media::CameraConfig::CreateCameraConfig ()

**Description:**

Creates the `CameraConfig <ohos-media-cameraconfig.md>`__ instance of
this singleton class to configure and read the required parameters.

**Returns:**

Returns the `CameraConfig <ohos-media-cameraconfig.md>`__ instance if
created; returns **NULL** otherwise.

GetEventHandler()
-----------------

::

   virtual EventHandler* OHOS::Media::CameraConfig::GetEventHandler () const

**Description:**

Obtains the **EventHandler** object.

**Returns:**

Returns the pointer to the **EventHandler** object if obtained; returns
**NULL** otherwise.

GetFrameStateCb()
-----------------

::

   virtual [FrameStateCallback](ohos-media-framestatecallback.md)* OHOS::Media::CameraConfig::GetFrameStateCb () const

**Description:**

Obtains a `FrameStateCallback <ohos-media-framestatecallback.md>`__
object.

**Returns:**

Returns the pointer to the
`FrameStateCallback <ohos-media-framestatecallback.md>`__ object if
obtained; returns **NULL** otherwise.

SetFrameStateCallback()
-----------------------

::

   virtual void OHOS::Media::CameraConfig::SetFrameStateCallback ([FrameStateCallback](ohos-media-framestatecallback.md) * callback, EventHandler * handler )

**Description:**

Sets a frame state callback to responds to state changes.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row721560332084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1944190132084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1911600946084827">

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

   <tr id="row894139932084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

callback

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the frame state callback.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1840249745084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handler

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the event handler.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

.. _cameraconfig-1:

~CameraConfig()
---------------

::

   virtual OHOS::Media::CameraConfig::~CameraConfig ()

**Description:**

A destructor used to delete the
`CameraAbility <ohos-media-cameraability.md>`__ instance.
