MultiMedia_Camera
=================

**Overview**\ 
--------------

Defines the **Camera** class for camera-related operations.

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

   <tr id="row556418638084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p439646740084827">

File Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1419641004084827">

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

   <tr id="row1195358678084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p386961104084827">

camera.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1970304108084827">

Declares functions in the Camera class to implement camera operations.

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

   <tr id="row1371850475084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1147925292084827">

Data Structure Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1853686083084827">

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

   <tr id="row558515897084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1905275131084827">

OHOS::Media::Camera

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p934468959084827">

Provides functions in the Camera class to implement camera operations.
operations.

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

   <tr id="row209230622084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p874604836084827">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1355810737084827">

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

   <tr id="row1628072791084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1736470196084827">

OHOS::Media::Camera::~Camera ()=default

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p218600620084827">

virtual

.. raw:: html

   </p>

.. raw:: html

   <p id="p640990420084827">

A destructor used to delete the Camera instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row724054503084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p645995091084827">

OHOS::Media::Camera::GetCameraId ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1462751851084827">

virtual std::string

.. raw:: html

   </p>

.. raw:: html

   <p id="p1918879995084827">

Obtains the camera ID.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1256935035084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1604180431084827">

OHOS::Media::Camera::GetCameraConfig () const

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p519118055084827">

virtual const CameraConfig \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p816403533084827">

Obtains the camera configuration. You can use the obtained CameraConfig
object to configure the camera.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row532846220084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1818245845084827">

OHOS::Media::Camera::GetFrameConfig (int32_t type)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p246791770084827">

virtual FrameConfig \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1657103706084827">

Obtains the frame configuration.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row891780585084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p354461499084827">

OHOS::Media::Camera::Configure (CameraConfig &config)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p853646593084827">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p4046432084827">

Configures the camera using the CameraConfig object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1303477917084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1002446667084827">

OHOS::Media::Camera::TriggerLoopingCapture (FrameConfig &frameConfig)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1704363650084827">

virtual int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p232411056084827">

Triggers looping-frame capture.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row34772695084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1026540319084827">

OHOS::Media::Camera::StopLoopingCapture ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p666626720084827">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1961259597084827">

Stops looping-frame capture.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1886153005084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1844442938084827">

OHOS::Media::Camera::TriggerSingleCapture (FrameConfig &frameConfig)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1456476069084827">

virtual int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2074319233084827">

Starts single-frame capture. The frame parameters are set through the
FrameConfig object, and the captured image data is stored in the surface
of the FrameConfig object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1672174510084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2072359526084827">

OHOS::Media::Camera::Release ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p425542048084827">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p90303236084827">

Releases the Camera object and associated resources.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row32036374084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p339246978084827">

OHOS::Media::Camera::Camera ()=default

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2010712204084827">

.. raw:: html

   </p>

.. raw:: html

   <p id="p421972722084827">

A constructor used to create a Camera instance.

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

Camera()
--------

::

   OHOS::Media::Camera::Camera ()

**Description:**

A constructor used to create a `Camera <ohos-media-camera.md>`__
instance.

Configure()
-----------

::

   virtual void OHOS::Media::Camera::Configure ([CameraConfig](ohos-media-cameraconfig.md) & config)

**Description:**

Configures the camera using the
`CameraConfig <ohos-media-cameraconfig.md>`__ object.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row350703700084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p602019674084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p242499538084827">

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

   <tr id="row1333502601084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

config

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the CameraConfig object.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

GetCameraConfig()
-----------------

::

   virtual const [CameraConfig](ohos-media-cameraconfig.md)* OHOS::Media::Camera::GetCameraConfig () const

**Description:**

Obtains the camera configuration. You can use the obtained
`CameraConfig <ohos-media-cameraconfig.md>`__ object to configure the
camera.

**Returns:**

Returns the pointer to the `CameraConfig <ohos-media-cameraconfig.md>`__
object if obtained; returns **NULL** otherwise.

GetCameraId()
-------------

::

   virtual std::string OHOS::Media::Camera::GetCameraId ()

**Description:**

Obtains the camera ID.

**Returns:**

Returns the camera ID if obtained; returns the “Error” string if the
camera fails to be created.

GetFrameConfig()
----------------

::

   virtual [FrameConfig](ohos-media-frameconfig.md)* OHOS::Media::Camera::GetFrameConfig (int32_t type)

**Description:**

Obtains the frame configuration.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1990731937084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p193687814084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1670727326084827">

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

   <tr id="row1389033079084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

type

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the type of the frame configuration.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the pointer to the `FrameConfig <ohos-media-frameconfig.md>`__
object if obtained; returns **NULL** otherwise.

Release()
---------

::

   virtual void OHOS::Media::Camera::Release ()

**Description:**

Releases the `Camera <ohos-media-camera.md>`__ object and associated
resources.

StopLoopingCapture()
--------------------

::

   virtual void OHOS::Media::Camera::StopLoopingCapture ()

**Description:**

Stops looping-frame capture.

**Returns:**

Returns **true** if the looping-frame capture is successfully stopped;
returns **false** otherwise.

TriggerLoopingCapture()
-----------------------

::

   virtual int32_t OHOS::Media::Camera::TriggerLoopingCapture ([FrameConfig](ohos-media-frameconfig.md) & frameConfig)

**Description:**

Triggers looping-frame capture.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1141631070084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1718951211084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1336002590084827">

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

   <tr id="row134835942084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

fc

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the frame configuration.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **true** if the looping-frame capture is successfully started;
returns **false** otherwise.

TriggerSingleCapture()
----------------------

::

   virtual int32_t OHOS::Media::Camera::TriggerSingleCapture ([FrameConfig](ohos-media-frameconfig.md) & frameConfig)

**Description:**

Starts single-frame capture. The frame parameters are set through the
`FrameConfig <ohos-media-frameconfig.md>`__ object, and the captured
image data is stored in the surface of the
`FrameConfig <ohos-media-frameconfig.md>`__ object.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row230903783084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p629992173084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p678279672084827">

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

   <tr id="row594595840084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

fc

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the frame configuration.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **true** if the single-frame capture is successfully started and
the data is stored; returns **false** otherwise.

.. _camera-1:

~Camera()
---------

::

   virtual OHOS::Media::Camera::~Camera ()

**Description:**

A destructor used to delete the `Camera <ohos-media-camera.md>`__
instance.
