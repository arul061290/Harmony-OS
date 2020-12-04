Development Guidelines on Photographing
=======================================

When to Use
-----------

Use the camera module APIs to capture frames (photographing).

Available APIs
--------------

**Table 1** APIs for photographing

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row4903852104914">

.. raw:: html

   <th class="cellrowborder" valign="top" width="18.811881188118814%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p2903252174918">

Class

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="46.534653465346544%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p1595113912507">

Function

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="34.65346534653466%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p15951597508">

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

   <tr id="row492815717494">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1592812716495">

CameraKit

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1492837144919">

int32_t GetCameraIds(std::list<string> cameraList)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2092807134919">

Obtains IDs of cameras that are currently available.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row11928157114912">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p139287774911">

CameraKit

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p9928107174915">

CameraAbility& GetCameraAbility(string cameraId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p139281171494">

Obtains the camera capability

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row119282719496">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p159288734914">

CameraKit

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p99280794913">

void RegisterCameraDeviceCallback(CameraDeviceCallback\* callback,
EventHandler\* handler)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p8928197134910">

Registers a camera callback for camera status changes.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row4928673496">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p14928770497">

CameraKit

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p14928197194915">

void UnregisterCameraDeviceCallback(CameraDeviceCallback\* callback)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p17929197134913">

Unregisters a camera callback.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row16929187104912">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p6929157184911">

CameraKit

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1192910704914">

void CreateCamera(string cameraId, CameraStateCallback\* callback,
EventHandler\* handler)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p12929167154912">

Creates a Camera instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row592967184912">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p9929127134915">

Camera

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p0929107204913">

string GetCameraId()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1592914710490">

Obtains the camera ID.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row13929197104913">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p16929167134913">

Camera

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p15929175491">

CameraConfig& GetCameraConfig()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p19298714917">

Obtains the camera configuration.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1892918764915">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p69291072495">

Camera

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p5930172494">

FrameConfig& GetFrameConfig(int32_t type)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p19301176495">

Obtains the frame configuration.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row893019794915">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p893016714919">

Camera

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1093067134915">

void Configure(CameraConfig& config)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1493037114912">

Configures the camera using the CameraConfig object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row11930197174917">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p4930197184914">

Camera

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p19304717492">

void Release()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p189301479494">

Releases the Camera object and associated resources.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row109304717499">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p4930873496">

Camera

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1893017720490">

int TriggerLoopingCapture(FrameConfig& frameConfig)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p149307754918">

Starts looping-frame capture.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row19306794915">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p6930167194910">

Camera

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p139311577499">

void StopLoopingCapture()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p693115764914">

Stops looping-frame capture.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row593116713492">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1193187174913">

Camera

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1493111713496">

int32_t TriggerSingleCapture(FrameConfig& frameConfig)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1193137104919">

Starts single-frame capture.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1693112711491">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p89312716494">

CameraConfig

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p199312784912">

void SetFrameStateCallback(FrameStateCallback\* callback, EventHandler\*
handler);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p49312714495">

Sets a frame state callback to respond to state changes.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row9931076492">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p59317784917">

CameraConfig

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p17931197124912">

static CameraConfig\* CreateCameraConfig()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p5931177164912">

Creates a CameraConfig instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row29321744917">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1093219716492">

CameraAbility

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p12932979493">

std::list<Size> GetSupportedSizes(int format)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1493210764918">

Obtains the supported image sizes for a specified image format.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1193267184910">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1393214717492">

CameraAbility

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p119321477495">

std::list<T> GetParameterRange(uint32_t key)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p139331079491">

Obtains the parameter value range based on a specified parameter key.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row0933197134920">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1493310764917">

CameraDevice

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p493313724915">

CameraDeviceCallback()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p993416724915">

A constructor used to create a CameraDeviceCallback instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row093418712498">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p159341779492">

CameraDevice

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1493411774912">

void OnCameraStatus​(std::string cameraId, int32_t status)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1393419715491">

Called when the camera device status changes.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row109348711497">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p993419724914">

CameraStateCallback

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p993418720497">

CameraStateCallback​()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p693511794919">

A constructor used to create a CameraStateCallback instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row159358717497">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1992012253527">

CameraStateCallback

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p29351077497">

void OnConfigured​(Camera& camera)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p093515774914">

Called when the camera is configured.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row9935147184918">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p117291328135211">

CameraStateCallback

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p19935174496">

void OnConfigureFailed​(Camera& camera,int32_t errorCode)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p159352077495">

Called when the camera fails to be configured.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1935279498">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1514619311525">

CameraStateCallback

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p493512744915">

void OnCreated​(Camera& camera)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1493511784914">

Called when the camera is successfully created.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row189351877493">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p172071933175218">

CameraStateCallback

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p129361977498">

void OnCreateFailed​(std::string cameraId,int32_t errorCode)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2936197114919">

Called when the camera fails to be created.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row20936472491">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p61213391523">

CameraStateCallback

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p793697174919">

void OnReleased​(Camera& camera)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p49361719495">

Called when the camera is released.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row159361179493">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p10936147194918">

FrameStateCallback

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p9936279496">

FrameStateCallback​()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p49367718499">

A constructor used to create a FrameStateCallback instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1893617744916">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p136968511524">

FrameStateCallback

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p209379744911">

void OnFrameFinished(Camera& camera, FrameConfig& frameConfig,
FrameResult& frameResult)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p19374724913">

Called when the frame capture is completed.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row093719718495">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p772975317527">

FrameStateCallback

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p189371471498">

void OnFrameError​(Camera& camera, FrameConfig& frameConfig, int32_t
errorCode, FrameResult& frameResult)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p109371778497">

Called when the frame capture fails.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row179381979499">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p169381975499">

FrameConfig

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1793867124910">

int32_t GetFrameConfigType()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1993817744915">

Obtains the frame configuration type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row793817784912">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p69381724914">

FrameConfig

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p149382077496">

std::list<OHOS::Surface> GetSurfaces()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p893867114919">

Obtains a list of surface objects (shared memories).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row109401570498">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p294019712492">

FrameConfig

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p19940170499">

void AddSurface(OHOS::AGP::UISurface& surface);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p11940197144915">

Adds a surface.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row994018711492">

.. raw:: html

   <td class="cellrowborder" valign="top" width="18.811881188118814%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1094016718493">

FrameConfig

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="46.534653465346544%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p139411279498">

void RemoveSurface(OHOS::AGP::UISurface& surface);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.65346534653466%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p39415717494">

Removes a surface.

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

Limitations and Constraints
---------------------------

None

How to Develop
--------------

1. Extend the **CameraDeviceCallback** class and call **OnCameraStatus**
   to customize operations when the camera device changes, for example,
   when a camera becomes available or unavailable.

   ::

      class SampleCameraDeviceCallback : public CameraDeviceCallback {
          void OnCameraStatus(std::string cameraId, int32_t status) override
          {
              // Do something when camera is available or unavailable.
          }
      };

2. Extend the **FrameStateCallback** class. After obtaining the frame
   data, save the data as a file.

   ::

      static void SampleSaveCapture(const char *p, uint32_t size)
      {
          cout << "Start saving picture" << endl;
          struct timeval tv;
          gettimeofday(&tv, NULL);
          struct tm *ltm = localtime(&tv.tv_sec);
          if (ltm != nullptr) {
              ostringstream ss("Capture_");
              ss << "Capture" << ltm->tm_hour << "-" << ltm->tm_min << "-" << ltm->tm_sec << ".jpg";

              ofstream pic("/sdcard/" + ss.str(), ofstream::out | ofstream::trunc);
              cout << "write " << size << " bytes" << endl;
              pic.write(p, size);
              cout << "Saving picture end" << endl;
          }
      }

      class TestFrameStateCallback : public FrameStateCallback {
          void OnFrameFinished(Camera &camera, FrameConfig &fc, FrameResult &result) override
          {
              cout << "Receive frame complete inform." << endl;
              if (fc.GetFrameConfigType() == FRAME_CONFIG_CAPTURE) {
                  cout << "Capture frame received." << endl;
                  list<Surface *> surfaceList = fc.GetSurfaces();
                  for (Surface *surface : surfaceList) {
                      SurfaceBuffer *buffer = surface->AcquireBuffer();
                      if (buffer != nullptr) {
                          char *virtAddr = static_cast<char *>(buffer->GetVirAddr());
                          if (virtAddr != nullptr) {
                              SampleSaveCapture(virtAddr, buffer->GetSize());
                          }
                          surface->ReleaseBuffer(buffer);
                      }
                      delete surface;
                  }
                  delete &fc;
              }
          }
      };

3. Extend the **CameraStateCallback** class and customize operations
   when the camera state changes (configuration successful or failed,
   and creation successful or failed).

   ::

      class SampleCameraStateMng : public CameraStateCallback {
      public:
          SampleCameraStateMng() = delete;
          SampleCameraStateMng(EventHandler &eventHdlr) : eventHdlr_(eventHdlr) {}
          ~SampleCameraStateMng()
          {
              if (recordFd_ != -1) {
                  close(recordFd_);
              }
          }
          void OnCreated(Camera &c) override
          {
              cout << "Sample recv OnCreate camera." << endl;
              auto config = CameraConfig::CreateCameraConfig();
              config->SetFrameStateCallback(&fsCb_, &eventHdlr_);
              c.Configure(*config);
              cam_ = &c;
          }
          void OnCreateFailed(const std::string cameraId, int32_t errorCode) override {}
          void OnReleased(Camera &c) override {}
      };

4. Create a **CameraKit** instance to set and obtain camera information.

   ::

      CameraKit *camKit = CameraKit::GetInstance();
      list<string> camList = camKit->GetCameraIds();
      string camId;
      for (auto &cam : camList) {
          cout << "camera name:" << cam << endl;
          const CameraAbility *ability = camKit->GetCameraAbility(cam);
          /* Find the camera that fits your ability. */
          list<CameraPicSize> sizeList = ability->GetSupportedSizes(0);
          if (find(sizeList.begin(), sizeList.end(), CAM_PIC_1080P) != sizeList.end()) {
              camId = cam;
              break;
          }
      }

5. Create a **Camera** instance.

   ::

      EventHandler eventHdlr; // Create a thread to handle callback events.
      SampleCameraStateMng CamStateMng(eventHdlr);

      camKit->CreateCamera(camId, CamStateMng, eventHdlr);

6. In the main process, synchronize configurations set by callback
   functions implemented in `step 1 <#li378084192111>`__, `step
   2 <#li8716104682913>`__, and `step 3 <#li6671035102514>`__.

   ::

      void OnCreated(Camera &c) override
      {
          cout << "Sample recv OnCreate camera." << endl;
          auto config = CameraConfig::CreateCameraConfig();
          config->SetFrameStateCallback(&fsCb_, &eventHdlr_);
          c.Configure(*config);
          cam_ = &c;
      }

      void Capture()
      {
          if (cam_ == nullptr) {
              cout << "Camera is not ready." << endl;
              return;
          }
          FrameConfig *fc = new FrameConfig(FRAME_CONFIG_CAPTURE);
          Surface *surface = Surface::CreateSurface();
          if (surface == nullptr) {
              delete fc;
          }
          surface->SetWidthAndHeight(1920, 1080); /* 1920:width,1080:height */
          fc->AddSurface(*surface);
          cam_->TriggerSingleCapture(*fc);
      }
