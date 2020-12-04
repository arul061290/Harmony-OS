Parameter
=========

**Overview**\ 
--------------

Provides functions for obtaining system parameters.

This module can obtain device information such as device type and
manufacturer.

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

   <tr id="row1248861041093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1728401573093523">

File Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1877853050093523">

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

   <tr id="row1639769413093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1140487342093523">

parameter.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p221033526093523">

Declares functions for obtaining system parameters.

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

   <tr id="row1931302609093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1116466615093523">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p733739402093523">

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

   <tr id="row1020220054093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2092998029093523">

GetParameter (const char *key, const char*\ def, char \*value, unsigned
int len)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1882815170093523">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p398194718093523">

Obtains a system parameter matching the specified key.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row516669785093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1561252009093523">

SetParameter (const char *key, const char*\ value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p264661786093523">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p198237632093523">

Sets or updates a system parameter.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row499435826093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1119444072093523">

GetProductType (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1313840134093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1979423143093523">

Obtains the device type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1486087999093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p18278811093523">

GetManufacture (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1299279981093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p415050108093523">

Obtains the device manufacturer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row929437629093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p338850531093523">

GetBrand (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p21256843093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1643984360093523">

Obtains the device brand.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1765685357093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2097463510093523">

GetMarketName (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1607330401093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1187060220093523">

Obtains the device marketing name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row248358973093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p275004468093523">

GetProductSeries (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1324899406093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1745516668093523">

Obtains the device series name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row449315299093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1329084388093523">

GetProductModel (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p716523645093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1148297952093523">

Obtains the device authentication model.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row756000334093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p170301001093523">

GetSoftwareModel (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1104137557093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1379173536093523">

Obtains the device software model.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1675599114093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p328224660093523">

GetHardwareModel (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1724109733093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1578380183093523">

Obtains the device hardware model.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1761878580093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p536570485093523">

GetHardwareProfile (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p958168334093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p707759194093523">

Obtains the device hardware profile.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1247599877093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2009746469093523">

GetSerial (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1840005117093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1455410709093523">

Obtains the device serial number (SN).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1697329777093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1636918761093523">

GetOsName (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p996545081093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1702593018093523">

Obtains the operating system (OS) name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1572013438093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1473262768093523">

GetDisplayVersion (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p39896933093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1836309266093523">

Obtains the software version visible to users.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row255946012093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p183773978093523">

GetBootloaderVersion (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p886296348093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p754253369093523">

Obtains the bootloader version of this device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row364476806093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1554949555093523">

GetSecurityPatchTag (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1101119099093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p518331584093523">

Obtains the security patch tag.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row936882442093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p387947115093523">

GetAbiList (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p131242343093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1878753534093523">

Obtains the list of application binary interfaces (ABIs) supported on
this device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1398996054093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1109412012093523">

GetSdkApiLevel (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2024078415093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1945282121093523">

Obtains the SDK API level that matches the current system software.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row474514530093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p510507751093523">

GetFirstApiLevel (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p356723414093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p467908179093523">

Obtains the first SDK API level of the system software.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row689093441093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p879486719093523">

GetIncrementalVersion (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1210474311093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p958170233093523">

Obtains the incremental version.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2110253737093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1637011210093523">

GetVersionId (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p572131669093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1003059329093523">

Obtains the version ID.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1296764116093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p123310986093523">

GetBuildType (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p997308206093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1853281070093523">

Obtains the build type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row621677990093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2102103534093523">

GetBuildUser (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2027486460093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p872797589093523">

Obtains the build account user name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row251286060093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p773359516093523">

GetBuildHost (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p568602662093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p435137115093523">

Obtains the build host name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1781230758093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p908351599093523">

GetBuildTime (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p753788626093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1220106210093523">

Obtains the version build time.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row923031911093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p772494946093523">

GetBuildRootHash (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p48845147093523">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p535740538093523">

Obtains the buildroot hash value of this version.

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

GetAbiList()
------------

::

   char* GetAbiList (void )

**Description:**

Obtains the list of application binary interfaces (ABIs) supported on
this device.

The interfaces in the ABI list are separated by commas (,). This
function is available only for an OS with an ecosystem accommodating
native applications.

**Returns:**

Returns the ABI list if a result is found; returns **NULL** otherwise.
The return result is released by the caller.

GetBootloaderVersion()
----------------------

::

   char* GetBootloaderVersion (void )

**Description:**

Obtains the bootloader version of this device.

The bootloader version can have a maximum length of 64 characters.

**Returns:**

Returns the bootloader version if a result is found; returns **NULL**
otherwise. The return result is released by the caller.

GetBrand()
----------

::

   char* GetBrand (void )

**Description:**

Obtains the device brand.

The device brand can have a maximum length of 32 characters.

**Returns:**

Returns the device brand if a result is found; returns **NULL**
otherwise. The return result is released by the caller.

GetBuildHost()
--------------

::

   char* GetBuildHost (void )

**Description:**

Obtains the build host name.

The build host name can have a maximum length of 32 characters.

**Returns:**

Returns the build host name if a result is found; returns **NULL**
otherwise. The return result is released by the caller.

GetBuildRootHash()
------------------

::

   char* GetBuildRootHash (void )

**Description:**

Obtains the buildroot hash value of this version.

The buildroot hash value is represented by the root hash value in the
software version hash tree.

**Returns:**

Returns the buildroot hash value if a result is found; returns **NULL**
otherwise. The return result is released by the caller.

GetBuildTime()
--------------

::

   char* GetBuildTime (void )

**Description:**

Obtains the version build time.

The version build time is represented by the number of milliseconds
elapsed since 1970-01-01 00:00:00 GMT.

**Returns:**

Returns the version build time if a result is found; returns **NULL**
otherwise. The return result is released by the caller.

GetBuildType()
--------------

::

   char* GetBuildType (void )

**Description:**

Obtains the build type.

Different build types with the same baseline codes will be returned, for
example, **debug/release** and **log/nolog**. Multiple build types can
be separated by semicolons (;).

**Returns:**

Returns the build type if a result is found; returns **NULL** otherwise.
The return result is released by the caller.

GetBuildUser()
--------------

::

   char* GetBuildUser (void )

**Description:**

Obtains the build account user name.

The build account user name can have a maximum length of 32 characters.

**Returns:**

Returns the build account user name if a result is found; returns
**NULL** otherwise. The return result is released by the caller.

GetDisplayVersion()
-------------------

::

   char* GetDisplayVersion (void )

**Description:**

Obtains the software version visible to users.

The software version visible to users can have a maximum length of 64
characters.

**Returns:**

Returns the software version visible to users if a result is found;
returns **NULL** otherwise. The return result is released by the caller.

GetFirstApiLevel()
------------------

::

   char* GetFirstApiLevel (void )

**Description:**

Obtains the first SDK API level of the system software.

In general, the first SDK API level is an integer. This function is only
available for an OS with an ecosystem.

**Returns:**

Returns the first SDK API level if a result is found; returns **NULL**
otherwise. The return result is released by the caller.

GetHardwareModel()
------------------

::

   char* GetHardwareModel (void )

**Description:**

Obtains the device hardware model.

The device hardware model can have a maximum length of 32 characters.

**Returns:**

Returns the device hardware model if a result is found; returns **NULL**
otherwise. The return result is released by the caller.

GetHardwareProfile()
--------------------

::

   char* GetHardwareProfile (void )

**Description:**

Obtains the device hardware profile.

The device hardware profile is a string in JSON format and has a maximum
length of 1000 characters.

**Returns:**

Returns the device hardware profile if a result is found; returns
**NULL** otherwise. The return result is released by the caller. The
JSON field in the device hardware profile is defined as follows:

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1291834144093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1198703222093523">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1598493399093523">

key

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

   <tr id="row425125485093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1223746831093523">

Audio playback

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p53020346093523">

aout

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1385593769093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1994108726093523">

Display

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1999530869093523">

display

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row433524928093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1791147140093523">

Camera

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1606987096093523">

camera

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1054223029093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p427566820093523">

2D acceleration capability

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p436284920093523">

DMA_2D

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1460295583093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p513072201093523">

Random-access memory

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p765924691093523">

RAM

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row344349361093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p502868672093523">

Read-only memory

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1687315571093523">

ROM

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row750088250093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1302119573093523">

Graphics processing unit

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1528288179093523">

GPU

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1435473161093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p248894306093523">

Neural-network processing unit

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1284515491093523">

NPU

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row832412248093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2144244684093523">

Radio

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p964405780093523">

radio

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row984743211093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p461261962093523">

Bluetooth

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1747425900093523">

bluetooth

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1300941378093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p260486586093523">

Wi-Fi

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1601297181093523">

WIFI

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row251964019093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p929453925093523">

USB

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1818877276093523">

usbhost

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

GetIncrementalVersion()
-----------------------

::

   char* GetIncrementalVersion (void )

**Description:**

Obtains the incremental version.

The incremental version can be used as the unique software version when
the device model is the same.

**Returns:**

Returns the incremental version if a result is found; returns **NULL**
otherwise. The return result is released by the caller.

GetManufacture()
----------------

::

   char* GetManufacture (void )

**Description:**

Obtains the device manufacturer.

The device manufacturer can have a maximum length of 32 characters.

**Returns:**

Returns the device manufacturer if a result is found; returns **NULL**
otherwise. The return result is released by the caller.

GetMarketName()
---------------

::

   char* GetMarketName (void )

**Description:**

Obtains the device marketing name.

The device marketing name can have a maximum length of 32 characters.

**Returns:**

Returns the device marketing name if a result is found; returns **NULL**
otherwise. The return result is released by the caller.

GetOsName()
-----------

::

   char* GetOsName (void )

**Description:**

Obtains the operating system (OS) name.

The device OS name can have a maximum length of 32 characters.

**Returns:**

Returns the device OS name if a result is found; returns **NULL**
otherwise. The return result is released by the caller.

GetParameter()
--------------

::

   int GetParameter (const char * key, const char * def, char * value, unsigned int len )

**Description:**

Obtains a system parameter matching the specified **key**.

If no system parameter is found, the **def** parameter will be returned.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2144234814093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1189881401093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1722945605093523">

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

   <tr id="row336398849093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

key

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the key for the system parameter to query. The value can
contain lowercase letters, digits, underscores (_), and dots (.). Its
length cannot exceed 32 bytes (including the end-of-text character in
the string).

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row578196924093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

def

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the default value to return when no query result is found.
This parameter is specified by the caller.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row419733018093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

value

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the data buffer that stores the query result. This parameter
is applied for and released by the caller and can be used as an output
parameter.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row665063266093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

len

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the length of the data in the buffer.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the number of bytes of the system parameter if the operation is
successful; returns **-9** if a parameter is incorrect; returns **-1**
in other scenarios.

GetProductModel()
-----------------

::

   char* GetProductModel (void )

**Description:**

Obtains the device authentication model.

The device authentication model can have a maximum length of 32
characters.

**Returns:**

Returns the device authentication model if a result is found; returns
**NULL** otherwise. The return result is released by the caller.

GetProductSeries()
------------------

::

   char* GetProductSeries (void )

**Description:**

Obtains the device series name.

The device series name can have a maximum length of 32 characters.

**Returns:**

Returns the device series name if a result is found; returns **NULL**
otherwise. The return result is released by the caller.

GetProductType()
----------------

::

   char* GetProductType (void )

**Description:**

Obtains the device type.

The device type can have a maximum length of 32 characters.

**Returns:**

Returns the device type if a result is found, for example, returns
**wifiiot** if the application is running on a Wi-Fi connected IoT
device; returns **NULL** otherwise. The return result is released by the
caller.

GetSdkApiLevel()
----------------

::

   char* GetSdkApiLevel (void )

**Description:**

Obtains the SDK API level that matches the current system software.

In general, the SDK API level is an integer. This function is only
available for an OS with an ecosystem.

**Returns:**

Returns the SDK API level if a result is found; returns **NULL**
otherwise. The return result is released by the caller.

GetSecurityPatchTag()
---------------------

::

   char* GetSecurityPatchTag (void )

**Description:**

Obtains the security patch tag.

**Returns:**

Returns the security patch tag if a result is found; returns **NULL**
otherwise. The return result is released by the caller.

GetSerial()
-----------

::

   char* GetSerial (void )

**Description:**

Obtains the device serial number (SN).

The device SN can have a maximum length of 64 characters.

**Returns:**

Returns the device SN if a result is found; returns **NULL** otherwise.
The return result is released by the caller.

GetSoftwareModel()
------------------

::

   char* GetSoftwareModel (void )

**Description:**

Obtains the device software model.

The device software model can have a maximum length of 32 characters.

**Returns:**

Returns the device software model if a result is found; returns **NULL**
otherwise. The return result is released by the caller.

GetVersionId()
--------------

::

   char* GetVersionId (void )

**Description:**

Obtains the version ID.

The version ID can have a maximum length of 127 characters. It is the
unique identifier of a device.

**Returns:**

Returns the version ID if a result is found; returns **NULL** otherwise.
The return result is released by the caller.

SetParameter()
--------------

::

   int SetParameter (const char * key, const char * value )

**Description:**

Sets or updates a system parameter.

You can use this function to set a system parameter that matches **key**
as **value**.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row864910666093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p664293457093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p480218148093523">

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

   <tr id="row1532336283093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

key

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the key for the parameter to set or update. The value can
contain lowercase letters, digits, underscores (_), and dots (.). Its
length cannot exceed 32 bytes (including the end-of-text character in
the string).

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1056192134093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

value

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the system parameter value. Its length cannot exceed 128 bytes
(including the end-of-text character in the string).

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns **-9** if a
parameter is incorrect; returns **-1** in other scenarios.
