BundleManager
=============

**Overview**\ 
--------------

Provides structures and functions for managing application bundles and
obtaining application information.

You can use functions provided by this module to install, update, or
uninstall an application, obtain `AbilityInfo <abilityinfo.md>`__ and
`BundleInfo <bundleinfo.md>`__ about an application, and obtain the
bundle name of an application based on the application’s user ID (UID).

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

   <tr id="row1793113913093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p919981763093521">

File Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p732970626093521">

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

   <tr id="row1869706205093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p747288203093521">

ability_info.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1620921144093521">

Declares structures and functions for managing ability information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1607180618093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p416400925093521">

appexecfwk_errors.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p861480779093521">

Declares error codes returned by bundle management functions.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row676168500093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p13523210093521">

bundle_info.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p941027504093521">

Declares structures and functions for managing application bundle
information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2134376377093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p765709369093521">

bundle_manager.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1906008099093521">

Declares functions used for managing application bundles and obtaining
bundle information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1723044627093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1535925580093521">

element_name.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1128859850093521">

Declares the structure that defines the required information for
querying AbilityInfo, including the device ID, bundle name, and class
name, and functions for setting such information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row486388225093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p534542925093521">

module_info.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p240703501093521">

Declares structures and functions for managing HAP package information.

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

   <tr id="row660381627093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p285032353093521">

Data Structure Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1128761498093521">

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

   <tr id="row1850014023093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1584578457093521">

AbilityInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p500432909093521">

Defines the ability information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1851248532093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p183474961093521">

BundleInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p192903337093521">

Defines the bundle information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row16962057093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2120342730093521">

ElementName

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p839340808093521">

Defines the ability information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row225977623093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1163858266093521">

MetaData

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p863846640093521">

Defines the metadata information in a ModuleInfo object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1620653953093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p628156997093521">

ModuleInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1665750187093521">

Defines the HAP information.

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

   <tr id="row542578146093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1954455529093521">

Typedef Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1754604855093521">

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

   <tr id="row2004666810093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2100179586093521">

InstallerCallback) (const uint8_t resultCode, const void
\*resultMessage)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p265532883093521">

typedef void(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1328599859093521">

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

Enumerations
------------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2051079811093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1329321181093521">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p602219339093521">

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

   <tr id="row95913554093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1910762204093521">

AbilityType { UNKNOWN = 0, PAGE, SERVICE }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p465484643093521">

Enumerates types of templates used by an ability.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row859041213093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1923390096093521">

LaunchMode { SINGLETON = 0, STANDARD }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p136414741093521">

Enumerates startup modes of an ability.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1966402120093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p381974435093521">

AppexecfwkErrors { ERR_OK = 0, ERR_APPEXECFWK_QUERY_PARAMETER_ERROR,
ERR_APPEXECFWK_QUERY_NO_INFOS, ERR_APPEXECFWK_QUERY_INFOS_INIT_ERROR,
ERR_APPEXECFWK_OBJECT_NULL, ERR_APPEXECFWK_INSTALL_FAILED_INTERNAL_ERROR
= 10, ERR_APPEXECFWK_INSTALL_FAILED_PARAM_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_FILE_PATH_INVALID,
ERR_APPEXECFWK_INSTALL_FAILED_FILE_NOT_EXISTS,
ERR_APPEXECFWK_INSTALL_FAILED_INVALID_FILE_NAME,
ERR_APPEXECFWK_INSTALL_FAILED_BAD_FILE,
ERR_APPEXECFWK_INSTALL_FAILED_CREATE_FILE_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_CREATE_CODE_DIR_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_REMOVE_CODE_DIR_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_CREATE_PERMISSIONS_DIR_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_RENAME_DIR_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_RENAME_FILE_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_REMOVE_DATA_DIR_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_CREATE_DATA_DIR_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_RECORD_INFO_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_UID_AND_GID_BACKUP_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_CHOWN_DATA_DIR_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_VERSION_DOWNGRADE,
ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_BUNDLE_NUMBER,
ERR_APPEXECFWK_INSTALL_FAILED_STORE_PERMISSIONS_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_FILE_DATA_INVALID,
ERR_APPEXECFWK_INSTALL_FAILED_INCOMPATIBLE_SIGNATURE,
ERR_APPEXECFWK_INSTALL_FAILED_INVALID_PROVISIONINFO,
ERR_APPEXECFWK_INSTALL_FAILED_OPERATE_SIGNED_FILE_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_APP_SIGNATURE_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_PROFILE_SIGNATURE_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_INTERNAL_SIGNATURE_ERROR,
ERR_APPEXECFWK_SET_DEBUG_MODE_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_PROFILE_ERROR = 40,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_BUNDLENAME_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_INVALID_BUNDLENAME,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_VENDOR_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_VERSIONCODE_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_VERSIONNAME_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_PERMISSIONS_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_API_VERSION_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_DEVICE_CONFIG_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_KEEPALIVE_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_MODULENAME_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_INVALID_MODULENAME,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_MODULE_DESCRIPTION_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_DEVICETYPE_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_DISTRO_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_DISTRO_MODULENAME_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_DISTRO_MODULETYPE_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_DISTRO_DELIVERY_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_METADATA_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_ABILITIES_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_ABILITY_NAME_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_ABILITY_TYPE_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_ABILITY_ICONPATH_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_ABILITY_LABEL_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_ABILITY_DESCRIPTION_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_ABILITY_LAUNCHTYPE_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_ABILITY_VISIBLE_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_INVALID_BUNDLENAME_LENGTH,
ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_LABEL_LENGTH_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_VERSIONNAME_LENGTH_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_METADATA_NAME_LENGTH_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_METADATA_VALUE_LENGTH_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_VENDOR_LENGTH_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_MODULENAME_LENGTH_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_ABILITYNAME_LENGTH_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_ABILITY_DESCRIPTION_LENGTH_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_ABILITY_LABEL_LENGTH_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_EXTRACTOR_NOT_INIT,
ERR_APPEXECFWK_INSTALL_FAILED_EXTRACT_HAP_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_JS_DIR_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_RESOURCE_INDEX_NOT_EXISTS,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_LABEL_RES_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_ICON_RES_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_PARSE_DESCRIPTION_RES_ERROR,
ERR_APPEXECFWK_INSTALL_FAILED_SEND_REQUEST_ERROR,
ERR_APPEXECFWK_UNINSTALL_FAILED_INTERNAL_ERROR = 90,
ERR_APPEXECFWK_UNINSTALL_FAILED_PARAM_ERROR,
ERR_APPEXECFWK_UNINSTALL_FAILED_BUNDLE_NOT_EXISTS,
ERR_APPEXECFWK_UNINSTALL_FAILED_DELETE_DIRS_ERROR,
ERR_APPEXECFWK_UNINSTALL_FAILED_DELETE_RECORD_INFO_ERROR,
ERR_APPEXECFWK_UNINSTALL_FAILED_DELETE_PERMISSIONS_ERROR,
ERR_APPEXECFWK_UNINSTALL_FAILED_BUNDLE_NOT_UNINSTALLABLE,
ERR_APPEXECFWK_UNINSTALL_FAILED_DELETE_UID_INFO_ERROR,
ERR_APPEXECFWK_UNINSTALL_FAILED_SEND_REQUEST_ERROR,
ERR_APPEXECFWK_DUMP_ERROR = 100, ERR_APPEXECFWK_COMMAND_ERROR,
ERR_APPEXECFWK_CALLBACK_REGISTER_FAILED,
ERR_APPEXECFWK_CALLBACK_UNREGISTER_FAILED,
ERR_APPEXECFWK_CALLBACK_GENERATE_LOCAL_SERVICEID_FAILED,
ERR_APPEXECFWK_CALLBACK_SERVICEID_TRANSMITTED_FAILED,
ERR_APPEXECFWK_CALLBACK_NEVER_REGISTERED,
ERR_APPEXECFWK_CALLBACK_OBTAIN_ALL_BUNDLE_FAILED,
ERR_APPEXECFWK_CALLBACK_NULL_CORRESPONDING_CALLBACK,
ERR_APPEXECFWK_CALLBACK_GET_INSTALLTYPE_FAILED,
ERR_APPEXECFWK_CALLBACK_GET_ERROR_INSTALLTYPE,
ERR_APPEXECFWK_SERIALIZATION_FAILED,
ERR_APPEXECFWK_DESERIALIZATION_FAILED,
ERR_APPEXECFWK_SYSTEM_INTERNAL_ERROR,
ERR_APPEXECFWK_NO_BUNDLENAME_FOR_UID, ERR_APPEXECFWK_IPCIO_UNAVAILABLED,
ERR_APPEXECFWK_INVOKE_ERROR, ERR_APPEXECFWK_PERMISSION_DENIED }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p369097805093521">

Enumerates error codes provided by the Bundle Manager Service.

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

   <tr id="row121296279093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1289575734093521">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p728571820093521">

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

   <tr id="row1674376475093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1401644731093521">

ClearAbilityInfo (AbilityInfo \*abilityInfo)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p786550091093521">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1821831815093521">

Clears an AbilityInfo object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1859906909093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p945012461093521">

ClearBundleInfo (BundleInfo \*bundleInfo)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p369027243093521">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p368788772093521">

Clears a BundleInfo object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row859193333093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p577911181093521">

RegisterCallback (BundleStatusCallback \*BundleStatusCallback)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1681533592093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p689589102093521">

Registers a callback to monitor the installation, update, and
uninstallation state changes of an application.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row916699480093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p261374341093521">

UnregisterCallback ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p623132084093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p679759869093521">

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

   <tr id="row1930519011093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p923624192093521">

Install (const char *hapPath, const InstallParam*\ installParam,
InstallerCallback installerCallback)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p84818610093521">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p228326753093521">

Installs or updates an application.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row324116416093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p396691451093521">

Uninstall (const char *bundleName, const InstallParam*\ installParam,
InstallerCallback installerCallback)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1429507132093521">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p993393501093521">

Uninstalls an application.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row376402025093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1114443723093521">

QueryAbilityInfo (const Want *want, AbilityInfo*\ abilityInfo)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1733187778093521">

uint8_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1453439028093521">

Queries the AbilityInfo of an ability based on the information carried
in the Want structure.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row400056372093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p175657797093521">

GetBundleInfo (const char *bundleName, int32_t flags,
BundleInfo*\ bundleInfo)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1367884189093521">

uint8_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p94462384093521">

Obtains the BundleInfo of an application based on the specified bundle
name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1878123309093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p157003656093521">

GetBundleInfos (const int flags, BundleInfo \**bundleInfos, int32_t
\*len)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1453320315093521">

uint8_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1614233916093521">

Obtains the BundleInfo of all bundles in the system.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1382835757093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1615448619093521">

QueryKeepAliveBundleInfos (BundleInfo \**bundleInfos, int32_t \*len)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p92606509093521">

uint8_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p778632645093521">

Obtains the BundleInfo of all keep-alive applications in the system.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row38693616093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p948981354093521">

GetBundleInfosByMetaData (const char \*metaDataKey, BundleInfo
\**bundleInfos, int32_t \*len)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2118879914093521">

uint8_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1264075806093521">

Obtains the BundleInfo of application bundles based on the specified
MetaData.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row102360059093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p898881225093521">

GetBundleNameForUid (int32_t uid, char \**bundleName)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1557690892093521">

uint8_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p7034499093521">

Obtains the bundle name of an application based on the specified UID.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1963553440093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1089049175093521">

ClearElement (ElementName \*element)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p246898233093521">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1077839849093521">

Clears the internal data of a specified ElementName.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row512937472093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p71581386093521">

SetElementDeviceID (ElementName *element, const char*\ deviceId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1076172885093521">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p1454612503093521">

Sets the device ID used to query AbilityInfo.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1555762653093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1176334384093521">

SetElementBundleName (ElementName *element, const char*\ bundleName)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1377375157093521">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p1091204771093521">

Sets the bundle name used to query AbilityInfo.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1774171577093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p658551431093521">

SetElementAbilityName (ElementName *element, const char*\ abilityName)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1552623744093521">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p426377150093521">

Sets the class name of the ability used to query AbilityInfo.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row438703208093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2132084322093521">

ClearModuleInfo (ModuleInfo \*moduleInfo)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p595365136093521">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1234973230093521">

Clears a ModuleInfo object.

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

**Typedef Documentation**\ 
---------------------------

InstallerCallback
-----------------

::

   typedef void(* InstallerCallback) (const uint8_t resultCode, const void *resultMessage)

**Description:**

Called when an application is installed, updated, or uninstalled.

This function can be registered through
`Install <bundlemanager.md#gaf1f1521a64cc98f076b0082df6c0abdd>`__ and
`Uninstall <bundlemanager.md#gaa117e44378315a61b4e71fd252b2e496>`__ to
receive the installation, update, and uninstallation result.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row58893898093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p53721517093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1962111118093521">

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

   <tr id="row1314325301093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

resultCode

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the status code returned for the application installation,
update, or uninstallation result. For details, see AppexecfwkErrors.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1497689551093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

resultMessage

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the result message returned with the status code.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Enumeration Type Documentation**\ 
------------------------------------

AbilityType
-----------

::

   enum [AbilityType](bundlemanager.md#ga44b675d687acff3d739404c1227b4259)

**Description:**

Enumerates types of templates used by an ability.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2112762075093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1119009550093521">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p214173517093521">

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

   <tr id="row1944238126093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

UNKNOWN

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1165683046093521">

Unknown

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2064764759093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PAGE

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2113490324093521">

Page

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row761144862093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

SERVICE

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1155679750093521">

Service

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

AppexecfwkErrors
----------------

::

   enum [AppexecfwkErrors](bundlemanager.md#gac318d4f4dc0125e2367ea8c539770ed1)

**Description:**

Enumerates error codes provided by the Bundle Manager
`Service <service.md>`__.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row21673050093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p181326643093521">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p259661758093521">

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

   <tr id="row1128564832093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_OK

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1671245110093521">

The function is successfully called.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1550376434093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_QUERY_PARAMETER_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p216654507093521">

Incorrect parameter for querying AbilityInfo or BundleInfo.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row171880679093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_QUERY_NO_INFOS

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p201025105093521">

No AbilityInfo or BundleInfo is found.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1352840430093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_QUERY_INFOS_INIT_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1486331419093521">

An error occurred when initializing BundleInfo or AbilityInfo during
information query.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row318877754093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_OBJECT_NULL

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2003600519093521">

The object or pointer is null.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1550723600093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_INTERNAL_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1342828483093521">

Failed to install the application due to an internal logic error.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2106395871093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARAM_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1141020031093521">

Failed to install the application due to incorrect parameters.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row328903254093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_FILE_PATH_INVALID

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1830511926093521">

Failed to install the application because the installation file path is
invalid.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row503438612093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_FILE_NOT_EXISTS

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2025112739093521">

Failed to install the application because the installation file does not
exist.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row956791300093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_INVALID_FILE_NAME

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p490416033093521">

Failed to install the application because the installation file name is
invalid.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row299562518093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_BAD_FILE

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1990533129093521">

Failed to install the application due to incorrect file content.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1242992977093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_CREATE_FILE_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2010041952093521">

Failed to install the application due to a file creation error.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row522766567093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_CREATE_CODE_DIR_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1929681575093521">

Failed to install the application due to a file path creation error.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row982695176093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_REMOVE_CODE_DIR_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1808837174093521">

Failed to install the application due to a file path deletion error.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row926051444093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_CREATE_PERMISSIONS_DIR_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1482901112093521">

Failed to install the application because an error occurred when
creating the permission file directory.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1729745434093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_RENAME_DIR_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1941088940093521">

Failed to install the application due to a path renaming error.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row960880758093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_RENAME_FILE_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1879504623093521">

Failed to install the application due to a file renaming error.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1763433530093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_REMOVE_DATA_DIR_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1236798838093521">

Failed to install the application due to an error occurred when removing
the data path.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row611521365093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_CREATE_DATA_DIR_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2040771235093521">

Failed to install the application due to an error occurred when creating
the data path.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row696053568093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_RECORD_INFO_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p904652752093521">

Failed to install the application due to an error occurred when
recording installation information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1925719458093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_UID_AND_GID_BACKUP_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1417432531093521">

Failed to install the application due to an error occurred when backing
up the UID and GID.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1003072324093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_CHOWN_DATA_DIR_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1918462896093521">

Failed to install the application due to an error occurred when changing
ownership of the data directory.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row261024112093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_VERSION_DOWNGRADE

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p31174058093521">

Failed to install the application because an application of a later
version has been installed.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row943927576093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_BUNDLE_NUMBER

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2087452718093521">

Failed to install the application because the number of installed
applications exceeds the maximum (30). This error code is available only
to basic watches.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1542429534093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_STORE_PERMISSIONS_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p101896163093521">

Failed to install the application due to an error occurred when storing
permission information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1661509933093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_FILE_DATA_INVALID

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1616944600093521">

Failed to install the application due to invalid file data. This error
code is available only to basic watches.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1891748385093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_INCOMPATIBLE_SIGNATURE

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1377416591093521">

Failed to install the application due to unmatched signature used for
version update.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1975525203093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_INVALID_PROVISIONINFO

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1594417392093521">

Failed to install the application due to unmatched provisioning
information during signature verification.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1378090969093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_OPERATE_SIGNED_FILE_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1881551754093521">

Failed to install the application due to an error occurred when
processing the signature file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1536543905093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_APP_SIGNATURE_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1893710130093521">

Failed to install the application due to an error occurred when parsing
the application signature.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row762915430093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_PROFILE_SIGNATURE_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p376172717093521">

Failed to install the application due to an error occurred when parsing
the file signature.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1632946282093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_INTERNAL_SIGNATURE_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1737101593093521">

Failed to install the application due to an internal error during
signature verification.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2042313111093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_SET_DEBUG_MODE_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p249793082093521">

Failed to install the application due to an error occurred when setting
the signature verification mode.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row105409504093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_PROFILE_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p521022526093521">

Failed to parse the file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1783889812093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_BUNDLENAME_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1705562286093521">

Failed to parse the bundle name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row597804088093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_INVALID_BUNDLENAME

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p25645234093521">

Invalid bundle name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1060148372093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_VENDOR_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p742403208093521">

Failed to parse the vendor information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row539985688093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_VERSIONCODE_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p800246655093521">

Failed to parse the version code.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1638502394093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_VERSIONNAME_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p539116618093521">

Failed to parse the version name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1773654246093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_PERMISSIONS_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p384601954093521">

Failed to parse the installation permission information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row341217297093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_API_VERSION_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p723385448093521">

Failed to parse the API version.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1774632649093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_DEVICE_CONFIG_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p917891309093521">

Failed to parse the device configuration.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row487703049093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_KEEPALIVE_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p796780619093521">

Failed to parse the isKeepAlive field of the application.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1500779727093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_MODULENAME_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p120111366093521">

Failed to parse the name field of the application’s HAP package. The HAP
information is encapsulated in a ModuleInfo object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1062068617093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_INVALID_MODULENAME

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1651701370093521">

Invalid HAP name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1817786258093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_MODULE_DESCRIPTION_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1330092271093521">

Failed to parse the HAP description information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1927174386093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_DEVICETYPE_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1690738224093521">

Failed to parse the deviceType field of the application’s HAP package.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row585959628093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_DISTRO_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2069770364093521">

Failed to parse the HAP information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row717739429093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_DISTRO_MODULENAME_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p210572711093521">

Failed to parse the moduleName field of the application’s HAP package.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row504102502093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_DISTRO_MODULETYPE_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p289127541093521">

Invalid HAP type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1178580372093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_DISTRO_DELIVERY_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1682997438093521">

Failed to parse the isDeliveryInstall field of the application’s HAP
package.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1564177336093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_METADATA_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p607411629093521">

Failed to parse the MetaData information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1887433158093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_ABILITIES_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1533102746093521">

Failed to parse the AbilityInfo.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1718699579093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_ABILITY_NAME_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p759603252093521">

Failed to parse the class name of the ability.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1368888684093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_ABILITY_TYPE_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1650829632093521">

Failed to parse the template used by the ability.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row507482523093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_ABILITY_ICONPATH_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p15356469093521">

Failed to parse the icon path of the ability.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1340691524093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_ABILITY_LABEL_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p35642318093521">

Failed to parse the label of the ability.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1656431608093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_ABILITY_DESCRIPTION_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1336622161093521">

Failed to parse the description of the ability.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row422166329093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_ABILITY_LAUNCHTYPE_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p311374046093521">

Failed to parse the startup mode of the ability.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1316786154093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_ABILITY_VISIBLE_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2054312017093521">

Failed to parse the isVisible field of the ability.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1161191498093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_INVALID_BUNDLENAME_LENGTH

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p672222933093521">

Invalid length of the bundle name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2029958940093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_LABEL_LENGTH_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p531816140093521">

The parsed application label exceeds the maximum length (255 bytes).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row986174956093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_VERSIONNAME_LENGTH_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p4612224093521">

The parsed application version name exceeds the maximum length (127
bytes).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row951218862093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_METADATA_NAME_LENGTH_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p467077811093521">

The parsed application metadata name exceeds the maximum length (255
bytes).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row754667942093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_METADATA_VALUE_LENGTH_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1427156186093521">

The parsed application metadata value exceeds the maximum length (255
bytes).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row709089290093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_VENDOR_LENGTH_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p391163194093521">

The parsed application vendor name exceeds the maximum length (255
bytes).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row935497354093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_MODULENAME_LENGTH_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p156340629093521">

The parsed HAP name exceeds the maximum length (31 bytes).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row779813635093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_ABILITYNAME_LENGTH_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p427473637093521">

The parsed ability class name exceeds the maximum length (127 bytes).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row827254673093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_ABILITY_DESCRIPTION_LENGTH_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1883158082093521">

The parsed ability description exceeds the maximum length (255 bytes).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1183101334093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_EXCEED_MAX_ABILITY_LABEL_LENGTH_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p122707092093521">

The parsed ability label exceeds the maximum length (255 bytes).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row227508683093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_EXTRACTOR_NOT_INIT

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p903241373093521">

Failed to initialize the extractor.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row113237027093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_EXTRACT_HAP_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1348382719093521">

Failed to extract hap.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row34929068093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_JS_DIR_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1222030494093521">

Failed to parse the JavaScript path. This error code is available only
to basic watches.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row803287004093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_RESOURCE_INDEX_NOT_EXISTS

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1569579947093521">

The resource index does not exist.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row797715969093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_LABEL_RES_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1708132028093521">

Failed to parse the label resource.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1680361701093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_ICON_RES_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p667399953093521">

Failed to parse the icon resource.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1081131257093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_PARSE_DESCRIPTION_RES_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p751558777093521">

Failed to parse the description resource.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row914634576093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INSTALL_FAILED_SEND_REQUEST_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1132426731093521">

Failed to install the application due to a request sending error.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row345298797093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_UNINSTALL_FAILED_INTERNAL_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1539152122093521">

Failed to uninstall the application due to an internal error.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row232181075093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_UNINSTALL_FAILED_PARAM_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p514175282093521">

Failed to uninstall the application due to incorrect input parameters.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1499126027093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_UNINSTALL_FAILED_BUNDLE_NOT_EXISTS

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1253241288093521">

Failed to uninstall the application because it does not exist.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1754700633093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_UNINSTALL_FAILED_DELETE_DIRS_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p404028929093521">

Failed to uninstall the application due to an error occurred when
deleting the path.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row234009439093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_UNINSTALL_FAILED_DELETE_RECORD_INFO_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1858285793093521">

Failed to uninstall the application due to an error occurred when
deleting the installation record.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row857915361093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_UNINSTALL_FAILED_DELETE_PERMISSIONS_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1528140273093521">

Failed to uninstall the application due to an error occurred when
deleting the permission information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row341948095093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_UNINSTALL_FAILED_BUNDLE_NOT_UNINSTALLABLE

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1334255238093521">

Failed to uninstall the application because the application cannot be
uninstalled.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1364749397093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_UNINSTALL_FAILED_DELETE_UID_INFO_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p687770285093521">

Failed to uninstall the application due to an error occurred when
deleting the UID information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1859742058093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_UNINSTALL_FAILED_SEND_REQUEST_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1998606006093521">

Failed to uninstall the application due to a request sending error.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2100025237093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_DUMP_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1115666819093521">

Incorrect dump information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1587004753093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_COMMAND_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p351856071093521">

Incorrect command.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row512661145093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_CALLBACK_REGISTER_FAILED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1205179100093521">

Failed to register the callback.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1268094331093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_CALLBACK_UNREGISTER_FAILED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p905322704093521">

Failed to unregister the callback.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2025981853093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_CALLBACK_GENERATE_LOCAL_SERVICEID_FAILED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p826720172093521">

Failed to generate a service ID for the current process.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1210916089093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_CALLBACK_SERVICEID_TRANSMITTED_FAILED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1702201862093521">

Failed to transmit the service ID of the current process.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row309171381093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_CALLBACK_NEVER_REGISTERED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1396736700093521">

The callback is never registered.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2042864916093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_CALLBACK_OBTAIN_ALL_BUNDLE_FAILED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p609032428093521">

Failed to obtain the bundle names of all applications in the system.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1562939191093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_CALLBACK_NULL_CORRESPONDING_CALLBACK

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1215738106093521">

The required callback is unavailable.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1008283653093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_CALLBACK_GET_INSTALLTYPE_FAILED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p616542756093521">

Failed to obtain the installation type (installation or uninstallation).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1665182138093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_CALLBACK_GET_ERROR_INSTALLTYPE

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p194056334093521">

Incorrect installation type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row340834892093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_SERIALIZATION_FAILED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1751247097093521">

Serialization failed.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1327889587093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_DESERIALIZATION_FAILED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1649188941093521">

Deserialization failed.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2019716826093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_SYSTEM_INTERNAL_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1295498574093521">

Internal system error.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row687807327093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_NO_BUNDLENAME_FOR_UID

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p369555126093521">

No bundle name associated with the UID is found.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row860189365093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_IPCIO_UNAVAILABLED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p216770423093521">

The IpcIo structure is unavailable.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2105803388093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_INVOKE_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p733021506093521">

An error occurred when calling the invoke function of the Bundle Manager
Service.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row781447961093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ERR_APPEXECFWK_PERMISSION_DENIED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1901937823093521">

The server that invokes the Bundle Manager Service does not have
required permission.

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

LaunchMode
----------

::

   enum [LaunchMode](bundlemanager.md#ga605d46d860e356a74db6842e66522854)

**Description:**

Enumerates startup modes of an ability.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1498491874093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p882332387093521">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p350408673093521">

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

   <tr id="row1002401075093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

SINGLETON

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p775440350093521">

Singleton mode, allowing only one instance

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2117065033093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

STANDARD

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1628689557093521">

Standard mode, allowing multiple instances

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

**Function Documentation**\ 
----------------------------

ClearAbilityInfo()
------------------

::

   void ClearAbilityInfo ([AbilityInfo](abilityinfo.md) * abilityInfo)

**Description:**

Clears an `AbilityInfo <abilityinfo.md>`__ object.

This function clears and releases the memory occupied by the fields of
the pointer type included in the specified
`AbilityInfo <abilityinfo.md>`__ object.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1807315770093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2141302947093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1278144769093521">

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

   <tr id="row448576586093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

abilityInfo

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the AbilityInfo object to clear.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

ClearBundleInfo()
-----------------

::

   void ClearBundleInfo ([BundleInfo](bundleinfo.md) * bundleInfo)

**Description:**

Clears a `BundleInfo <bundleinfo.md>`__ object.

This function clears and releases the memory occupied by the fields of
the pointer type included in the specified
`BundleInfo <bundleinfo.md>`__ object.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1249252398093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1425632885093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1155237175093521">

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

   <tr id="row1288116560093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

bundleInfo

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the BundleInfo object to clear.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

ClearElement()
--------------

::

   void ClearElement ([ElementName](elementname.md) * element)

**Description:**

Clears the internal data of a specified
`ElementName <elementname.md>`__.

After `AbilityInfo <abilityinfo.md>`__ is queried, clear the internal
data of an `ElementName <elementname.md>`__ if it is no longer required.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row13496989093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p669799926093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p685684708093521">

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

   <tr id="row819524350093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

element

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the ElementName to clear.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

ClearModuleInfo()
-----------------

::

   void ClearModuleInfo ([ModuleInfo](moduleinfo.md) * moduleInfo)

**Description:**

Clears a `ModuleInfo <moduleinfo.md>`__ object.

This function clears and releases the memory occupied by the fields of
the pointer type included in the specified
`ModuleInfo <moduleinfo.md>`__ object.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1059407364093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p983109235093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1139124292093521">

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

   <tr id="row670212141093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

moduleInfo

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the ModuleInfo object to clear.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

GetBundleInfo()
---------------

::

   uint8_t GetBundleInfo (const char * bundleName, int32_t flags, [BundleInfo](bundleinfo.md) * bundleInfo )

**Description:**

Obtains the `BundleInfo <bundleinfo.md>`__ of an application based on
the specified bundle name.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1677855892093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p775331552093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p196593553093521">

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

   <tr id="row1939625031093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

bundleName

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the name of the application bundle to query.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1999543172093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

flags

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Specifies whether the obtained BundleInfo object can contain
AbilityInfo. The value 1 indicates that it can contain AbilityInfo, and
0 indicates that it cannot.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1735973783093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

bundleInfo

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the obtained BundleInfo object.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Attention:**

Before querying a `BundleInfo <bundleinfo.md>`__ object, you should
first call **memset** on the constructed `BundleInfo <bundleinfo.md>`__
object so that each field in it can be properly initialized for carrying
the obtained information.

**Returns:**

Returns
`ERR_OK <bundlemanager.md#ggac318d4f4dc0125e2367ea8c539770ed1aa26c163b80b1f6786ca81dadc14b00fb>`__
if this function is successfully called; returns another error code
defined in
`AppexecfwkErrors <bundlemanager.md#gac318d4f4dc0125e2367ea8c539770ed1>`__
otherwise.

GetBundleInfos()
----------------

::

   uint8_t GetBundleInfos (const int flags, [BundleInfo](bundleinfo.md) ** bundleInfos, int32_t * len )

**Description:**

Obtains the `BundleInfo <bundleinfo.md>`__ of all bundles in the system.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row240826745093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p362296363093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p149499964093521">

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

   <tr id="row1356204490093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

flags

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Specifies whether each of the obtained BundleInfo objects can contain
AbilityInfo. The value 1 indicates that it can contain AbilityInfo, and
0 indicates that it cannot.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row213984482093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

bundleInfos

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the double pointer to the obtained BundleInfo objects.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row368587871093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

len

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the number of BundleInfo objects obtained.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns
`ERR_OK <bundlemanager.md#ggac318d4f4dc0125e2367ea8c539770ed1aa26c163b80b1f6786ca81dadc14b00fb>`__
if this function is successfully called; returns another error code
defined in
`AppexecfwkErrors <bundlemanager.md#gac318d4f4dc0125e2367ea8c539770ed1>`__
otherwise.

GetBundleInfosByMetaData()
--------------------------

::

   uint8_t GetBundleInfosByMetaData (const char * metaDataKey, [BundleInfo](bundleinfo.md) ** bundleInfos, int32_t * len )

**Description:**

Obtains the `BundleInfo <bundleinfo.md>`__ of application bundles based
on the specified `MetaData <metadata.md>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row591299082093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p725593963093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p558861968093521">

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

   <tr id="row1867752428093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

metaDataKey

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the metadata name in the MetaData.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row683561039093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

bundleInfos

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the double pointer to the obtained BundleInfo objects.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1622344350093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

len

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the number of BundleInfo objects obtained.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns
`ERR_OK <bundlemanager.md#ggac318d4f4dc0125e2367ea8c539770ed1aa26c163b80b1f6786ca81dadc14b00fb>`__
if this function is successfully called; returns another error code
defined in
`AppexecfwkErrors <bundlemanager.md#gac318d4f4dc0125e2367ea8c539770ed1>`__
otherwise.

GetBundleNameForUid()
---------------------

::

   uint8_t GetBundleNameForUid (int32_t uid, char ** bundleName )

**Description:**

Obtains the bundle name of an application based on the specified UID.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1333750311093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p162150895093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p102988444093521">

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

   <tr id="row968437521093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

uid

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the UID of the application to query.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row22975477093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

bundleName

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the double pointer to the bundle name of the application.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns
`ERR_OK <bundlemanager.md#ggac318d4f4dc0125e2367ea8c539770ed1aa26c163b80b1f6786ca81dadc14b00fb>`__
if this function is successfully called; returns another error code
defined in
`AppexecfwkErrors <bundlemanager.md#gac318d4f4dc0125e2367ea8c539770ed1>`__
otherwise.

Install()
---------

::

   bool Install (const char * hapPath, const InstallParam * installParam, [InstallerCallback](bundlemanager.md#ga00f021e76d728d2d44e1a28887ccc3af) installerCallback )

**Description:**

Installs or updates an application.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2055587081093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1098930137093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2132054705093521">

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

   <tr id="row557708253093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

hapPath

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the path for storing the OpenHarmony Ability
Package (HAP) of the application to install or update.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1147055748093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

bundleCallback

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the callback to be invoked for notifying the installation or
update result.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **true** if this function is successfully called; returns
**false** otherwise.

QueryAbilityInfo()
------------------

::

   uint8_t QueryAbilityInfo (const [Want](want.md) * want, [AbilityInfo](abilityinfo.md) * abilityInfo )

**Description:**

Queries the `AbilityInfo <abilityinfo.md>`__ of an ability based on the
information carried in the `Want <want.md>`__ structure.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row797767663093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2112047274093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2070079002093521">

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

   <tr id="row157797826093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

want

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the Want structure used for querying the
specified ability.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1572326069093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

abilityInfo

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the obtained AbilityInfo object.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Attention:**

Before querying an `AbilityInfo <abilityinfo.md>`__ object, you should
first call **memset** on the constructed
`AbilityInfo <abilityinfo.md>`__ object so that each field in it can be
properly initialized for carrying the obtained information.

**Returns:**

Returns
`ERR_OK <bundlemanager.md#ggac318d4f4dc0125e2367ea8c539770ed1aa26c163b80b1f6786ca81dadc14b00fb>`__
if this function is successfully called; returns another error code
defined in
`AppexecfwkErrors <bundlemanager.md#gac318d4f4dc0125e2367ea8c539770ed1>`__
otherwise.

QueryKeepAliveBundleInfos()
---------------------------

::

   uint8_t QueryKeepAliveBundleInfos ([BundleInfo](bundleinfo.md) ** bundleInfos, int32_t * len )

**Description:**

Obtains the `BundleInfo <bundleinfo.md>`__ of all keep-alive
applications in the system.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1516522526093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2045632891093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1578613858093521">

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

   <tr id="row1428294321093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

bundleInfos

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the double pointer to the obtained BundleInfo objects.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1496165144093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

len

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the number of BundleInfo objects obtained.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns
`ERR_OK <bundlemanager.md#ggac318d4f4dc0125e2367ea8c539770ed1aa26c163b80b1f6786ca81dadc14b00fb>`__
if this function is successfully called; returns another error code
defined in
`AppexecfwkErrors <bundlemanager.md#gac318d4f4dc0125e2367ea8c539770ed1>`__
otherwise.

RegisterCallback()
------------------

::

   int32_t RegisterCallback (BundleStatusCallback * BundleStatusCallback)

**Description:**

Registers a callback to monitor the installation, update, and
uninstallation state changes of an application.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row783442767093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1682115450093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p870409052093521">

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

   <tr id="row1599161081093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

bundleCallback

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the callback to be invoked when the installation, update, or
uninstallation state of the monitored application changes.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row40732401093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

bundleName

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the bundle name of the application to monitor.
If this parameter is set to nullptr, the installation, update, or
uninstallation state of all applications will be monitored.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns
`ERR_OK <bundlemanager.md#ggac318d4f4dc0125e2367ea8c539770ed1aa26c163b80b1f6786ca81dadc14b00fb>`__
if this function is successfully called; returns another error code
defined in
`AppexecfwkErrors <bundlemanager.md#gac318d4f4dc0125e2367ea8c539770ed1>`__
otherwise.

SetElementAbilityName()
-----------------------

::

   bool SetElementAbilityName ([ElementName](elementname.md) * element, const char * abilityName )

**Description:**

Sets the class name of the ability used to query
`AbilityInfo <abilityinfo.md>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row773168224093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p829630877093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1831655249093521">

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

   <tr id="row1692171303093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

element

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the ElementName to set.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row574065410093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

abilityName

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the class name to set.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **true** if the setting is successful; returns **false**
otherwise.

SetElementBundleName()
----------------------

::

   bool SetElementBundleName ([ElementName](elementname.md) * element, const char * bundleName )

**Description:**

Sets the bundle name used to query `AbilityInfo <abilityinfo.md>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1045511573093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2053415525093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1638136950093521">

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

   <tr id="row1492592660093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

element

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the ElementName to set.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2138713387093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

bundleName

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the bundle name to set.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **true** if the setting is successful; returns **false**
otherwise.

SetElementDeviceID()
--------------------

::

   bool SetElementDeviceID ([ElementName](elementname.md) * element, const char * deviceId )

**Description:**

Sets the device ID used to query `AbilityInfo <abilityinfo.md>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row651048947093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1700894872093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1325436702093521">

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

   <tr id="row1206601700093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

element

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the ElementName to set.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1685590886093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

deviceId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the device ID to set.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **true** if the setting is successful; returns **false**
otherwise.

Uninstall()
-----------

::

   bool Uninstall (const char * bundleName, const InstallParam * installParam, [InstallerCallback](bundlemanager.md#ga00f021e76d728d2d44e1a28887ccc3af) installerCallback )

**Description:**

Uninstalls an application.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2141114823093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p263524617093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1156255887093521">

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

   <tr id="row636366823093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

bundleName

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the bundle name of the application to
uninstall.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1222177983093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

bundleCallback

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the callback to be invoked for notifying the uninstallation
result.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **true** if this function is successfully called; returns
**false** otherwise.

UnregisterCallback()
--------------------

::

   int32_t UnregisterCallback ()

**Description:**

Unregisters a callback previously registered for monitoring the
installation, update, and uninstallation state changes of an
application.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1603631108093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p884465190093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p218522356093521">

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

   <tr id="row2073656645093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

bundleName

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the bundle name of the application being
monitored. If this parameter is set to nullptr, monitoring on the
installation, update, or uninstallation state of all applications will
be canceled.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns
`ERR_OK <bundlemanager.md#ggac318d4f4dc0125e2367ea8c539770ed1aa26c163b80b1f6786ca81dadc14b00fb>`__
if this function is successfully called; returns another error code
defined in
`AppexecfwkErrors <bundlemanager.md#gac318d4f4dc0125e2367ea8c539770ed1>`__
otherwise.
