Startup
=======

Introduction
------------

The startup subsystem is responsible for starting key system processes
and services after the kernel is started and before applications are
started. This subsystem has the following modules:

-  **init** for starting system service processes

This module can be used on the Hi3516DV300 and Hi3518EV300 platforms
powered by LiteOS Cortex-A.

It starts system service processes from the time the kernel loads the
first user-space process to the time the first application program is
started. In addition to loading key system processes, the startup
subsystem needs to configure required permissions during the startup,
and keeps the specified process alive after sub-processes are started.
If a process exits abnormally, the startup subsystem needs to restart
it, and to perform system reset for a special process.

-  **appspawn** for spawning applications

   This module can be used on the Hi3516DV300 and Hi3518EV300 platforms
   powered by LiteOS Cortex-A.

   It spawns application processes upon receiving commands from the
   application framework, configures required permissions, and invokes
   the entry of the application framework.

-  **bootstrap** for starting service modules

   This module can be used on the Hi3861 platform powered by LiteOS
   Cortex-M.

   It provides identifiers for starting services and functions. When the
   SAMGR is started, the entry function identified by **boostrap** is
   invoked and system services are started.

-  **Syspara**

   This module can be used on the Hi3861, Hi3516DV300 and Hi3518EV300
   platforms powered by LiteOS Cortex-M and LiteOS Cortex-A.

   It obtains and sets system attributes for the operating system.

   System attributes consist of default, OEM-specified, and custom
   system attributes. OEM-specified system attributes provide only
   default values. The specific values need to be adjusted as required.
   For details, see `Usage <#section674513182447>`__.

Directory Structure
-------------------

**Table 1** Directory structure of the source code for the Startup
subsystem

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row7977610131417">

.. raw:: html

   <th class="cellrowborder" valign="top" width="19.439999999999998%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p18792459121314">

Directory

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="66.64%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p77921459191317">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="13.919999999999998%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p101617019356">

Applicable Platform

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

   <tr id="row17977171010144">

.. raw:: html

   <td class="cellrowborder" valign="top" width="19.439999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2793159171311">

base/startup/services/appspawn_lite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="66.64%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p879375920132">

appspawn module for spawning application processes. It receives AMS
messages via lightweight IPC, parses the messages, starts application
processes based on the parsing result, and grants permissions to them.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="13.919999999999998%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p63463619360">

Hi3516DV300

.. raw:: html

   </p>

.. raw:: html

   <p id="p141611802359">

Hi3518EV300

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row6978161091412">

.. raw:: html

   <td class="cellrowborder" valign="top" width="19.439999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p37931659101311">

base/startup/services/bootstrap_lite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="66.64%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p6793059171318">

bootstrap module for starting all services except core system services.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="13.919999999999998%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p101610019353">

Hi3861

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row6978201031415">

.. raw:: html

   <td class="cellrowborder" align="left" valign="top" width="19.439999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p117935599130">

base/startup/services/init_lite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="66.64%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p0793185971316">

init module for the init process, which is the first user-space process
loaded after the kernel is initialized. After the startup, the
configuration file in /etc/init.cfg is parsed. Based on the parsing
result, other key system processes are started and granted required
permissions.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="13.919999999999998%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2176757193619">

Hi3516DV300

.. raw:: html

   </p>

.. raw:: html

   <p id="p51611013358">

Hi3518EV300

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1897841071415">

.. raw:: html

   <td class="cellrowborder" valign="top" width="19.439999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p16793185961315">

base/startup/interfaces

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="66.64%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p20413161014013">

Open APIs provided by the bootstrap module. The main function directs
the calls to these APIs to start the service framework.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="13.919999999999998%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1956516512380">

Hi3861

.. raw:: html

   </p>

.. raw:: html

   <p id="p2670195353812">

Hi3516DV300

.. raw:: html

   </p>

.. raw:: html

   <p id="p116118053518">

Hi3518EV300

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row178841725886">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p88841825887">

base/startup/frameworks/syspara_lite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p98851625589">

syspara module. It provides APIs to obtain device information, including
the product name, brand name, category name, and manufacturer name.

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

::

   base
   ├──startup    Root directory of the startup subsystem
   ├──── frameworks
   │     └── syspara_lite
   │         ├── LICENSE     License file for open-source code
   │         ├── parameter   Source files for the syspara module
   │         │   ├── BUILD.gn
   │         │   └── src
   │         │       ├── BUILD.gn
   │         │       ├── param_impl_hal     syspara module implemented based on LiteOS Cortex-M
   │         │       └── param_impl_posix   syspara module implemented based on LiteOS Cortex-A
   │         └── token
   │             ├── BUILD.gn
   │             └── src
   │                 ├── token_impl_hal
   │                 └── token_impl_posix
   ├──── hals         
   │     └── syspara_lite       Header files at the hardware abstraction layer of the syspara module
   ├──── interfaces
   │     └── kits
   │         └── syspara_lite   Open APIs related to the syspara module
   └──── services
         ├── appspawn_lite    appspawn module
         │   ├── BUILD.gn    Compilation and configuration of the appspawn module
         │   ├── include     Header files for the appspawn module
         │   ├── LICENSE     License file for open-source code
         │   ├── moduletest  Self-testing code for the appspawn module
         │   └── src         Source files for the appspawn module
         ├── bootstrap_lite   bootstrap module
         │   ├── BUILD.gn    Compilation and configuration of the bootstrap module
         │   ├── LICENSE     License file for open-source code
         │   └── source      Source files for the bootstrap module
         └── init_lite       init module
              ├── BUILD.gn    Compilation and configuration of the init module
             ├── include     Header files for the init module
             ├── LICENSE     License file for open-source code
             ├── moduletest  Self-testing code for the init module
             └── src         Sources for the init module
   vendor
   └──huawei
           └──camera
                   └──init_configs  Configuration file of the init module (in JSON format, in the /etc/ directory)

Constraints
-----------

-  The startup subsystem is developed using the C language.
-  OEM-specified system attributes provide only default values. The
   specific values need to be adjusted as required.

Usage
-----

-  Configuration file of the init module

The configuration file **init.cfg** of the **init** module contains
service names, executable file paths, permissions, and other attributes
of all key system services that need to be started by the init process.
The file is stored in **/vendor/huawei/camera/init_configs/** under
**/etc/**. It is in JSON format, and its size cannot exceed 100 KB.

After the init process starts, it reads the **/etc/init.cfg** file,
parses the JSON content, and loads system services in sequence based on
the parsing result. The format and content of the configuration file are
described as follows:

::

   {
       "jobs" : [{
               "name" : "pre-init",      -------- Job executed before the initialization. It can be used to store some pre-operations (for example, creating a folder) before the init process is started.
               "cmds" : [
                    "mkdir /testdir",      -------- Command for creating a folder. mkdir and the target folder must be separated by only one space.
                   "chmod 0700 /testdir", -------- Command for modifying the permission, which must be in the 0xxxx format. chmod, permission, and the target folder must be separated by only one space.
                   "chown 99 99 /testdir",-------- Command for modifying the owner group. chown, UID, GID, and the target folder must be separated by only one space.
                   "mkdir /testdir2",
                   "mount vfat /dev/mmcblk0p0 /testdir2 noexec nosuid" -------- mount command in the following format: mount file system type source target flags data
                                                                       -------- flags currently supports only nodev, noexec, nosuid, and rdonly, which are separated by a space.
               ]
           }, {
               "name" : "init",          -------- Job name supported by the init process. Ensure that an extended job name contains a maximum of 32 bytes.
               "cmds" : [                -------- Command set supported by the current job. Only one space is allowed between the command name (less than 10 bytes) and the following parameter (less than 32 bytes).
                   "start service1",     -------- First command of the current job
                   "start service2"      -------- Second command of the current job (You can adjust the sequence of commands in the array as required. The init process executes the commands in the same order as they are parsed.)
                ]
           }, {
                "name" : "post-init",    -------- Job executed after the initialization. It can be used to store some operations performed after the init process is started.
                "cmds" : []
           }
       ],
       "services" : [{                         -------- service set (in an array), including all system services that need to be started by the init process
               "name" : "service1",            -------- Name of the current service. A maximum of 32 bytes must be specified for the name.
               "path" : "/bin/process1"        -------- Full path of the executable file of the current service. A maximum of 64 bytes must be specified for the path.
               "uid" : 1,                      -------- UID of the current service process
               "gid" : 1,                      -------- GID of the current service process
               "once" : 0,                     -------- Whether the current service process is a one-off process
                                                        0 --- The current service process is not a one-off process. If the process exits due to any reason, the init module restarts the service process upon receiving the SIGCHLD signal.
                                                      non-0 --- The current service is a one-off process. If the process exits due to any reason, the init module does not restart the service process.
               "importance" : 1,               -------- Whether the current service is a key system process
                                                        0 --- The current service is not a key system process. If the process exits due to any reason, the init module does not reset the system.
                                                      non-0 --- The current service is a key system process. If the process exits due to any reason, the init module resets and restarts the system upon receiving the SIGCHLD signal.
               "caps" : [0, 1, 2, 5]           -------- Capabilities required by the current service. They are evaluated based on the capabilities supported by the security subsystem and configured in accordance with the principle of least permission.
       }, {
               "name" : "service2",            -------- Next service that needs to be started by the init module. The service sequence is irrelevant to the startup sequence, which is determined by the cmd sequence in the previous job.
               "path" : "/bin/process2",
               "uid" : 2,
               "gid" : 2,
               "once" : 1,
               "importance" : 0,
               "caps" : [ ]
           }
       ]
   }

**Table 2** Supported commands

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row5623144194017">

.. raw:: html

   <th class="cellrowborder" valign="top" width="12.5%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p56231449404">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="31.05%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p962313447401">

Syntax

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="56.45%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p88724434113">

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

   <tr id="row962344416405">

.. raw:: html

   <td class="cellrowborder" valign="top" width="12.5%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p66231144104011">

start

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="31.05%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p9607551369">

start ServiceName

.. raw:: html

   </p>

.. raw:: html

   <p id="p862384484010">

Only one space is allowed.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="56.45%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p17872104184113">

Starts a service. The service name must be the same as that in the
services array in the file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row962311443404">

.. raw:: html

   <td class="cellrowborder" valign="top" width="12.5%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p13837142094117">

mkdir

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="31.05%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p637613010714">

mkdir /xxxx/xxx

.. raw:: html

   </p>

.. raw:: html

   <p id="p2624244204019">

Only one space is allowed.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="56.45%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p158722484112">

Creates a directory.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row662404414406">

.. raw:: html

   <td class="cellrowborder" valign="top" width="12.5%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p3624444154011">

chmod

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="31.05%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p68331741271">

chmod 0xxx /xxx/xx

.. raw:: html

   </p>

.. raw:: html

   <p id="p7624344134020">

Only one space is allowed.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="56.45%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p18872945418">

Changes the permission. The permission value must be in 0xxx format, for
example, 0755 and 0600. This configuration must comply with the
principle of least permission.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1462404494017">

.. raw:: html

   <td class="cellrowborder" valign="top" width="12.5%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p136241144144013">

chown

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="31.05%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p84976100714">

chown uid gid /xxx/xx

.. raw:: html

   </p>

.. raw:: html

   <p id="p1624144194011">

Only one space is allowed.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="56.45%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p9872246417">

Changes the owner group.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1285512468412">

.. raw:: html

   <td class="cellrowborder" valign="top" width="12.5%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1385515468413">

mount

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="31.05%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p358535124815">

mount fileSysType source target flags data

.. raw:: html

   </p>

.. raw:: html

   <p id="p178550463412">

Only one space is allowed.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="56.45%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1085544611415">

Mounts data. Currently, flags supports only nodev, noexec, nosuid, and
rdonly, and other strings are considered as data.

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

It is worth noting that the modified **init.cfg** file must be in JSON
format. Otherwise, the init process fails to parse the file, and no
service will be started. The configured service permission
**uid/gid/capability** must meet the requirements imposed by the
security subsystem and comply with the principle of least permission. In
addition, if the values of **once** and **importance** of a service are
both **0** and the service exits for more than four consecutive times
within four minutes, the init process will stop restarting the service.

-  System parameters

   -  OEM-specific system attributes

   For Hi3516DV300 and Hi3518EV300 development boards, you need to
   modify the source files in the
   **vendor/huawei/camera/hals/utils/sys_param** directory.

   ::

      static const char HOS_PRODUCT_TYPE[] = {"****"};
      static const char HOS_MANUFACTURE[] = {"****"};
      static const char HOS_BRAND[] = {"****"};
      static const char HOS_MARKET_NAME[] = {"****"};
      static const char HOS_PRODUCT_SERIES[] = {"****"};
      static const char HOS_PRODUCT_MODEL[] = {"****"};
      static const char HOS_SOFTWARE_MODEL[] = {"****"};
      static const char HOS_HARDWARE_MODEL[] = {"****"};
      static const char HOS_HARDWARE_PROFILE[] = {"aout:true,display:true"};
      static const char HOS_BOOTLOADER_VERSION[] = {"bootloader"};
      static const char HOS_SECURE_PATCH_LEVEL[] = {"2020-6-5"};
      static const char HOS_ABI_LIST[] = {"****"};

   For Hi3861 development boards, you need to modify the source files in
   the **vendor/huawei/wifi-iot/hals/utils/sys_param** directory.

   ::

      static const char HOS_PRODUCT_TYPE[] = {"****"};
      static const char HOS_MANUFACTURE[] = {"****"};
      static const char HOS_BRAND[] = {"****"};
      static const char HOS_MARKET_NAME[] = {"****"};
      static const char HOS_PRODUCT_SERIES[] = {"****"};
      static const char HOS_PRODUCT_MODEL[] = {"****"};
      static const char HOS_SOFTWARE_MODEL[] = {"****"};
      static const char HOS_HARDWARE_MODEL[] = {"****"};
      static const char HOS_HARDWARE_PROFILE[] = {"aout:true,display:true"};
      static const char HOS_BOOTLOADER_VERSION[] = {"bootloader"};
      static const char HOS_SECURE_PATCH_LEVEL[] = {"2020-6-5"};
      static const char HOS_ABI_LIST[] = {"****"};

   -  Obtaining default system attributes

   ::

      char* value1 = GetProductType();
      printf("Product type =%s\n", value1);
      free(value1);
      char* value2 = GetManufacture();
      printf("Manufacture =%s\n", value2);
      free(value2);
      char* value3 = GetBrand();
      printf("GetBrand =%s\n", value3);
      free(value3);

   -  Obtaining custom system attributes

   ::

      const char* defSysParam = "data of sys param ***...";
      char key[] = "rw.parameter.key";
      char value[] = "OEM-hisi-10.1.0";
      int ret = SetParameter(key, value);
      char valueGet[128] = {0};
      ret = GetParameter(key, defSysParam, valueGet, 128);
      printf("value = %s\n", valueGet);

Repositories Involved
---------------------

startup_frameworks_syspara_lite

startup_hals_syspara_lite

startup_interfaces_kits_syspara_lite

startup_appspawn_lite

startup_services_bootstrap_lite

startup_init_lite
