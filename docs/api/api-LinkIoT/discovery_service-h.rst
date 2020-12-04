discovery_service.h
===================

**Overview**\ 
--------------

**Related Modules:**

`Softbus <softbus.md>`__

**Description:**

Declares unified device service publishing interfaces.

This file provides capabilities related to device service publishing,
including publishing services, unpublishing services, and setting device
parameters. After multiple nearby devices are discovered and networked,
these interfaces can be used to perform service publishing-related
operations.

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

   <tr id="row907744138090253">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1977245706090253">

Data Structure Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p674994225090253">

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

   <tr id="row773743802090253">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1868199937090253">

PublishInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p505311872090253">

Defines service provisioning information sent to a discovering device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2009657402090253">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2081744149090253">

CapabilityMap

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1062287069090253">

Defines the mapping between supported capabilities and bitmaps.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1145479363090253">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p607076055090253">

DeviceMap

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p306102614090253">

Defines the mappings between the device type enumerations and device
type names.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1827597504090253">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p329295987090253">

IPublishCallback

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1390193299090253">

Defines the callbacks for successful and failed service publishing.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1380029524090253">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1783813532090253">

CommonDeviceInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1238567183090253">

Defines the type and content of a device to set.

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

   <tr id="row1297238380090253">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p660569662090253">

Typedef Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p986399404090253">

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

   <tr id="row143389890090253">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1158371923090253">

PublishInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1000368490090253">

typedef struct PublishInfo

.. raw:: html

   </p>

.. raw:: html

   <p id="p162031656090253">

Defines service provisioning information sent to a discovering device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row168471488090253">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1456119219090253">

DeviceType

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2146456532090253">

typedef enum DeviceTypeEnum

.. raw:: html

   </p>

.. raw:: html

   <p id="p11239047090253">

Enumerates device types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2058637896090253">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1722871345090253">

IPublishCallback

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p764741101090253">

typedef struct IPublishCallback

.. raw:: html

   </p>

.. raw:: html

   <p id="p1539713823090253">

Defines the callbacks for successful and failed service publishing.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1475899461090253">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1016434066090253">

CommonDeviceInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p764160030090253">

typedef struct CommonDeviceInfo

.. raw:: html

   </p>

.. raw:: html

   <p id="p1028410221090253">

Defines the type and content of a device to set.

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

   <tr id="row1886292022090253">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p42210489090253">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1551695649090253">

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

   <tr id="row573379789090253">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p522457574090253">

ExchanageMedium { AUTO = 0, BLE = 1, COAP = 2, USB = 3 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p645407247090253">

Enumerates media, such as Bluetooth, Wi-Fi, and USB, used for publishing
services.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row202308569090253">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p236723361090253">

ExchangeFre { LOW = 0, MID = 1, HIGH = 2, SUPER_HIGH = 3 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1679419102090253">

Enumerates frequencies for publishing services. This enumeration is
involved only in Bluetooth and is not supported currently.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1675518825090253">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p551680741090253">

DiscoverMode { DISCOVER_MODE_PASSIVE = 0x55, DISCOVER_MODE_ACTIVE = 0xAA
}

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p908450638090253">

Enumerates the modes in which services are published. The publishing
service supports the passive mode. Lite devices support the passive mode
only.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1759950538090253">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1001982808090253">

PublishFailReason { PUBLISH_FAIL_REASON_NOT_SUPPORT_MEDIUM = 1,
PUBLISH_FAIL_REASON_PARAMETER_INVALID = 2, PUBLISH_FAIL_REASON_UNKNOWN =
0xFF }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p698021068090253">

Enumerates failure reasons for publishing services.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1692775405090253">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1527768056090253">

DataBitMap { HICALL_CAPABILITY_BITMAP = 0, PROFILE_CAPABILITY_BITMAP =
1, HOMEVISIONPIC_CAPABILITY_BITMAP = 2, CASTPLUS_CAPABILITY_BITMAP,
AA_CAPABILITY_BITMAP, DVKIT_CAPABILITY_BITMAP, DDMP_CAPABILITY_BITMAP }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1604333221090253">

Enumerates supported capabilities published by a device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row439418683090253">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2000678037090253">

DeviceTypeEnum { UNKOWN = 0x00, PHONE = 0x0E, PAD = 0x11, TV = 0x9C, PC
= 0x0C, AUDIO = 0x0A, CAR = 0x83, L0 = 0xF1, L1 = 0xF2 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1798466826090253">

Enumerates device types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2126160349090253">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1402410320090253">

CommonDeviceKey { COMM_DEVICE_KEY_DEVID = 0, COMM_DEVICE_KEY_DEVTYPE =
1, COMM_DEVICE_KEY_DEVNAME = 2, COMM_DEVICE_KEY_MAX }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p783396070090253">

Enumerates device information, such as its ID, type, and name.

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

   <tr id="row1969072315090253">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p59022275090253">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1430344193090253">

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

   <tr id="row1762120235090253">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p539797665090253">

PublishService (const char *moduleName, const struct PublishInfo*\ info,
const struct IPublishCallback \*cb)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p849549818090253">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p654805535090253">

Publishes a service to the discovering device in the LAN.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row410402513090253">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1906723982090253">

UnPublishService (const char \*moduleName, int publishId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1055214080090253">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p900719817090253">

Unpublishes a service based on the publicId and moduleName.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row799413974090253">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p858928627090253">

SetCommonDeviceInfo (const struct CommonDeviceInfo \*devInfo, unsigned
int num)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p493724513090253">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p264921489090253">

Sets common device information, such as its ID, type, and name.

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
