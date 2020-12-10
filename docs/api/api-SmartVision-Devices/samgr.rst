Samgr
=====

**Overview**\ 
--------------

Manages system capabilities.

This module provides the development framework base of the
service-oriented architecture (SOA). You can develop your own abilities
based on the Samgr development framework. This module provides basic
models of services, features, and functions, and registration and
discovery capabilities.

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

   <tr id="row1087012152084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p84099068084827">

File Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1837641440084827">

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

   <tr id="row1713691753084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2066576351084827">

common.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p314736075084827">

Provides common objects and functions for Samgr and external modules.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1754271254084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1643812094084827">

feature.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p433535044084827">

Defines the base class of a feature.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row865625999084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1197777375084827">

iunknown.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p975947673084827">

Provides the base class and default implementation for external
functions of system capabilities.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1874096405084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1289428444084827">

message.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p268754356084827">

Provides message communication APIs that help you to implement
asynchronous functions of IUnknown.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1625120694084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1149759562084827">

samgr_lite.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p489325550084827">

Manages system capabilities.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1096435911084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1331908262084827">

service.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1585358557084827">

Provides basic types and constants of services.

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

   <tr id="row1698546300084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1745980117084827">

Data Structure Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2048833202084827">

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

   <tr id="row1023732016084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1116587178084827">

SimpleVector

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p153640798084827">

Defines the simplified vector class, which is extended by four elements.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row711993890084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p666731011084827">

Feature

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1884737924084827">

Defines the base class of a feature.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row195347723084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1908407212084827">

IUnknown

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p866110407084827">

Defines the IUnknown class.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row988905304084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p376570300084827">

IUnknownEntry

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1995337922084827">

Defines the IUnknown implementation class.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row683501105084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1168452740084827">

Identity

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p262697980084827">

Identifies a service and feature.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row928744412084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p905685358084827">

Request

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1479556180084827">

Defines a request.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1108606448084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1771956533084827">

Response

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p115748867084827">

Defines a response.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1463987609084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1160332745084827">

SamgrLite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p829381634084827">

Represents the system ability management class.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row288517771084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1587397443084827">

TaskConfig

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1407148805084827">

Defines task configurations for a service.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1921229624084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2017029999084827">

Service

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p967484135084827">

Indicates the basic type of a service.

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

Macros
------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row192672235084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p627420659084827">

Macro Name and Value

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p509104918084827">

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

   <tr id="row1082939270084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1509390940084827">

GET_OFFSIZE(T, member) (long)((char *)&(((T*)(0))->member))

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1684394854084827">

Calculates the offset of the member in the T type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row95827344084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2092111564084827">

INHERIT_FEATURE

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p106908795084827">

Inherits from the macro of the feature class.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1200693528084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p685816324084827">

DEFAULT_VERSION 0x20

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1600697705084827">

Defines the default IUnknown version. You can customize the version.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row909047461084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1662386054084827">

INHERIT_IUNKNOWN

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1098342477084827">

Defines the macro for inheriting the IUnknown interface.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1145592201084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1172399949084827">

INHERIT_IUNKNOWNENTRY(T)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1117728441084827">

Defines the macro for inheriting the classes that implement the IUnknown
interface.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1454447143084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1703528301084827">

DEFAULT_IUNKNOWN_IMPL

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p557254105084827">

Defines the default marco for initializing the IUnknown interface.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1588891837084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1107047548084827">

IUNKNOWN_ENTRY_BEGIN(version)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p973308134084827">

Defines the macro for initializing the classes that implement the
IUnknown interface.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row549404123084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p331862266084827">

IUNKNOWN_ENTRY_END }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p947806832084827">

IUnknown Defines the end macro for initializing the IUnknown
implementation object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row998359490084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1102108245084827">

GET_IUNKNOWN(T) (IUnknown \*)(&((T).iUnknown))

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p401512978084827">

Obtains the pointer of the IUnknown interface object from the subclass
object T (generic macro) of the IUnknown implementation class.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row882611732084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1519401640084827">

BOOTSTRAP_SERVICE “Bootstrap”

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1012846381084827">

Starts a bootstrap service, which is used by samgr and implemented by
system service developers.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1285116967084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1723087974084827">

INHERIT_SERVICE

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p65663916084827">

Indicates the macro used to inherit the members from the service class.

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

   <tr id="row2029678779084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p216805329084827">

Typedef Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1354420624084827">

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

   <tr id="row817170725084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p614836901084827">

Vector

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p327587993084827">

typedef struct SimpleVector

.. raw:: html

   </p>

.. raw:: html

   <p id="p1991510650084827">

Defines the simplified vector class, which is extended by four elements.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row965708970084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1610578805084827">

IUnknownEntry

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p359905373084827">

typedef struct IUnknownEntry

.. raw:: html

   </p>

.. raw:: html

   <p id="p675232559084827">

Defines the IUnknown implementation class.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1564921056084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p823341877084827">

Handler) (const Request *request, const Response*\ response)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p415707742084827">

typedef void(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1306959744084827">

Handles asynchronous responses.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row22309771084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p828594437084827">

BootMessage

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1374165009084827">

typedef enum BootMessage

.. raw:: html

   </p>

.. raw:: html

   <p id="p1555042967084827">

Enumerates the IDs of the message to be processed for starting the
bootstrap service.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row211431122084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p793721045084827">

SamgrLite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p77118183084827">

typedef struct SamgrLite

.. raw:: html

   </p>

.. raw:: html

   <p id="p1551632355084827">

Represents the system ability management class.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row135554709084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1630992824084827">

TaskType

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1481027735084827">

typedef enum TaskType

.. raw:: html

   </p>

.. raw:: html

   <p id="p1291725831084827">

Enumerates task types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row525531971084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p973646178084827">

SpecifyTag

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1435278756084827">

typedef enum SpecifyTag

.. raw:: html

   </p>

.. raw:: html

   <p id="p632009839084827">

Specifies the tag for the task shared by multiple services.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1212975967084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p5705428084827">

TaskPriority

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p605663935084827">

typedef enum TaskPriority

.. raw:: html

   </p>

.. raw:: html

   <p id="p1342982091084827">

Enumerates task priority.

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

   <tr id="row1153572712084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p723242208084827">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1757239055084827">

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

   <tr id="row572077164084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p440476002084827">

BootMessage { BOOT_SYS_COMPLETED, BOOT_APP_COMPLETED, BOOT_REG_SERVICE,
BOOTSTRAP_BUTT }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p611276245084827">

Enumerates the IDs of the message to be processed for starting the
bootstrap service.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2140007566084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1746629423084827">

TaskType { SHARED_TASK = 0, SINGLE_TASK = 1, SPECIFIED_TASK = 2, NO_TASK
= 0xFF }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p797541715084827">

Enumerates task types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1670420171084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1238013101084827">

SpecifyTag { LEVEL_HIGH = 0, LEVEL_MIDDLE = 1, LEVEL_LOW = 2,
LEVEL_CUSTOM_BEGIN }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1021770324084827">

Specifies the tag for the task shared by multiple services.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1507141821084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p563076420084827">

TaskPriority { PRI_LOW = 9, PRI_BELOW_NORMAL = 16, PRI_NORMAL = 24,
PRI_ABOVE_NORMAL = 32, PRI_BUTT = 39 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1452331322084827">

Enumerates task priority.

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

   <tr id="row1439862156084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p854183053084827">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2023589296084827">

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

   <tr id="row1061272160084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1257512488084827">

VECTOR_Make (VECTOR_Key key, VECTOR_Compare compare)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1802752286084827">

Vector

.. raw:: html

   </p>

.. raw:: html

   <p id="p1439730560084827">

Creates or initializes a vector object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row621226815084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p645607473084827">

VECTOR_Clear (Vector \*vector)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1953923745084827">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1752298978084827">

Destruct a vector object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row748270231084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1381811827084827">

VECTOR_Add (Vector *vector, void*\ element)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1332407263084827">

int16

.. raw:: html

   </p>

.. raw:: html

   <p id="p422713342084827">

Adds an element to the vector.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row486392568084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1875905902084827">

VECTOR_Size (Vector \*vector)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1079502690084827">

int16

.. raw:: html

   </p>

.. raw:: html

   <p id="p1421443057084827">

Obtains the number of elements in the vector, including elements that
have been set to NULL.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1914668881084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p18765677084827">

VECTOR_Num (Vector \*vector)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1665603171084827">

int16

.. raw:: html

   </p>

.. raw:: html

   <p id="p1124612860084827">

Obtains the number of valid elements in the vector, excluding elements
that have been set to NULL.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row145787749084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p46960605084827">

VECTOR_At (Vector \*vector, int16 index)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p304258594084827">

void \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p534982227084827">

Obtains the element at a specified position.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row440386990084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p386891961084827">

VECTOR_Swap (Vector *vector, int16 index, void*\ element)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p378248941084827">

void \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1693948370084827">

Swaps the element at a specified position in a vector with another
element.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row995021145084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p632250178084827">

VECTOR_Find (Vector *vector, const void*\ element)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p117168994084827">

int16

.. raw:: html

   </p>

.. raw:: html

   <p id="p372815327084827">

Checks the position of an element.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row288414522084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1242227579084827">

VECTOR_FindByKey (Vector *vector, const void*\ key)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p878633409084827">

int16

.. raw:: html

   </p>

.. raw:: html

   <p id="p386255529084827">

Checks the position of the element with a specified key.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1210504086084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p328683935084827">

IUNKNOWN_AddRef (IUnknown \*iUnknown)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1582389987084827">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1761583135084827">

Increments the reference count in this IUnknown interface.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1115671376084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p49985063084827">

IUNKNOWN_QueryInterface (IUnknown \*iUnknown, int ver, void \**target)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1414018416084827">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1519927568084827">

Queries the IUnknown interfaces of a specified version (downcasting).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row455961907084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1104491486084827">

IUNKNOWN_Release (IUnknown \*iUnknown)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1620233973084827">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p806651360084827">

Releases a reference to an IUnknown interface that is no longer used.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1937784697084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p439900242084827">

SAMGR_SendRequest (const Identity *identity, const Request*\ request,
Handler handler)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1946689916084827">

int32

.. raw:: html

   </p>

.. raw:: html

   <p id="p339351578084827">

Sends a request to a service or feature of a specified identity.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1100704540084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p7826961084827">

SAMGR_SendSharedRequest (const Identity *identity, const
Request*\ request, uint32 \*token, Handler handler)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p28457000084827">

uint32 \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1146004714084827">

Sends a request to multiple services or features to save memory.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1361687422084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1376160620084827">

SAMGR_SendSharedDirectRequest (const Identity *id, const Request*\ req,
const Response \*resp, uint32 \**ref, Handler handler)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1229809285084827">

int32

.. raw:: html

   </p>

.. raw:: html

   <p id="p750163943084827">

Sends a request and response of a caller to the feature thread. The
handler is directly called to process the request and response without
using the message processing functions. (Customized function for the
broadcast service)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row38756340084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1407379035084827">

SAMGR_SendResponse (const Request *request, const Response*\ response)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p901733457084827">

int32

.. raw:: html

   </p>

.. raw:: html

   <p id="p150418359084827">

Sends a response after processing a request.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1743884511084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p570781978084827">

SAMGR_SendResponseByIdentity (const Identity *id, const
Request*\ request, const Response \*response)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p379415117084827">

int32

.. raw:: html

   </p>

.. raw:: html

   <p id="p1352661404084827">

Sends a response to a specified service or feature after processing the
original request. (Customized function for bootstrap)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1640690991084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1332161064084827">

SAMGR_GetInstance (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1310924113084827">

SamgrLite \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1412454563084827">

Obtains the singleton Samgr instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row82324249084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p683608978084827">

SAMGR_Bootstrap (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1910043933084827">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1004388570084827">

Starts system services and features.

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

**Macro Definition Documentation**\ 
------------------------------------

DEFAULT_IUNKNOWN_IMPL
---------------------

::

   #define DEFAULT_IUNKNOWN_IMPL

::

   Values: .QueryInterface = [IUNKNOWN_QueryInterface](samgr.rst#gac857d12648500c7dab1cb43e85ae2ed4), \

    .AddRef = [IUNKNOWN_AddRef](samgr.rst#ga9abef49ec89bf913c3bed03faf478c1e), \

    .Release = [IUNKNOWN_Release](samgr.rst#gabd462f8a5e6460a68760cd0719982296)

**Description:**

Defines the default marco for initializing the
`IUnknown <iunknown.rst>`__ interface.

When creating a subclass object of the `IUnknown <iunknown.rst>`__
interface, you can use this macro to initialize members of the
`IUnknown <iunknown.rst>`__ interface to their default values.

DEFAULT_VERSION
---------------

::

   #define DEFAULT_VERSION   0x20

**Description:**

Defines the default `IUnknown <iunknown.rst>`__ version. You can
customize the version.

The `IUnknown <iunknown.rst>`__ interface of the default version can be
called only in the current process. Inter-process communication is not
supported.

GET_IUNKNOWN
------------

::

   #define GET_IUNKNOWN( T)   ([IUnknown](iunknown.rst) *)(&((T).iUnknown))

**Description:**

Obtains the pointer of the `IUnknown <iunknown.rst>`__ interface object
from the subclass object T (generic macro) of the
`IUnknown <iunknown.rst>`__ implementation class.

Use this macro when registering `IUnknown <iunknown.rst>`__ interfaces
with Samgr so that you can obtain the interfaces from the subclass
objects of different `IUnknown <iunknown.rst>`__ implementation classes.

GET_OFFSIZE
-----------

::

   #define GET_OFFSIZE( T,  member )   (long)((char *)&(((T *)(0))->member))

**Description:**

Calculates the offset of the member in the T type.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row941415986084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p117027420084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1589556434084827">

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

   <tr id="row1443878669084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

Indicates

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

the T type.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row157396553084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

member

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the name of the T member variable.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

INHERIT_FEATURE
---------------

::

   #define INHERIT_FEATURE

::

   Values: const char *(*GetName)([Feature](feature.rst) *feature); \

    void (*OnInitialize)([Feature](feature.rst) *feature, [Service](service.rst) *parent, [Identity](identity.rst) identity); \

    void (*OnStop)([Feature](feature.rst) *feature, [Identity](identity.rst) identity); \

    BOOL (*OnMessage)([Feature](feature.rst) *feature, [Request](request.rst) *request)

**Description:**

Inherits from the macro of the feature class.

This macro provides the capability of inheriting the feature lifecycle.

INHERIT_IUNKNOWN
----------------

::

   #define INHERIT_IUNKNOWN

::

   Values: int (*QueryInterface)([IUnknown](iunknown.rst) *iUnknown, int version, void **target); \

    int (*AddRef)([IUnknown](iunknown.rst) *iUnknown); \

    int (*Release)([IUnknown](iunknown.rst) *iUnknown)

**Description:**

Defines the macro for inheriting the `IUnknown <iunknown.rst>`__
interface.

When developing a subclass of the `IUnknown <iunknown.rst>`__ class, you
can use this macro to inherit the structures of the
`IUnknown <iunknown.rst>`__ interface.

INHERIT_IUNKNOWNENTRY
---------------------

::

   #define INHERIT_IUNKNOWNENTRY( T)

::

   Values: uint16 ver; \

    int16 ref; \

    T iUnknown

**Description:**

Defines the macro for inheriting the classes that implement the
`IUnknown <iunknown.rst>`__ interface.

When developing a subclass of a class that implements the
`IUnknown <iunknown.rst>`__ interface, you can use this macro to inherit
the structures of the `IUnknown <iunknown.rst>`__ implementation class.

INHERIT_SERVICE
---------------

::

   #define INHERIT_SERVICE

::

   Values: const char *(*GetName)([Service](service.rst) * service); \

    BOOL (*Initialize)([Service](service.rst) * service, [Identity](identity.rst) identity); \

    BOOL (*MessageHandle)([Service](service.rst) * service, [Request](request.rst) * request); \

    TaskConfig (*GetTaskConfig)([Service](service.rst) * service)

**Description:**

Indicates the macro used to inherit the members from the **service**
class.

This macro provides the capability of inheriting the lifecycle functions
of the **service** class. You can use this macro to customize the
service structure.

IUNKNOWN_ENTRY_BEGIN
--------------------

::

   #define IUNKNOWN_ENTRY_BEGIN( version)

::

   Values: .ver = (version), \

    .ref = 1, \

    .iUnknown = { \

    DEFAULT_IUNKNOWN_IMPL

**Description:**

Defines the macro for initializing the classes that implement the
`IUnknown <iunknown.rst>`__ interface.

When creating a subclass object of a class that implements the
`IUnknown <iunknown.rst>`__ interface, you can use this macro to
initialize members of the `IUnknown <iunknown.rst>`__ implementation
class to their default values. You need to add the initialization of the
customized member variable.

IUNKNOWN_ENTRY_END
------------------

::

   #define IUNKNOWN_ENTRY_END   }

**Description:**

`IUnknown <iunknown.rst>`__ Defines the end macro for initializing the
`IUnknown <iunknown.rst>`__ implementation object.

This macro is used when a subclass object of the
`IUnknown <iunknown.rst>`__ implementation class is initialized.

**Typedef Documentation**\ 
---------------------------

BootMessage
-----------

::

   typedef enum [BootMessage](samgr.rst#gaf39e482610dca95f0dba85613755eb40) [BootMessage](samgr.rst#gaf39e482610dca95f0dba85613755eb40)

**Description:**

Enumerates the IDs of the message to be processed for starting the
bootstrap service.

This function is implemented by developers of the system service.
Messages sent to the bootstrap service when Samgr is started.

Handler
-------

::

   typedef void(* Handler) (const [Request](request.rst) *request, const [Response](response.rst) *response)

**Description:**

Handles asynchronous responses.

This function will be used when a service or feature uses
`IUnknown <iunknown.rst>`__ to send a request. If the caller is a
feature, this function is used to handle the response that is sent after
the feature processes a request. If the caller is a service, **Handler**
will run in the service thread.

IUnknownEntry
-------------

::

   typedef struct [IUnknownEntry](iunknownentry.rst) [IUnknownEntry](iunknownentry.rst)

**Description:**

Defines the `IUnknown <iunknown.rst>`__ implementation class.

You need to inherit this structure when developing a subclass of the
`IUnknown <iunknown.rst>`__ implementation class. Each
`IUnknown <iunknown.rst>`__ interface must correspond to one or more
`IUnknown <iunknown.rst>`__ implementation classes.

SamgrLite
---------

::

   typedef struct [SamgrLite](samgrlite.rst) [SamgrLite](samgrlite.rst)

**Description:**

Represents the system ability management class.

This class is used for registering and discovering services, features,
and functions.

SpecifyTag
----------

::

   typedef enum [SpecifyTag](samgr.rst#ga704a59a45a705ef7a15d16e3cab8c1b0) [SpecifyTag](samgr.rst#ga704a59a45a705ef7a15d16e3cab8c1b0)

**Description:**

Specifies the tag for the task shared by multiple services.

These enumerations are used for specifying a multi-service sharing task.

TaskPriority
------------

::

   typedef enum [TaskPriority](samgr.rst#gaee057e5f06a7b2533e6f58bde34d15fa) [TaskPriority](samgr.rst#gaee057e5f06a7b2533e6f58bde34d15fa)

**Description:**

Enumerates task priority.

These enumerations are used for configuring the task priority. The valid
range of the priority is (9, 39).

TaskType
--------

::

   typedef enum [TaskType](samgr.rst#ga026844c14ab62f42a2e19b54d622609b) [TaskType](samgr.rst#ga026844c14ab62f42a2e19b54d622609b)

**Description:**

Enumerates task types.

These enumerations are used for configuring the task type.

Vector
------

::

   typedef struct [SimpleVector](simplevector.rst) [Vector](samgr.rst#ga255ca81c214b8a94a90f786ceef94514)

**Description:**

Defines the simplified vector class, which is extended by four elements.

This class is applicable to the C language development scenario where
the data volume is small and dynamic expansion is required.

**Enumeration Type Documentation**\ 
------------------------------------

.. _bootmessage-1:

BootMessage
-----------

::

   enum [BootMessage](samgr.rst#gaf39e482610dca95f0dba85613755eb40)

**Description:**

Enumerates the IDs of the message to be processed for starting the
bootstrap service.

This function is implemented by developers of the system service.
Messages sent to the bootstrap service when Samgr is started.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1826895657084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1246190226084827">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p467267960084827">

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

   <tr id="row664845097084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

BOOT_SYS_COMPLETED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1985724055084827">

Message indicating that the core system service is initialized

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row63182364084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

BOOT_APP_COMPLETED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1662024056084827">

Message indicating that the system and application-layer services are
initialized

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row897765696084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

BOOT_REG_SERVICE

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2052764445084827">

Message indicating service registration during running

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row547584164084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

BOOTSTRAP_BUTT

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p792013247084827">

Maximum number of message IDs

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

.. _specifytag-1:

SpecifyTag
----------

::

   enum [SpecifyTag](samgr.rst#ga704a59a45a705ef7a15d16e3cab8c1b0)

**Description:**

Specifies the tag for the task shared by multiple services.

These enumerations are used for specifying a multi-service sharing task.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1111592708084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p607493626084827">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p932022712084827">

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

   <tr id="row1306264174084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

LEVEL_HIGH

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1708317248084827">

Preset tag

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1259051043084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

LEVEL_MIDDLE

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p961934448084827">

Preset tag

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1091538983084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

LEVEL_LOW

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1833340155084827">

Preset tag

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row759440413084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

LEVEL_CUSTOM_BEGIN

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p445366086084827">

Customized tag

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

.. _taskpriority-1:

TaskPriority
------------

::

   enum [TaskPriority](samgr.rst#gaee057e5f06a7b2533e6f58bde34d15fa)

**Description:**

Enumerates task priority.

These enumerations are used for configuring the task priority. The valid
range of the priority is (9, 39).

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1081326012084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1241923903084827">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p489196703084827">

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

   <tr id="row668870189084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PRI_LOW

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p291174510084827">

Low-priority: (9, 15)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1122742308084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PRI_BELOW_NORMAL

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1520339079084827">

Lower than the normal priority: [16, 23)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2082342429084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PRI_NORMAL

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p672626925084827">

Normal priority: [24, 31). The log service is available.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row350940836084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PRI_ABOVE_NORMAL

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p449731203084827">

Higher than the normal priority: [32, 39). The communication service is
available.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1601389495084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PRI_BUTT

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p3270449084827">

Upper limit of the priority

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

.. _tasktype-1:

TaskType
--------

::

   enum [TaskType](samgr.rst#ga026844c14ab62f42a2e19b54d622609b)

**Description:**

Enumerates task types.

These enumerations are used for configuring the task type.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row183005029084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1755750180084827">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p320665494084827">

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

   <tr id="row1348999600084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

SHARED_TASK

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1427736936084827">

Tasks shared based on their priority by services

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row103339163084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

SINGLE_TASK

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1806013450084827">

Task exclusively occupied by a service

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1293704136084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

SPECIFIED_TASK

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2087580924084827">

A specified task shared by multiple services

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row834461537084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

NO_TASK

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2021096930084827">

No task for the service. Generally, this situation does not occur.

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

IUNKNOWN_AddRef()
-----------------

::

   int IUNKNOWN_AddRef ([IUnknown](iunknown.rst) * iUnknown)

**Description:**

Increments the reference count in this `IUnknown <iunknown.rst>`__
interface.

This function is called in **QueryInterface**. Do not call this function
in the `IUnknown <iunknown.rst>`__ interface. When the **QueryInterface**
function is re-implemented, you need to call this function in the new
**QueryInterface**.***\*

\****The system does not provide a lock to protect functions. Therefore,
you need to re-implement functions if multiple developers are using
them. \***\*

**Parameters:**

IUNKNOWN_QueryInterface()
-------------------------

::

   int IUNKNOWN_QueryInterface ([IUnknown](iunknown.rst) * iUnknown, int ver, void ** target )

**Description:**

Queries the `IUnknown <iunknown.rst>`__ interfaces of a specified version
(downcasting).

After obtaining the `IUnknown <iunknown.rst>`__ interface object, the
function caller uses **QueryInterface** to convert the object to the
required subclass type. The system converts
`DEFAULT_VERSION <samgr.rst#ga13dae059206df8d2d9b9b42e694b3f9c>`__ into
the subclass type required by the caller. If the type conversion
requirements cannot be met, you need to re-implement this function.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row943782988084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1848983872084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p646625709084827">

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

   <tr id="row873292132084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

iUnknown

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the IUnknown interface.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row621519575084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

version

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the version of the IUnknown interface object to be converted.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1285357531084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

target

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the IUnknown subclass type required by the caller. This is an
output parameter.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **EC_SUCCESS** if the conversion is successful; returns other
error codes if the conversion fails.

IUNKNOWN_Release()
------------------

::

   int IUNKNOWN_Release ([IUnknown](iunknown.rst) * iUnknown)

**Description:**

Releases a reference to an `IUnknown <iunknown.rst>`__ interface that is
no longer used.

In the default implementation provided by the system, if the reference
count is **0**, the memory of the `IUnknown <iunknown.rst>`__ interface
object and implementation object is not released. If the memory of the
`IUnknown <iunknown.rst>`__ interface object and implementation object is
dynamically allocated, this function needs to be re-implemented. If the
reference count is **0**, the memory of the `IUnknown <iunknown.rst>`__
interface object and implementation object is released.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1851570677084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p967520095084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1896123941084827">

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

   <tr id="row1579380233084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

iUnknown

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the IUnknown interface object.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

\***\* Indicates the number of `IUnknown <iunknown.rst>`__ interface
objects that are referenced after the current reference is
released.*******\*

SAMGR_Bootstrap()
-----------------

::

   void SAMGR_Bootstrap (void )

**Description:**

Starts system services and features.

This function is called in the **main** function to start all services
when an independent process is developed. This function is called after
the dynamic library (containing system services and features) is loaded
during system running.

**Attention:**

This function cannot be called frequently. Otherwise, problems such as
repeated service startup may occur. It is recommended that this function
be called once in the **main** function or after the dynamic library is
loaded.

SAMGR_GetInstance()
-------------------

::

   [SamgrLite](samgrlite.rst)* SAMGR_GetInstance (void )

**Description:**

Obtains the singleton Samgr instance.

You need to call this function before using the Samgr capabilities.

**Returns:**

Returns the pointer to the singleton instance
`SamgrLite <samgrlite.rst>`__.

SAMGR_SendRequest()
-------------------

::

   int32 SAMGR_SendRequest (const [Identity](identity.rst) * identity, const [Request](request.rst) * request, [Handler](samgr.rst#ga5e13d943cc6a87a5c99fe604f3bc01e4) handler )

**Description:**

Sends a request to a service or feature of a specified identity.

This function is called by a service to send messages to its own
features through the asynchronous function of
`IUnknown <iunknown.rst>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row325528906084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1506535060084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1220123526084827">

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

   <tr id="row1598926254084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

identity

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the ID of the feature or service that processes
the message.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row219620400084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

request

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the request.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row685586445084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handler

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the function handling the response. If the value is NULL, no
response is required.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **EC_SUCCESS** if the request is sent successfully; returns
other error codes if the request fails to be sent. The caller needs to
release the memory applied in the request.

SAMGR_SendResponse()
--------------------

::

   int32 SAMGR_SendResponse (const [Request](request.rst) * request, const [Response](response.rst) * response )

**Description:**

Sends a response after processing a request.

This function is called to send a response after processing a request by
**MessageHandle** of a service or **OnMessage** of a feature.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row985556219084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1662946455084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1059543708084827">

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

   <tr id="row1619747852084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

request

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the original request.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1647232201084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

response

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the response content.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **EC_SUCCESS** if the response is sent successfully; returns
other error codes if the response fails to be sent.

**Attention:**

-  This function can be called only in **MessageHandle** or
   **OnMessage**.
-  The request must be the original one passed from **MessageHandle** or
   **OnMessage**. Otherwise, a memory exception occurs.
-  When the caller sends a request, the **handler** callback function
   must be carried.
-  The response is sent to the message queue of the service to which the
   requester belongs for processing. Therefore, the requester should
   wait for the response in non-blocking mode.

SAMGR_SendResponseByIdentity()
------------------------------

::

   int32 SAMGR_SendResponseByIdentity (const [Identity](identity.rst) * id, const [Request](request.rst) * request, const [Response](response.rst) * response )

**Description:**

Sends a response to a specified service or feature after processing the
original request. (Customized function for **bootstrap**)

This function is called to send a response after processing a request by
**MessageHandle** of a service or **OnMessage** of a feature. This
function can be customized to implement phased startup of different
types of services.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row71401478084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1223550055084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1180949390084827">

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

   <tr id="row641217016084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

id

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the ID of a service or feature. The response is
sent to the thread of the service or feature for processing.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row22852660084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

request

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the original request.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row644844266084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

response

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the response content.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **EC_SUCCESS** if the response is sent successfully; returns
other error codes if the response fails to be sent.

**Attention:**

-  This function can be called only in **MessageHandle** or
   **OnMessage**.
-  The request must be the original one passed from **MessageHandle** or
   **OnMessage**. Otherwise, a memory exception occurs.
-  When the caller sends a request, the **handler** callback function
   must be carried.
-  The response is sent to the message queue of a specified ID for
   processing. Therefore, wait for the response in non-blocking mode.

SAMGR_SendSharedDirectRequest()
-------------------------------

::

   int32 SAMGR_SendSharedDirectRequest (const [Identity](identity.rst) * id, const [Request](request.rst) * req, const [Response](response.rst) * resp, uint32 ** ref, [Handler](samgr.rst#ga5e13d943cc6a87a5c99fe604f3bc01e4) handler )

**Description:**

Sends a request and response of a caller to the feature thread. The
handler is directly called to process the request and response without
using the message processing functions. (Customized function for the
broadcast service)

This function is used to publish topics for the
`Broadcast <broadcast.rst>`__ service to broadcast messages. The value of
reference counting is incremented by one each time this function is
called.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row970307468084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p84370070084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1184348500084827">

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

   <tr id="row29696998084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

id

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the IDs of services or features, to which the
request and response are sent.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row703292607084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

request

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the request.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row732971693084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

resp

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the response.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1270172204084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ref

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the reference counting.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1485932502084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handler

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the function for handling the request and response. This
parameter cannot be NULL.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **EC_SUCCESS** if the request and response are sent
successfully; returns other error codes if the request and response fail
to be sent.

**Attention:**

-  Ensure that the thread specified by **identity** processes the
   message after all messages are sent. Common practice: Add a lock
   before sending a request and add the same lock during processing.
-  If **NULL** is returned, the caller needs to release the memory of
   the request and response.
-  If the response changes each time when a request is sent, ensure that
   the response will not be released. (Set **len** to **0**, the
   **data** of response will be the resident memory.)

SAMGR_SendSharedRequest()
-------------------------

::

   uint32* SAMGR_SendSharedRequest (const [Identity](identity.rst) * identity, const [Request](request.rst) * request, uint32 * token, [Handler](samgr.rst#ga5e13d943cc6a87a5c99fe604f3bc01e4) handler )

**Description:**

Sends a request to multiple services or features to save memory.

This function is used to publish topics for the
`Broadcast <broadcast.rst>`__ service to broadcast messages.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row424898449084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1182177316084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p910411564084827">

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

   <tr id="row687559011084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

identity

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the IDs of services or features, to which
requests are sent.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1717368813084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

request

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the request.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1523982061084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

token

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to reference counting.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1599203830084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handler

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the function handling the response. If the value is NULL, no
response is required.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Attention:**

-  Ensure that the thread specified by **identity** processes the
   message after all messages are sent. Common practice: Add a lock
   before sending a request and add the same lock during processing.
-  If **NULL** is returned, the caller needs to release the memory of
   the request.

VECTOR_Add()
------------

::

   int16 VECTOR_Add ([Vector](samgr.rst#ga255ca81c214b8a94a90f786ceef94514) * vector, void * element )

**Description:**

Adds an element to the vector.

This function is used to add an element to the vector.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row106012767084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1288498749084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1958028114084827">

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

   <tr id="row344942262084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

vector

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the this pointer to the vector.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row266141007084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

element

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the element to add.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the location of the element to be added if the operation is
successful; returns **INVALID_INDEX** if the operation fails.

VECTOR_At()
-----------

::

   void* VECTOR_At ([Vector](samgr.rst#ga255ca81c214b8a94a90f786ceef94514) * vector, int16 index )

**Description:**

Obtains the element at a specified position.

This function is used to obtain the element at a specified position.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row615753016084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p384100012084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1292591324084827">

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

   <tr id="row1511351171084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

vector

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the this pointer to the vector.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1520774900084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

index

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the subscript to be obtained.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the element if obtained; returns **NULL** otherwise.

VECTOR_Clear()
--------------

::

   void VECTOR_Clear ([Vector](samgr.rst#ga255ca81c214b8a94a90f786ceef94514) * vector)

**Description:**

Destruct a vector object.

This function is used to clear the memory applied by the vector after
the temporary vector in the stack is used.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row288637707084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p969502873084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1367456151084827">

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

   <tr id="row1767321718084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

vector

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the vector to clear.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

VECTOR_Find()
-------------

::

   int16 VECTOR_Find ([Vector](samgr.rst#ga255ca81c214b8a94a90f786ceef94514) * vector, const void * element )

**Description:**

Checks the position of an element.

This function is used to check whether a vector has a specified element.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1034310467084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1977692582084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p106229066084827">

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

   <tr id="row1849115575084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

vector

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the this pointer to the vector.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1121108377084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

element

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the element to be checked.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the index of the element that is not less than 0 if the check is
successful; returns **INVALID_INDEX** if the check fails.

VECTOR_FindByKey()
------------------

::

   int16 VECTOR_FindByKey ([Vector](samgr.rst#ga255ca81c214b8a94a90f786ceef94514) * vector, const void * key )

**Description:**

Checks the position of the element with a specified key.

This function is used to check an element based on its key value.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1557712763084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1707346909084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1321658454084827">

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

   <tr id="row1554643263084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

vector

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the this pointer to the vector.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1391553920084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

key

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the key value of the element to check.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the index of the key element that is not less than 0 if the
check is successful; returns **INVALID_INDEX** if the check fails.

VECTOR_Make()
-------------

::

   [Vector](samgr.rst#ga255ca81c214b8a94a90f786ceef94514) VECTOR_Make (VECTOR_Key key, VECTOR_Compare compare )

**Description:**

Creates or initializes a vector object.

This function is used to create or initialize a vector object.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row877268616084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p751673413084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1150647680084827">

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

   <tr id="row848962605084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

key

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the function provided by users for converting
data elements into key values. If this function is not provided, set it
to NULL.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2124002445084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

compare

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the function for comparing the sizes of two
elements. If this function is not provided, set it to NULL.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the vector right value object.

VECTOR_Num()
------------

::

   int16 VECTOR_Num ([Vector](samgr.rst#ga255ca81c214b8a94a90f786ceef94514) * vector)

**Description:**

Obtains the number of valid elements in the vector, excluding elements
that have been set to **NULL**.

This function is used to check whether the number of elements reaches
the upper limit.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row818903856084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p700847165084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p60130186084827">

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

   <tr id="row1047826577084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

vector

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the this pointer to the vector.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the top - free value of the vector, which indicates the number
of non-null elements.

VECTOR_Size()
-------------

::

   int16 VECTOR_Size ([Vector](samgr.rst#ga255ca81c214b8a94a90f786ceef94514) * vector)

**Description:**

Obtains the number of elements in the vector, including elements that
have been set to **NULL**.

This function is used for full traversal.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row397149397084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p245713471084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1196646563084827">

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

   <tr id="row2112891313084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

vector

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the this pointer to the vector.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the top value of the vector, which indicates the number of
elements.

VECTOR_Swap()
-------------

::

   void* VECTOR_Swap ([Vector](samgr.rst#ga255ca81c214b8a94a90f786ceef94514) * vector, int16 index, void * element )

**Description:**

Swaps the element at a specified position in a vector with another
element.

This function is used to clear, sort, or update elements in the vector.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row169991328084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p994559027084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p736047863084827">

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

   <tr id="row721113098084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

vector

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the this pointer to the vector.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row91456032084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

index

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the position of the element to be swapped.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1744087056084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

element

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the new element.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Attention:**

Before using this function, ensure that the index is valid. You can use
**VECTOR_Size** to obtain the upper limit of the index.

**Returns:**

Returns the original element if the swapping is successful; returns
**NULL** if the swapping fails.

**See also:**

`VECTOR_Size <samgr.rst#ga1432f30c136d14bc00414d883d8be3bd>`__
