Distributed Remote Startup
==========================

Overview
--------

The Distributed Manager Service sets up a distributed service platform
in OpenHarmony by using a proxy between the primary and secondary
devices. With the Distributed Manager Service, the primary device
(OpenHarmony-powered smart TV) can start a Feature Ability (FA) deployed
on the secondary device (a memory-constrained OpenHarmony device such as
an IP camera or a lite wearable).

For example, if a user presses the **Remind Me** button for a TV program
on the smart TV, the smart TV will start the corresponding reminder FA
on the lite wearable to remind the user when the particular TV program
is available.

Basic Concepts
--------------

-  FA

   Feature Ability, representing an ability with a UI for interacting
   with users

-  Remote startup

   Cross-device FA startup, which is the counterpart of local FA startup

Available APIs
--------------

The following table describes the API that can be used by smart TVs to
remotely start an FA. This API is provided in the **AbilitySlice**
class. For details, see the Java API reference for OpenHarmony
application development.

**Table 1** API for remotely starting an FA on the distributed network

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row4419501537">

.. raw:: html

   <th class="cellrowborder" valign="top" width="57.38999999999999%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p54150165315">

Method

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="42.61%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p941150145313">

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

   <tr id="row34145016535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="57.38999999999999%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1682733119213">

void startAbility(Want want)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="42.61%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p13562171015712">

Remotely starts an FA based on the specified Want information. If the
name and type of the want parameter are different from those used in the
integrated development environment (IDE), use the parameter name and
type in the IDE.

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

**Table 2** Description of the want parameter

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row172294315361">

.. raw:: html

   <th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p722144318360">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="17%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p10227434363">

Type

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="69%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p22284383616">

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

   <tr id="row3228436365">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1391227193713">

want

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p20993611193719">

ohos.aafwk.content.Want

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p10555172211377">

When you use startAbility(Want want) to remotely start an FA, you must
first specify the deviceId, bundleName, and abilityName attributes of
the target FA in the Want object.

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

-  The primary device can remotely start an FA of the secondary device,
   but the secondary device cannot remotely start an FA of the primary
   device.
-  Before the remote startup, ensure that the two OpenHarmony devices
   are on the same network segment and can ping each other on the
   distributed network. Otherwise, the remote startup fails.
-  Currently, only the FAs that have the same public key (that is, the
   same Huawei certificate) can be started between the primary and
   secondary devices.

How to Develop
--------------

To enable the primary device (smart TV) to start an FA of the secondary
device (assuming that the target FA has been developed), perform the
following steps:

1. Complete FA development for the smart TV on DevEco Studio.

2. Obtain the IDs of online secondary devices.

   ::

      // Import the header files required for device selection.
      import ohos.distributedschedule.interwork.DeviceInfo;
      import ohos.distributedschedule.interwork.DeviceManager;

      // Obtain the online device list.
      List<DeviceInfo> deviceInfoListOnline = DeviceManager.getDmsDeviceList(DeviceInfo.FLAG_GET_ONLINE_DEVICE);
      String remote_device_id;
      if (deviceInfoListOnline.size() > 0)
      {
          remote_device_id = deviceInfoListOnline[0].GetDeviceId(); // Obtain the ID of the first device in the online device list.
      }

3. Create a **Want** instance. You should first create an
   **ElementName** object with **deviceId**, **bundleName**,
   **abilityName** specified and add this object to the **Want**
   instance. Then, set the multi-device startup flag
   **Want.FLAG_ABILITYSLICE_MULTI_DEVICE** to the **Want** instance to
   enable remote FA startup.

   ::

      // Import related header files.
      import ohos.aafwk.ability.Ability;
      import ohos.aafwk.content.Want;
      import ohos.bundle.ElementName;

      // Start the remote FA on the secondary device.
      Want want = new Want(); // Create a Want instance that encapsulates information about the remote FA to start.
      // Use the device ID obtained in step 2 and specify the FA information.
      ElementName name = new ElementName(remote_device_id, "com.huawei.remote_package_name", "remote_class_name"); 
      want.setElement(name); // Add information about the target FA for startup to the Want instance.
      want.setFlags(Want.FLAG_ABILITYSLICE_MULTI_DEVICE); // Set the multi-device startup flag. If this flag is not set, remote FA startup will be unavailable.
      startAbility(want); // Start the specified FA based on the want parameter. If the name and type of the want parameter are different from those used in the IDE, use the parameter name and type in the IDE.
