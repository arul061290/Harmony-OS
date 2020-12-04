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

   <tr id="row437280217090252">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1627314734090252">

File Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1632121223090252">

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

   <tr id="row1553965245090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p112308717090252">

parameter.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1897536787090252">

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

   <tr id="row1056578116090252">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2144263055090252">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1617293712090252">

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

   <tr id="row932810788090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1673483853090252">

GetParameter (const char *key, const char*\ def, char \*value, unsigned
int len)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1445408033090252">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p563029969090252">

Obtains a system parameter matching the specified key.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1307691396090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p275967121090252">

SetParameter (const char *key, const char*\ value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1847965871090252">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1314636322090252">

Sets or updates a system parameter.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row875057868090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p980767321090252">

GetProductType (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p816741169090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1137141307090252">

Obtains the device type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2125597950090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p297071298090252">

GetManufacture (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1603900349090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p171278431090252">

Obtains the device manufacturer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1213301020090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1812989726090252">

GetBrand (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1351424179090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1150029038090252">

Obtains the device brand.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row930271424090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1773961769090252">

GetMarketName (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p858479720090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1407675180090252">

Obtains the device marketing name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1617115083090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p8249725090252">

GetProductSeries (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p263334908090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p598326783090252">

Obtains the device series name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1548253674090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p319180026090252">

GetProductModel (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2068829317090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1112331969090252">

Obtains the device authentication model.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1126189852090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1140214174090252">

GetSoftwareModel (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1555905253090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1191363673090252">

Obtains the device software model.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1882596141090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1288969206090252">

GetHardwareModel (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1432923802090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1772836848090252">

Obtains the device hardware model.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row690207607090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p464631606090252">

GetHardwareProfile (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1567615925090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1770647288090252">

Obtains the device hardware profile.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1921065716090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2146142586090252">

GetSerial (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1541008822090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p967380808090252">

Obtains the device serial number (SN).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row97632552090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p251166277090252">

GetOsName (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1517299799090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p179755500090252">

Obtains the operating system (OS) name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1163407656090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p908273051090252">

GetDisplayVersion (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p410869132090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1482028887090252">

Obtains the software version visible to users.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1102365474090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p618281961090252">

GetBootloaderVersion (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p33171130090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p176769296090252">

Obtains the bootloader version of this device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1803411652090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p125951321090252">

GetSecurityPatchTag (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p98923128090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p356540229090252">

Obtains the security patch tag.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row734473816090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1881499344090252">

GetAbiList (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1708765549090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1394346758090252">

Obtains the list of application binary interfaces (ABIs) supported on
this device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2097795580090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p544547905090252">

GetSdkApiLevel (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1310202916090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p340307495090252">

Obtains the SDK API level that matches the current system software.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1052890058090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p101396792090252">

GetFirstApiLevel (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2045412838090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1772203570090252">

Obtains the first SDK API level of the system software.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1973808837090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1136483230090252">

GetIncrementalVersion (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1533064707090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1951676183090252">

Obtains the incremental version.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1304089105090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1213040213090252">

GetVersionId (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1211889955090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p532184115090252">

Obtains the version ID.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row40338864090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p718831451090252">

GetBuildType (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p630165623090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p63319430090252">

Obtains the build type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row349366819090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p23054045090252">

GetBuildUser (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1517873593090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1628275459090252">

Obtains the build account user name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1455188442090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p363217629090252">

GetBuildHost (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p550687274090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p517353253090252">

Obtains the build host name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row669453698090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2050649103090252">

GetBuildTime (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1305567139090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p605541122090252">

Obtains the version build time.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row128576920090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1965170219090252">

GetBuildRootHash (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1078368763090252">

char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1119240449090252">

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

   <tr id="row251905452090252">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1356788590090252">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p302066452090252">

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

   <tr id="row1486181137090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1776532344090252">

Audio playback

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1968408227090252">

aout

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2081194574090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1689077176090252">

Display

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p457706885090252">

display

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row583615648090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1643052035090252">

Camera

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p421849755090252">

camera

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1416597976090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2084083067090252">

2D acceleration capability

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1338441684090252">

DMA_2D

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1803250631090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1788250788090252">

Random-access memory

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1631115424090252">

RAM

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1632529803090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p53586633090252">

Read-only memory

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2073057916090252">

ROM

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row811605079090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p516762800090252">

Graphics processing unit

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1289628992090252">

GPU

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1797409692090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p654942734090252">

Neural-network processing unit

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2002883252090252">

NPU

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1771276335090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p560035848090252">

Radio

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1946739906090252">

radio

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1967561705090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p567131903090252">

Bluetooth

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p884801842090252">

bluetooth

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row452138850090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p667760162090252">

Wi-Fi

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1428558769090252">

WIFI

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1917986293090252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p783277336090252">

USB

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p806560836090252">

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

   <tr id="row1520922523090252">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p278326812090252">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1592749319090252">

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

   <tr id="row1271625395090252">

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

   <tr id="row1636069936090252">

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

   <tr id="row1082125015090252">

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

   <tr id="row871169891090252">

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

   <tr id="row1802993833090252">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p337024397090252">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1108121953090252">

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

   <tr id="row417866710090252">

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

   <tr id="row522818540090252">

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
