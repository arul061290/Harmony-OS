Distributed Communication Subsystem
===================================

Overview
--------

The use of different communication modes (such as USB, WLAN, and
Bluetooth) varies greatly and is complex. In addition, the convergence,
sharing, and conflicts between communication links cannot be resolved,
and communication security is difficult to guarantee. The distributed
communication subsystem manages unified distributed communication
between near-field devices and provides device discovery and data
transmission APIs that apply to all links. Currently, the following
features are available:

-  Service publishing: After a service is published, peripheral devices
   can discover and use it.
-  Data transmission: A session is established based on the service name
   and device ID to transmit data between services.
-  Security: Communication data is encrypted.

You can use APIs of the distributed communication subsystem to implement
fast and secure communication between devices without caring about
management of communication details, thereby achieving cross-platform
development.

Directory Structure
-------------------

The following figure shows the softbus_lite source code directory
structure.

**Table 1** softbus_lite source code directory structure

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row16552191445314">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p75521114125314">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2055231419539">

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

   <tr id="row15552151465314">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p255221425316">

authmanager

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p11552114135313">

Provides the device authentication mechanism and manages device
knowledge libraries.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1755251416537">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p455231495317">

discovery

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p15531214115319">

Provides a device discovery mechanism that is based on the Constrained
Application Protocol (CoAP).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row155534148533">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1252015524711">

trans_service

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1752055220713">

Provides authentication and transmission channels.

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

Constraints
-----------

-  Language: C
-  Networking: Devices must be in the same LAN.

Usage
-----

1. Discover devices.

When using device discovery, ensure that the device to perform a
discovery and the discovered device are in the same LAN and the devices
can receive packets from each other.

a. After a device sends a discovery request, it uses CoAP to send a
   broadcast packet in the LAN. The following figure shows the request
   packet.

|image1|

b. The discovered device uses the **PublishService** API to publish
   services. After receiving the broadcast packet, the device sends a
   CoAP unicast packet to the device that performs the discovery. The
   following figure shows the packet example.

|image2|

c. After receiving the packet, the device that performs the discovery
   updates device information.

The following is an example of how to use device discovery:

::

   // Declare the callback function.
   void onSuccess(int publishId)
   {
       printf("public success,publishId = %d\r\n", publishId);
   }
   void onFail(int publishId, PublishFailReason reason)
   {
       printf("publish failed, publishId = %d, reason = %d\r\n", publishId, reason);
   }
   // Publish services.
   PublishInfo info = {0};
   IPublishCallback cb = {0};
   cb.onPublishSuccess = onSuccess;
   cb.onPublishFail = onFail;
   char a[] = "456";
   info.capabilityData = a;
   info.capability = "ddmpCapability";
   info.dataLen = strlen("456");
   info.medium = 2;
   info.publishId = 1;
   PublishService("cxx", &info, &cb);

2. Transmit data.

The soft bus provides unified session-based transmission. Services can
receive and send data or obtain basic attributes through **sessionId**.
Currently, services can determine whether to accept a received session
based on the service requirements and session attributes. Currently,
sessions cannot be enabled.

The sample code for data transmission is as follows:

::

   // Define the service name, session name, and related callback.
   const char *g_moduleName  = "BUSINESS_NAME";
   const char *g_sessionName = "SESSION_NAME";
   struct ISessionListener * g_sessionCallback= NULL;

   // Implement the callback: After receiving data sent by the peer end using SendBytes, return a fixed message.
   void OnBytesReceivedTest(int sessionId, const void* data, unsigned int dataLen)
   {
       printf("OnBytesReceivedTest\n");
       printf("Recv Data: %s\n", (char *)data);
       printf("Recv Data dataLen: %d\n", dataLen);
       char *testSendData = "Hello World, Hello!";
       SendBytes(sessionId, testSendData, strlen(testSendData));
       return;
   }

   // Implement the callback: Perform relevant operations after the session is closed, for example, releasing service resources related to the current session. The session does not need to be released by the service.
   void OnSessionClosedEventTest(int sessionId)
   {
       printf("Close session successfully, sessionId=%d\n", sessionId);
   }

   // Implement the callback: Perform relevant operations after a session is opened. The return value 0 means to accept the session, and other values mean to reject the session. In the following example, only sessions with the same name from other devices are accepted.
   int OnSessionOpenedEventTest(int sessionId)
   {
       if (strcmp(GetPeerSessionName(sessionId), SESSION_NAME) != 0) {
           printf("Reject the session which name is different from mine, sessionId=%d\n", sessionId);
           return -1;
       }
       printf("Open session successfully, sessionId=%d\n", sessionId);
       return 0;
   }

   // Register the service session service and its callbacks with the soft bus.
   int StartSessionServer()
   {
       if (g_sessionCallback == NULL) {
           g_sessionCallback = (struct ISessionListener*)malloc(sizeof(struct ISessionListener));
       }
       if (g_sessionCallback == NULL) {
           printf("Failed to malloc g_sessionCallback!\n");
           return -1;
       }
       g_sessionCallback->onBytesReceived = OnBytesReceivedTest;
       g_sessionCallback->onSessionOpened = OnSessionOpenedEventTest;
       g_sessionCallback->onSessionClosed = OnSessionClosedEventTest;
       int ret = CreateSessionServer(g_moduleName , g_sessionName, g_sessionCallback);
       if (ret < 0) {
           printf("Failed to create session server!\n");
           free(g_sessionCallback);
           g_sessionCallback = NULL;
       }
       return ret;
   }

   // Delete the service session service and its callbacks from the soft bus.
   void StopSessionServer()
   {
       int ret = RemoveSessionServer(g_moduleName , g_sessionName);
       if (ret < 0) {
           printf("Failed to remove session server!\n");
           return;
       }
       if (g_sessionCallback != NULL) {
           free(g_sessionCallback);
           g_sessionCallback = NULL;
       }
   }

Repositories Involved
---------------------

communication_frameworks_wifi_lite

communication_frameworks_ipc_lite

communication_hals_wifi_lite

communication_interfaces_kits_ipc_lite

communication_interfaces_kits_softbuskit_lite

communication_interfaces_kits_wifi_lite

communication_services_softbus_lite

.. |image1| image:: figures/1.png
.. |image2| image:: figures/2.png
