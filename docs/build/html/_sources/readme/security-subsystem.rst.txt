Security Subsystem
==================

Overview
--------

This section provides samples about how to use existing security
mechanisms to improve system security features, including secure boot,
application permission management, inter-process communication (IPC)
authentication, Huawei Universal Keystore Service (HUKS), HiChain, and
application signature verification.

Directory Structure
-------------------

::

   security
   ├── framework
   │     ├── appverify    Application signature verification
   │     ├── crypto_lite    Encryption and decryption
   │     ├── hichainsdk_lite    Device authentication
   │     ├── huks_lite    Key and certificate management
   │     ├── secure_os    Secure OS
   ├── interface    Interface directory
   │     ├── innerkits    Internal kit directory
   │     │     ├── appverify    Application signature verification
   │     │     ├── crypto_lite    Encryption and decryption
   │     │     ├── hichainsdk_lite    Device authentication
   │     │     ├── huks_lite    Key and certificate management
   │     │     ├── iam_lite    Application permission management
   │     │     ├── secure_os    Secure OS
   │     ├── kits    External kit directory
   │     │     ├── iam_lite    Application permission management
   ├── services    Implementation
   │     ├── iam_lite    Application permission management
   │     ├── secure_os    Secure OS

Constraints
-----------

C programming language is used. The preceding security features are
mainly used on Cortex-A or devices with equivalent processing
capabilities. On Cortex-M or devices with equivalent processing
capabilities, only HUKS and HiChain are available.

Secure Boot
-----------

To generate a x509 image package, perform compilation to generate the
required binary images, including kernel images **kernel.bin**
(liteos/OHOS_Image) and **rootfs.img**. If the Hi3516DV300 chip is used,
the generated images are stored in the
**out\ipcamera_hi3516dv300_liteos_a** directory. Copy the binary images
and the secure uboot private keys (in the
**vendor\hisi\hi35xx\hi3516dv300\uboot\secureboot_release** directory)
to the **secureboot_ohos** directory (in the
**vendor\hisi\hi35xx\hi3516dv300\uboot** directory). Go to the
**x509_creater** directory, run the **./creater.sh** command, and
generate the x509 certificate as prompted. Return to the
**secureboot_ohos** directory and run **./sec_os.sh** to generate the
x509 image package.

Application Permission Management
---------------------------------

Application permissions are used to control access to system resources
and features related to personal privacy, for example, accessing
hardware features of personal devices such as cameras and microphones,
and reading and writing media files. The OS protects such data and
features through application permission management.

The following table describes fields in a permission.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row11107193541417">

.. raw:: html

   <th class="cellrowborder" valign="top" width="22.220000000000002%" id="mcps1.1.4.1.1">

.. raw:: html

   <p id="p6107535141420">

Field

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="35.099999999999994%" id="mcps1.1.4.1.2">

.. raw:: html

   <p id="p111080352143">

Value

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="42.68%" id="mcps1.1.4.1.3">

.. raw:: html

   <p id="p161080358141">

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

   <tr id="row151081735111418">

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.220000000000002%" headers="mcps1.1.4.1.1 ">

.. raw:: html

   <p id="p1108193521417">

name

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="35.099999999999994%" headers="mcps1.1.4.1.2 ">

.. raw:: html

   <p id="p131081435151413">

String

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="42.68%" headers="mcps1.1.4.1.3 ">

.. raw:: html

   <p id="p0108235141411">

Permission name

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row19108143516148">

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.220000000000002%" headers="mcps1.1.4.1.1 ">

.. raw:: html

   <p id="p51081355145">

reason

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="35.099999999999994%" headers="mcps1.1.4.1.2 ">

.. raw:: html

   <p id="p01082358147">

Multi-language string ID

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="42.68%" headers="mcps1.1.4.1.3 ">

.. raw:: html

   <p id="p191081235171414">

Purpose of requesting the permission.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row13108123516145">

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.220000000000002%" headers="mcps1.1.4.1.1 ">

.. raw:: html

   <p id="p18109835101415">

used-scene{

.. raw:: html

   </p>

.. raw:: html

   <p id="p910913358146">

ability,

.. raw:: html

   </p>

.. raw:: html

   <p id="p11109235181420">

when

.. raw:: html

   </p>

.. raw:: html

   <p id="p16109193531417">

}

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="35.099999999999994%" headers="mcps1.1.4.1.2 ">

.. raw:: html

   <p id="p4109123511420">

ability: string of the component class name

.. raw:: html

   </p>

.. raw:: html

   <p id="p19109133531410">

when: inuse and always

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="42.68%" headers="mcps1.1.4.1.3 ">

.. raw:: html

   <p id="p31091835151413">

Scene where the APIs controlled by this permission are called.

.. raw:: html

   </p>

.. raw:: html

   <p id="p93361156407">

This field declares what components can call the APIs controlled by this
permission in the specified scene (foreground/background).

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

IPC Authentication
------------------

-  If system services registered with Samgr provide APIs for other
   processes to access the services through IPC, access control policies
   must be configured; otherwise, access to the system services will be
   denied.

-  You can configure access control policies in
   **base/security/services/iam_lite/ipc_auth/include/policy_preset.h**.

   1. Define the policies for each feature.

   2. Add the feature policies to the global policy.

For example, to configure an access policy for the BMS service, whose
service registered with Samgr is **bundlems** and whose registered
feature is **BmsFeature**, perform the following operations:

1. Define feature policies. You can configure multiple features and
   configure multiple access policies for each feature.

**Figure 1** Example feature policy

|image1|

There are three types of access policies:

**Figure 2** Access policy structure

|image2|

-  **RANGE**: Processes with a UID within a specified range are allowed
   to access **BmsFeature**. **uidMin** and **uidMax** need to be
   specified.
-  **FIXED**: Processes with specified UIDs are allowed to access
   **BmsFeature**. **fixedUid** needs to be specified. A maximum number
   of eight UIDs can be configured.
-  **BUNDLENAME**: Only a specified application is allowed to access
   **BmsFeature**. **bundleName** needs to be specified.

2. Add the defined feature policies to the global policy. You need to
   configure the number of features.

**Figure 3** Registering a feature policy

|image3|

UID allocation rules:

1. Init process: 0

appspawn process: 1

Shell process: 2

4. Other built-in system services: less than or equal to 99

5. System applications (such as settings, home screen, and camera):
   100–999

6. Preset applications: 1000–9999

7. Common third-party applications: 10000 to **INT_MAX**

HUKS
----

In distributed scenarios, trust relationships need to be established
between devices with varied hardware capabilities and system
environments. A typical application is HiChain for trusted
interconnection between devices. In this case, a unified key management
service is required to ensure consistent APIs and key data formats, and
provide industry-standard encryption/decryption algorithms. HUKS is such
a service that provides unified key management and
encryption/decryption.

HUKS consists of native APIs, the hardware abstraction layer (HAL), and
Core Module.

1. Native APIs are implemented using the C language to ensure
   consistency among all devices, and include the APIs for key
   generation, encryption, and decryption.
2. Core Module depends on the HAL and provides core functions such as
   encryption and decryption, signature verification, and key storage.
3. HAL shields differences between hardware and OSs and defines the
   unified APIs for HUKS. It contains platform algoIOrithm libraries,
   file systems, and logs.

HiChain
-------

**Device Interconnection Security**

To transmit user data securely between devices, ensure that the devices
are trusted by each other. A trust relationship and a secure data
transmission channel must be established between the devices. This
section describes how an IoT controller and IoT device establish a trust
relationship.

|image4|

-  **IoT device interconnection security**

A trust relationship can be established between an IoT device that runs
OpenHarmony (such as the AI speaker, smart home device, and wearable
device) and an IoT controller (such as the smartphone and tablet).
Encrypted user data can be transmitted between the IoT device and IoT
controller through a secure connection.

-  **IoT service identifier of the IoT controller**

An IoT controller generates different identifiers for different IoT
device management services to isolate these services. The identifier can
be used for authentication and communication between an IoT controller
and an IoT device. It is an Ed25519 public/private key pair generated
using the elliptic curve cryptography.

-  **IoT device identifier**

An IoT device can generate its own device identifier for communicating
with the IoT controller. It is also an Ed25519 public/private key pair
generated using elliptic curve cryptography, with the private key stored
on the IoT device. Each time the device is restored to factory settings,
the public/private key pair will be reset.

The identifier can be used for secure communication between the IoT
controller and IoT device. After the devices exchange the service
identifier or device identifier, they can negotiate the key and
establish a secure communication channel.

-  **P2P trusted binding between devices**

When an IoT controller and an IOT device establish a trust relationship,
they exchange identifiers.

During this process, the user needs to enter or scan the PIN provided by
the IoT device on the IoT controller. PIN is either dynamically
generated if the IoT device has a screen, or preset by the manufacturer
if it does not have a screen. A PIN can be a number or a QR code. Then
the IoT controller and IoT device perform authentication and session key
exchange based on password authenticated key exchange (PAKE), and use
the session key to encrypt the channel for exchanging identity public
keys.

**Secure communication between the IoT controller and IoT device**

When an IoT controller and an IoT device communicate with each other
after establishing a trust relationship, they authenticate each other by
using the locally stored identity public key of the peer. Bidirectional
identity authentication and session key exchange are performed using the
Station-to-Station (STS) protocol during each communication. The session
key is used to encrypt the data transmission channel between the
devices.

Application Signature Verification
----------------------------------

To ensure the integrity of application content, OpenHarmony uses
application signatures and profiles to manage application sources. Only
pre-installed applications and applications from HUAWEI AppGallery can
be installed on devices.

**Basic Concepts**

-  **Developer certificate**

Identity digital certificate of a developer, which is used to sign local
debugging software

-  **Application debugging profile**

Application debugging authorization file that allows you to install and
debug an application on a specified device

-  **Application publishing certificate**

Identity digital certificate of an application publisher, which is used
to sign an application to be published or preset

-  **Application publishing profile**

Description file of an application, which is used for reviewing an
application to be published or preset

-  **APPID**

Unique identifier of an application, which consists of the application
bundle name and the public key of the application publishing certificate

**How Application Signature Verification Works**

1. Apply for becoming an authorized application developer on HUAWEI
   AppGallery.
2. Install and debug an application on a specified device.
3. Publish the application.

**Signature of an Application Published on HUAWEI AppGallery**\ 
----------------------------------------------------------------

-  **Application debugging scenario**

To develop and debug applications for OpenHarmony devices, you need to
apply for becoming an authorized application developer on HUAWEI
AppGallery. You need to generate a public/private key pair and upload
the public key to HUAWEI AppGallery. HUAWEI AppGallery creates a
developer certificate based on your identity information and the
uploaded public key, and issues the certificate through the developer
certificate CA. You also need to upload the application information and
debugging device ID for creating an application debugging profile, which
contains the HUAWEI AppGallery signature and cannot be tampered with.
Upon obtaining the developer certificate and application debugging
profile, you can install and debug applications signed with the private
key on a specified OpenHarmony device.

The application installation service of OpenHarmony verifies the
application signature to ensure application integrity. In addition, the
service verifies the developer certificate, application debugging
profile, and the mapping between them to ensure the validity of your
identity and the application.

|image5|

-  **Application publishing**

To publish applications in HUAWEI AppGallery, you need to use the
application publishing certificate and profile issued by HUAWEI
AppGallery to sign the applications. As shown in the following figure,
the procedure of applying for the application publishing certificate and
profile is similar to that of applying for the developer certificate and
application debugging profile (you can use the same public/private key
pair). Applications signed by the application publishing certificate
cannot be directly installed on devices. Instead, the applications must
be published in HUAWEI AppGallery for review. After the applications are
reviewed and approved, HUAWEI AppGallery uses the publishing certificate
to re-sign the applications. The re-signed applications can be
downloaded and installed by users.

The application installation service of OpenHarmony verifies the
application signature to ensure application integrity. In addition, the
service checks whether the signature certificate is from HUAWEI
AppGallery to ensure that the application is trusted.

|image6|

Repositories Involved
---------------------

security_services_app_verify

security_frameworks_crypto_lite

security_services_hichainsdk_lite

security_services_huks_lite

security_frameworks_secure_os

security_interfaces_innerkits_hichainsdk_lite

security_interfaces_innerkits_iam_lite

security_interfaces_innerkits_huks_lite

security_interfaces_innerkits_app_verify

security_interfaces_innerkits_crypto_lite

security_interfaces_innerkits_secure_os

security_interfaces_kits_iam_lite

security_services_iam_lite

security_services_secure_os

.. |image1| image:: figures/bms策略举例.png
.. |image2| image:: figures/策略类型2.png
.. |image3| image:: figures/全局策略2.png
.. |image4| image:: figures/en-us_image_0000001052584330.png
.. |image5| image:: figures/en-us_image_0000001051282241.png
.. |image6| image:: figures/en-us_image_0000001051562162.png
