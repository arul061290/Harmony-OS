Application Security
====================

Mechanism
---------

-  Application signature management

   After developing and debugging an OpenHarmony application, sign the
   application installation package using a private key, which matches a
   public key. Generally, the OEM generates a public/private key pair,
   presets the public key in the device, and stores the private key on a
   local server that is not connected to the Internet to prevent private
   key leakage. After you finish developing an application, you can use
   an external device (such as a USB flash drive) to upload the
   installation package to the server where the private key is stored,
   calculate the signature, and download the signature to the external
   device. During application installation, the hash value of the bundle
   is calculated using the SHA-256 algorithm. The hash value, together
   with the signature and preset public key, is used for authentication.
   The application can be installed only after the authentication is
   successful.

   In addition, the application source must be verified to ensure that
   the application is from a valid developer. As a developer, you must
   apply for a development certificate and use it to sign the
   application you have developed. During application installation, the
   upper-level certificate stored on the device is used to verify the
   signature to ensure validity of the developer.

-  Application permission control

   OpenHarmony allows users to install third-party applications and
   controls calls made by third-party applications to sensitive
   permissions. When developing an application, you need to declare the
   sensitive permissions that the application may invoke in the
   **profile.json** file. The permissions include static and dynamic
   ones. Static permissions need to be registered during application
   installation, and dynamic permissions can be invoked only upon user
   authorization. Authorization modes include system settings, manual
   authorization by applications, and others. In addition, application
   signature control is used to ensure that the application installation
   package has been confirmed by the device vendor.

   **Table 1** OpenHarmony system permissions

   .. raw:: html

      <table>

   .. raw:: html

      <thead align="left">

   .. raw:: html

      <tr id="row736832612616">

   .. raw:: html

      <th class="cellrowborder" valign="top" width="40.574057405740575%" id="mcps1.2.4.1.1">

   .. raw:: html

      <p id="p19859181913610">

   OpenHarmony System Permission

   .. raw:: html

      </p>

   .. raw:: html

      </th>

   .. raw:: html

      <th class="cellrowborder" valign="top" width="23.052305230523054%" id="mcps1.2.4.1.2">

   .. raw:: html

      <p id="p1985961983610">

   Authorization Mode

   .. raw:: html

      </p>

   .. raw:: html

      </th>

   .. raw:: html

      <th class="cellrowborder" valign="top" width="36.37363736373638%" id="mcps1.2.4.1.3">

   .. raw:: html

      <p id="p78592196368">

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

      <tr id="row2036892662618">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="40.574057405740575%" headers="mcps1.2.4.1.1 ">

   .. raw:: html

      <p id="p196912621513">

   ohos.permission.LISTEN_BUNDLE_CHANGE

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="23.052305230523054%" headers="mcps1.2.4.1.2 ">

   .. raw:: html

      <p id="p158591919143612">

   system_grant (static permission)

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="36.37363736373638%" headers="mcps1.2.4.1.3 ">

   .. raw:: html

      <p id="p138591019133617">

   Allows an application to listen for application changes.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row836872652610">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="40.574057405740575%" headers="mcps1.2.4.1.1 ">

   .. raw:: html

      <p id="p12859141903614">

   ohos.permission.GET_BUNDLE_INFO

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="23.052305230523054%" headers="mcps1.2.4.1.2 ">

   .. raw:: html

      <p id="p73429411292">

   system_grant (static permission)

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="36.37363736373638%" headers="mcps1.2.4.1.3 ">

   .. raw:: html

      <p id="p486021918369">

   Allows an application to obtain application information.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row143694264267">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="40.574057405740575%" headers="mcps1.2.4.1.1 ">

   .. raw:: html

      <p id="p1386031918365">

   ohos.permission.INSTALL_BUNDLE

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="23.052305230523054%" headers="mcps1.2.4.1.2 ">

   .. raw:: html

      <p id="p5356164112915">

   system_grant (static permission)

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="36.37363736373638%" headers="mcps1.2.4.1.3 ">

   .. raw:: html

      <p id="p1786016192367">

   Allows an application to install applications.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row1836942652617">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="40.574057405740575%" headers="mcps1.2.4.1.1 ">

   .. raw:: html

      <p id="p178601196361">

   ohos.permission.CAMERA

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="23.052305230523054%" headers="mcps1.2.4.1.2 ">

   .. raw:: html

      <p id="p123691246291">

   user_grant (dynamic permission)

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="36.37363736373638%" headers="mcps1.2.4.1.3 ">

   .. raw:: html

      <p id="p18860151923618">

   Allows an application to use the camera to take photos and record
   videos at any time.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row23691426132616">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="40.574057405740575%" headers="mcps1.2.4.1.1 ">

   .. raw:: html

      <p id="p586011195362">

   ohos.permission.MODIFY_AUDIO_SETTINGS

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="23.052305230523054%" headers="mcps1.2.4.1.2 ">

   .. raw:: html

      <p id="p14868849111715">

   system_grant (static permission)

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="36.37363736373638%" headers="mcps1.2.4.1.3 ">

   .. raw:: html

      <p id="p6860121943619">

   Allows an application to modify global audio settings, such as the
   volume and speaker for output.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row83692026202610">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="40.574057405740575%" headers="mcps1.2.4.1.1 ">

   .. raw:: html

      <p id="p1686071913363">

   ohos.permission.READ_MEDIA

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="23.052305230523054%" headers="mcps1.2.4.1.2 ">

   .. raw:: html

      <p id="p1837524122914">

   user_grant (dynamic permission)

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="36.37363736373638%" headers="mcps1.2.4.1.3 ">

   .. raw:: html

      <p id="p118604196369">

   Allows an application to read users’ favorite videos.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row0369192616265">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="40.574057405740575%" headers="mcps1.2.4.1.1 ">

   .. raw:: html

      <p id="p2807144613213">

   ohos.permission.MICROPHONE

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="23.052305230523054%" headers="mcps1.2.4.1.2 ">

   .. raw:: html

      <p id="p113782462914">

   user_grant (dynamic permission)

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="36.37363736373638%" headers="mcps1.2.4.1.3 ">

   .. raw:: html

      <p id="p13860119103612">

   Allows an application to use the microphone for audio recording at
   any time.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row626918467266">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="40.574057405740575%" headers="mcps1.2.4.1.1 ">

   .. raw:: html

      <p id="p1860181943619">

   ohos.permission.WRITE_MEDIA

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="23.052305230523054%" headers="mcps1.2.4.1.2 ">

   .. raw:: html

      <p id="p13381442297">

   user_grant (dynamic permission)

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="36.37363736373638%" headers="mcps1.2.4.1.3 ">

   .. raw:: html

      <p id="p9860919163615">

   Allows an application to write users’ favorite music.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row6270164602610">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="40.574057405740575%" headers="mcps1.2.4.1.1 ">

   .. raw:: html

      <p id="p1326132832215">

   ohos.permission.DISTRIBUTED_DATASYNC

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="23.052305230523054%" headers="mcps1.2.4.1.2 ">

   .. raw:: html

      <p id="p4861101915365">

   user_grant (dynamic permission)

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="36.37363736373638%" headers="mcps1.2.4.1.3 ">

   .. raw:: html

      <p id="p15861161973614">

   Allows an application to manage distributed data transmission.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row62701646182614">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="40.574057405740575%" headers="mcps1.2.4.1.1 ">

   .. raw:: html

      <p id="p15247193132317">

   com.huawei.permission.DISTRIBUTED_VIRTUALDEVICE

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="23.052305230523054%" headers="mcps1.2.4.1.2 ">

   .. raw:: html

      <p id="p1081717542913">

   user_grant (dynamic permission)

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="36.37363736373638%" headers="mcps1.2.4.1.3 ">

   .. raw:: html

      <p id="p11861119123617">

   Allows an application to use distributed virtualization features.

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

Recommended Practices
---------------------

When developing an application, determine what permissions your
application needs and register the permissions in the **profile.json**
file. Sign the application to ensure that the devices on which the
application will be installed can verify its integrity and source.
