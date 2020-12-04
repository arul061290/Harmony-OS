DFX
===

Introduction
------------

This repository is used to store the code of Design for X (DFX)
frameworks, including Design for Reliability (DFR) and Design for
Testability (DFT).

As chip resources are limited and hardware platforms are diversified,
component-based and customizable DFX frameworks need to be provided for
different hardware architectures and resources. Two types of lightweight
DFX frameworks (mini and featured) are available for hardware platforms
powered by RISC-V, Cortex-M, and Cortex-A.

-  mini: This framework is intended for hardware platforms with Cortex-M
   or equivalent processing capabilities. The system memory is generally
   less than 512 KB. There is only one lightweight file system that can
   be used in limited scenarios, or no file system at all. The mini
   framework complies with the Cortex Microcontroller Software Interface
   Standard (CMSIS).

-  featured: This framework is intended for hardware platforms with
   Cortex-A or equivalent processing capabilities. The system memory is
   generally greater than 512 KB. There is a comprehensive file system
   for storing a large amount of data. The featured framework complies
   with the Portable Operating System Interface (POSIX) specifications.

Directory Structure
-------------------

**Table 1** Directory structure of the source code for lightweight DFX

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row7977610131417">

.. raw:: html

   <th class="cellrowborder" valign="top" width="30.34%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p18792459121314">

Directory

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="69.66%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p77921459191317">

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

   <tr id="row17977171010144">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p2793159171311">

interface

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p879375920132">

Stores all header files for open APIs.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row259142201312">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p5197366257">

interfaces/kits/hilog

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p10406450131319">

Defines open APIs available for logs in the featured framework.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row580915918401">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p9809189144014">

interfaces/kits/hilog_lite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p168101694401">

Defines open APIs available for logs in the mini framework.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1188919458130">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p14561174816401">

interfaces/innerkits/hievent_lite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1254413131146">

Defines open APIs available for event printing in the mini framework.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row6978161091412">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p37931659101311">

services/hilogcat_lite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p6793059171318">

Stores services and commands related to logs.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row6978201031415">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1738210441049">

services/hilogcat_lite/apphilogcat

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1629020401941">

Provides the log flushing to disk service in the featured framework.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1596814581415">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p158313363613">

services/hilogcat_lite/command

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p12969358749">

Provides DFX commands specific to the mini framework.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row175618551244">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p73791172718">

services/hilogcat_lite/hilogcat

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p107568558416">

Provides commands to output logs in the featured framework.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row11587111583">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p4491153104614">

services/hiview_lite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p159210361388">

Registers the DFX service specific to the mini framework.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row144311669479">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p443219624716">

frameworks/ddrdump_lite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p343218604718">

Dumps Double Data Rate (DDR) memory in the mini framework.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1125881215472">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p52581712124718">

frameworks/hievent_lite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1825921284710">

Records event printing in the DFX-mini framework.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row13101195476">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1210117994714">

frameworks/hilog_lite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p910159144719">

Defines APIs for logging.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2442416175011">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p14911117105011">

frameworks/hilog_lite/featured

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p18491171775019">

Defines APIs for logging in the featured framework.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row481417116116">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p468592018492">

frameworks/hilog_lite/mini

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p2051115253494">

Defines APIs for logging in the mini framework.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row13247163492">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p710851611910">

utils/lite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p112471431895">

Stores utils. It contains the configuration items of the mini framework.

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

The overall code of the mini framework is developed based on the C
standard library.

Usage (mini Framework)
----------------------

The mini framework is a simple and compact DFX design that provides the
logging function.

-  **The following takes Module A as an example to describe how to add a
   module and print logs.**

   1. **Step 1: Add the module ID.**

      Define **HILOG_MODULE_A** in **HiLogModuleDef** of
      **interfaces/kits/hilog_lite/hiview_log.h**.

      ::

         typedef enum {
             /** DFX */    
             HILOG_MODULE_HIVIEW = 0,    
             /** System Module A */    
             HILOG_MODULE_A,    
             /** Maximum number of modules */
             HILOG_MODULE_MAX
         } HiLogModuleType;

   2. **Step 2: Register the module.**

      Add the following code to the initialization process of Module A
      to register it with the logging framework:

      ::

         HiLogRegisterModule(HILOG_MODULE_A, "A");

   3. **Step 3: Modify the static configuration of the DFX framework.**

      Modify **g_hiviewConfig** in the following file as required (By
      default, modification is not required and logs are output to the
      serial port):

      ::

         utils/lite/hiview_config.c

      .. raw:: html

         <table>

      .. raw:: html

         <thead align="left">

      .. raw:: html

         <tr id="row07061028154510">

      .. raw:: html

         <th class="cellrowborder" valign="top" width="25.180000000000003%" id="mcps1.1.3.1.1">

      .. raw:: html

         <p id="p10706128184514">

      Configuration Item

      .. raw:: html

         </p>

      .. raw:: html

         </th>

      .. raw:: html

         <th class="cellrowborder" valign="top" width="74.82%" id="mcps1.1.3.1.2">

      .. raw:: html

         <p id="p11706928194520">

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

         <tr id="row8706828154511">

      .. raw:: html

         <td class="cellrowborder" valign="top" width="25.180000000000003%" headers="mcps1.1.3.1.1 ">

      .. raw:: html

         <p id="p19706112824514">

      outputOption

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         <td class="cellrowborder" valign="top" width="74.82%" headers="mcps1.1.3.1.2 ">

      .. raw:: html

         <p id="p9706528104512">

      Log output mode. The value can be:

      .. raw:: html

         </p>

      .. raw:: html

         <p id="p107061428124515">

      OUTPUT_OPTION_DEBUG: Logs are directly output to the serial port
      without cross-task scheduling. This value is used only for
      temporary debugging.

      .. raw:: html

         </p>

      .. raw:: html

         <p id="p870682819450">

      OUTPUT_OPTION_FLOW (default value): Logs are output as data flow
      to the serial port.

      .. raw:: html

         </p>

      .. raw:: html

         <p id="p16707182819454">

      OUTPUT_OPTION_TEXT_FILE: Logs are output as text files.

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         </tr>

      .. raw:: html

         <tr id="row1270720281453">

      .. raw:: html

         <td class="cellrowborder" valign="top" width="25.180000000000003%" headers="mcps1.1.3.1.1 ">

      .. raw:: html

         <p id="p137071528164516">

      level

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         <td class="cellrowborder" valign="top" width="74.82%" headers="mcps1.1.3.1.2 ">

      .. raw:: html

         <p id="p177071428154510">

      Log level for output. Only the logs whose levels are higher than
      or equal to the level specified by this parameter can be output.
      The value can be:

      .. raw:: html

         </p>

      .. raw:: html

         <p id="p1470712824515">

      HILOG_LV_DEBUG, HILOG_LV_INFO, HILOG_LV_WARN, HILOG_LV_ERROR, or
      HILOG_LV_FATAL

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         </tr>

      .. raw:: html

         <tr id="row17707142814513">

      .. raw:: html

         <td class="cellrowborder" valign="top" width="25.180000000000003%" headers="mcps1.1.3.1.1 ">

      .. raw:: html

         <p id="p11707192814517">

      logSwitch

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         <td class="cellrowborder" valign="top" width="74.82%" headers="mcps1.1.3.1.2 ">

      .. raw:: html

         <p id="p870711281452">

      Logging switch. The log component can be successfully initialized
      even if this switch is turned off before compilation. By default,
      this switch is turned on. The value can be:

      .. raw:: html

         </p>

      .. raw:: html

         <p id="p1570822810456">

      HIVIEW_FEATURE_ON or HIVIEW_FEATURE_OFF

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         </tr>

      .. raw:: html

         <tr id="row6708132813453">

      .. raw:: html

         <td class="cellrowborder" valign="top" width="25.180000000000003%" headers="mcps1.1.3.1.1 ">

      .. raw:: html

         <p id="p1570813280453">

      dumpSwitch

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         <td class="cellrowborder" valign="top" width="74.82%" headers="mcps1.1.3.1.2 ">

      .. raw:: html

         <p id="p970852810459">

      Dumping switch. If this switch is turned off before compilation,
      the DUMP component will not be initialized. By default, this
      switch is turned off. The value can be:

      .. raw:: html

         </p>

      .. raw:: html

         <p id="p147081328174519">

      HIVIEW_FEATURE_ON or HIVIEW_FEATURE_OFF

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         </tr>

      .. raw:: html

         <tr id="row87081282452">

      .. raw:: html

         <td class="cellrowborder" valign="top" width="25.180000000000003%" headers="mcps1.1.3.1.1 ">

      .. raw:: html

         <p id="p11708128124511">

      eventSwitch

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         <td class="cellrowborder" valign="top" width="74.82%" headers="mcps1.1.3.1.2 ">

      .. raw:: html

         <p id="p17708202834519">

      Event output switch. If this switch is turned off before
      compilation, the Event component will not be initialized. By
      default, this switch is turned off. The value can be:

      .. raw:: html

         </p>

      .. raw:: html

         <p id="p1670852894513">

      HIVIEW_FEATURE_ON or HIVIEW_FEATURE_OFF

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

   4. **Step 4: Print logs.**

      Include **#include “log.h”** in the **.c** file where logs need to
      be printed, call the following function:

      HILOG_INFO(HILOG_MODULE_A, “log test: %d”, 88);

      Parameter description:

      .. raw:: html

         <table>

      .. raw:: html

         <thead align="left">

      .. raw:: html

         <tr id="row1350818135519">

      .. raw:: html

         <th class="cellrowborder" valign="top" width="11.57%" id="mcps1.1.5.1.1">

      .. raw:: html

         <p id="p175031855513">

      Parameter

      .. raw:: html

         </p>

      .. raw:: html

         </th>

      .. raw:: html

         <th class="cellrowborder" valign="top" width="11.83%" id="mcps1.1.5.1.2">

      .. raw:: html

         <p id="p250131825511">

      Mandatory

      .. raw:: html

         </p>

      .. raw:: html

         </th>

      .. raw:: html

         <th class="cellrowborder" valign="top" width="15.21%" id="mcps1.1.5.1.3">

      .. raw:: html

         <p id="p3501418175516">

      Data Type

      .. raw:: html

         </p>

      .. raw:: html

         </th>

      .. raw:: html

         <th class="cellrowborder" valign="top" width="61.39%" id="mcps1.1.5.1.4">

      .. raw:: html

         <p id="p12501718125512">

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

         <tr id="row195016185559">

      .. raw:: html

         <td class="cellrowborder" valign="top" width="11.57%" headers="mcps1.1.5.1.1 ">

      .. raw:: html

         <p id="p6503180557">

      mod

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         <td class="cellrowborder" valign="top" width="11.83%" headers="mcps1.1.5.1.2 ">

      .. raw:: html

         <p id="p45061835518">

      Yes

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         <td class="cellrowborder" valign="top" width="15.21%" headers="mcps1.1.5.1.3 ">

      .. raw:: html

         <p id="p1050618155511">

      uint8

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         <td class="cellrowborder" valign="top" width="61.39%" headers="mcps1.1.5.1.4 ">

      .. raw:: html

         <p id="p1051618115519">

      Module or service ID.

      .. raw:: html

         </p>

      .. raw:: html

         <p id="p2511918165511">

      IDs are planned and allocated in a unified manner. A maximum of 64
      IDs are supported. Third-party applications use HILOG_MODULE_APP
      as their module ID.

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         </tr>

      .. raw:: html

         <tr id="row451818105516">

      .. raw:: html

         <td class="cellrowborder" valign="top" width="11.57%" headers="mcps1.1.5.1.1 ">

      .. raw:: html

         <p id="p15151845520">

      fmt

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         <td class="cellrowborder" valign="top" width="11.83%" headers="mcps1.1.5.1.2 ">

      .. raw:: html

         <p id="p251111817557">

      Yes

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         <td class="cellrowborder" valign="top" width="15.21%" headers="mcps1.1.5.1.3 ">

      .. raw:: html

         <p id="p1351151814555">

      char \*

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         <td class="cellrowborder" valign="top" width="61.39%" headers="mcps1.1.5.1.4 ">

      .. raw:: html

         <p id="p95117189556">

      Format specifier for output.

      .. raw:: html

         </p>

      .. raw:: html

         <p id="p25171895512">

      1. A maximum of six variable parameters are supported. %s is not
      supported.

      .. raw:: html

         </p>

      .. raw:: html

         <p id="p351181875510">

      2. The maximum length of a formatted log record is 128 bytes. If
      the length of a log exceeds 128 bytes, the log cannot be printed.

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         </tr>

      .. raw:: html

         <tr id="row95213183550">

      .. raw:: html

         <td class="cellrowborder" valign="top" width="11.57%" headers="mcps1.1.5.1.1 ">

      .. raw:: html

         <p id="p15291815518">

      Variable parameters

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         <td class="cellrowborder" valign="top" width="11.83%" headers="mcps1.1.5.1.2 ">

      .. raw:: html

         <p id="p1852151815514">

      No

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         <td class="cellrowborder" valign="top" width="15.21%" headers="mcps1.1.5.1.3 ">

      .. raw:: html

         <p id="p145221855520">

      int32

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         <td class="cellrowborder" valign="top" width="61.39%" headers="mcps1.1.5.1.4 ">

      .. raw:: html

         <p id="p15521018115510">

      Only numeric types are supported. A maximum of six variable
      parameters are allowed.

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

Usage (featured Framework)
--------------------------

The featured framework provides comprehensive DFX features and logging
APIs.

**Native C/C++** APIs

Available hilog APIs:

::

   HILOG_DEBUG(type, ...)
   HILOG_INFO(type, ...)
   HILOG_WARN(type, ...)
   HILOG_ERROR(type, ...)
   HILOG_FATAL(type, ...)

Usage guidelines:

1. Define the log tag.

2. Perform local debugging. (The domain value **0** can be used.)

3. Include the header file: #include <hilog/log.h>

4. Add the dependent library **libhilog** to **BUILD.gn**.

API rules:

1. The format specifier is labeled public by default, for example,
   **HILOGI(“Hello World\n”); >> Hello World**.

2. The formatted parameter is labeled private by default, for example,
   **HILOGI(“Age is %d\n”, 10); >> Age is <private>**.

3. Parameters labeled **%{private}** are private data, for example,
   **HILOGI(“Age is %{private}d\n”, 10); >> Age is <private>**.

4. Parameters labeled **%{public}** are public data, for example,
   **HILOGI(“Age is %{public}d\n”, 10); >>Age is 10**.

Parameter description:

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row72672598321">

.. raw:: html

   <th class="cellrowborder" valign="top" width="25.94%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1226718595323">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="74.06%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1026765918324">

Description:

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

   <tr id="row152675592321">

.. raw:: html

   <td class="cellrowborder" valign="top" width="25.94%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p12267135915328">

domain

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="74.06%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1826745953219">

Domain ID

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row20267135963212">

.. raw:: html

   <td class="cellrowborder" valign="top" width="25.94%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p152675591328">

tag

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="74.06%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p4267145920323">

Log tag

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row02671159203214">

.. raw:: html

   <td class="cellrowborder" valign="top" width="25.94%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1926785953216">

isFmtPrivate

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="74.06%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p326785963220">

Whether the format specifier is private

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row326795910325">

.. raw:: html

   <td class="cellrowborder" valign="top" width="25.94%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p72678597327">

fmt

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="74.06%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p11267195914324">

Format specifier

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1226825913326">

.. raw:: html

   <td class="cellrowborder" valign="top" width="25.94%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p142681259203215">

args

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="74.06%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1326895911325">

Parameters to be displayed using the format specifier

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

**Viewing logs**

1. Go to the **/storage/data/log/** directory to view hilog logs for
   debugging purpose.

2. Run the **hilogcat** command to view hilog logs in real time.

**Logging system architecture**

|image1|

1. hilogtask: kernel task for logging

   -  This is a task or thread of the Linux kernel. It is initialized
      during system startup.
   -  When a module in the kernel calls its logging API, it transfers
      the formatted log content to the task and stores it in a
      ringbuffer.
   -  When the logging API is called in user space, the formatted log
      content is written into the driver node by calling **ioctl**. The
      driver node then sends the log content to hilogtask, and hilogtask
      stores the log content in the ringbuffer.

2. hilogcatd: storing logs in user space

   -  This is a user-space process. It periodically reads the log
      content from the ringbuffer and stores it in the log file.
   -  Log files can be compressed in **gzip** format by using **zlib**.
   -  The size of a single file and the number of files can be
      configured during compilation.

3. hilogcat: command line tool for viewing logs

   This tool reads the content in the ringbuffer content via the kernel
   driver API, and then outputs the content to **stdout**.

4. ringbuffer: configurable

   -  The ringbuffer size can be configured during compilation.

Repositories Involved
---------------------

hiviewdfx_frameworks_hievent_lite

hiviewdfx_frameworks_ddrdump_lite

hiviewdfx_frameworks_hilog_lite

hiviewdfx_interfaces_innerkits_hilog

hiviewdfx_interfaces_innerkits_hievent_lite

hiviewdfx_interfaces_kits_hilog

hiviewdfx_interfaces_kits_hilog_lite

hiviewdfx_services_hiview_lite

hiviewdfx_services_hilogcat_lite

hiviewdfx_utils_lite

.. |image1| image:: figures/en-us_image_0000001054762887.png
