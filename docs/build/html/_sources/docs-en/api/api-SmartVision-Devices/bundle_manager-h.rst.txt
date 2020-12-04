bundle_manager.h
================

**Overview**\ 
--------------

**Related Modules:**

`BundleManager <bundlemanager.md>`__

**Description:**

Declares functions used for managing application bundles and obtaining
bundle information.

You can use functions provided in this file to install, update, or
uninstall an application, obtain `AbilityInfo <abilityinfo.md>`__ and
`BundleInfo <bundleinfo.md>`__ about an application, obtain the bundle
name of an application based on the application’s user ID (UID), and
obtain `BundleInfo <bundleinfo.md>`__ objects of all applications or
keep-alive applications in the system.

**Since:**

1.0

**Version:**

1.0

**Summary**\ 
-------------

Typedefs
--------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1578854507093524">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1119954181093524">

Typedef Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1395542995093524">

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

   <tr id="row1989341526093524">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p715104919093524">

InstallerCallback) (const uint8_t resultCode, const void
\*resultMessage)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p201537064093524">

typedef void(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p398651634093524">

Called when an application is installed, updated, or uninstalled.

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

   <tr id="row104506316093524">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1252524407093524">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1314004158093524">

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

   <tr id="row684537882093524">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1782456800093524">

RegisterCallback (BundleStatusCallback \*BundleStatusCallback)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1672981302093524">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p703890370093524">

Registers a callback to monitor the installation, update, and
uninstallation state changes of an application.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1918818587093524">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p28868020093524">

UnregisterCallback ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p51573455093524">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1932701562093524">

Unregisters a callback previously registered for monitoring the
installation, update, and uninstallation state changes of an
application.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row338895256093524">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p577833894093524">

Install (const char *hapPath, const InstallParam*\ installParam,
InstallerCallback installerCallback)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p679552401093524">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p1200763507093524">

Installs or updates an application.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row322610870093524">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p708888161093524">

Uninstall (const char *bundleName, const InstallParam*\ installParam,
InstallerCallback installerCallback)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1598571794093524">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p139496451093524">

Uninstalls an application.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row455369973093524">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2035346100093524">

QueryAbilityInfo (const Want *want, AbilityInfo*\ abilityInfo)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p940481416093524">

uint8_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1297071093093524">

Queries the AbilityInfo of an ability based on the information carried
in the Want structure.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row589755105093524">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p194060647093524">

GetBundleInfo (const char *bundleName, int32_t flags,
BundleInfo*\ bundleInfo)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1060241240093524">

uint8_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1976563097093524">

Obtains the BundleInfo of an application based on the specified bundle
name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2111378669093524">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1437306654093524">

GetBundleInfos (const int flags, BundleInfo \**bundleInfos, int32_t
\*len)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p938588569093524">

uint8_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p174585517093524">

Obtains the BundleInfo of all bundles in the system.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row24683789093524">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2087923994093524">

QueryKeepAliveBundleInfos (BundleInfo \**bundleInfos, int32_t \*len)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1576599104093524">

uint8_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2096697820093524">

Obtains the BundleInfo of all keep-alive applications in the system.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1578630687093524">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1791884562093524">

GetBundleInfosByMetaData (const char \*metaDataKey, BundleInfo
\**bundleInfos, int32_t \*len)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p26245787093524">

uint8_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1084706552093524">

Obtains the BundleInfo of application bundles based on the specified
MetaData.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row978035039093524">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1041508641093524">

GetBundleNameForUid (int32_t uid, char \**bundleName)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p165039705093524">

uint8_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p411537936093524">

Obtains the bundle name of an application based on the specified UID.

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
