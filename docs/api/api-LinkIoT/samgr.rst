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

   <tr id="row345291593090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p786054434090251">

File Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1466968346090251">

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

   <tr id="row1682363436090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2066921740090251">

common.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1266324314090251">

Provides common objects and functions for Samgr and external modules.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row867069756090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2093919664090251">

feature.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p119649395090251">

Defines the base class of a feature.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2108474342090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p547452597090251">

iunknown.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1991147643090251">

Provides the base class and default implementation for external
functions of system capabilities.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row796779364090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2048475469090251">

message.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1561654959090251">

Provides message communication APIs that help you to implement
asynchronous functions of IUnknown.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1932977983090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1559543293090251">

samgr_lite.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1673971483090251">

Manages system capabilities.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2143098297090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p341521057090251">

service.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p887721653090251">

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

   <tr id="row324001174090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p527272444090251">

Data Structure Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1844913962090251">

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

   <tr id="row90952491090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2087860125090251">

SimpleVector

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1360796389090251">

Defines the simplified vector class, which is extended by four elements.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1104533812090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p884304604090251">

Feature

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1667246312090251">

Defines the base class of a feature.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row388485771090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1804715358090251">

IUnknown

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p641648004090251">

Defines the IUnknown class.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1292128046090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p178598111090251">

IUnknownEntry

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1638863698090251">

Defines the IUnknown implementation class.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1674093872090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p521085203090251">

Identity

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p633635469090251">

Identifies a service and feature.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1029830504090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1457351485090251">

Request

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2090323063090251">

Defines a request.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row229030773090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2014719945090251">

Response

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p206473900090251">

Defines a response.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row531185981090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1592868998090251">

SamgrLite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p314008953090251">

Represents the system ability management class.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1867724626090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p935578751090251">

TaskConfig

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1116648357090251">

Defines task configurations for a service.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1323183419090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p729490945090251">

Service

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1294208744090251">

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

   <tr id="row891967589090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1478405054090251">

Macro Name and Value

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p365649652090251">

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

   <tr id="row727337731090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1983579211090251">

GET_OFFSIZE(T, member) (long)((char *)&(((T*)(0))->member))

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1654863425090251">

Calculates the offset of the member in the T type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1857742699090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p551951255090251">

INHERIT_FEATURE

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1957458352090251">

Inherits from the macro of the feature class.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row209527492090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1212062395090251">

DEFAULT_VERSION 0x20

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1303318244090251">

Defines the default IUnknown version. You can customize the version.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row272102842090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p900671566090251">

INHERIT_IUNKNOWN

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p73206041090251">

Defines the macro for inheriting the IUnknown interface.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1921264422090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1355983873090251">

INHERIT_IUNKNOWNENTRY(T)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p821347630090251">

Defines the macro for inheriting the classes that implement the IUnknown
interface.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row892687642090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2024681541090251">

DEFAULT_IUNKNOWN_IMPL

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1208606483090251">

Defines the default marco for initializing the IUnknown interface.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2019181798090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1137038963090251">

IUNKNOWN_ENTRY_BEGIN(version)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p538936643090251">

Defines the macro for initializing the classes that implement the
IUnknown interface.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2020027773090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1761953018090251">

IUNKNOWN_ENTRY_END }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p433759306090251">

IUnknown Defines the end macro for initializing the IUnknown
implementation object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1236569301090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p187609433090251">

GET_IUNKNOWN(T) (IUnknown \*)(&((T).iUnknown))

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1051372482090251">

Obtains the pointer of the IUnknown interface object from the subclass
object T (generic macro) of the IUnknown implementation class.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1762820117090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p324382283090251">

BOOTSTRAP_SERVICE “Bootstrap”

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1567994412090251">

Starts a bootstrap service, which is used by samgr and implemented by
system service developers.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1500298556090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p694884275090251">

INHERIT_SERVICE

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1099296592090251">

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

   <tr id="row1816888183090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1240500193090251">

Typedef Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p851258433090251">

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

   <tr id="row1289022097090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p330845254090251">

Vector

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1858442784090251">

typedef struct SimpleVector

.. raw:: html

   </p>

.. raw:: html

   <p id="p1487905068090251">

Defines the simplified vector class, which is extended by four elements.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1820871402090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p563625076090251">

IUnknownEntry

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p242508138090251">

typedef struct IUnknownEntry

.. raw:: html

   </p>

.. raw:: html

   <p id="p1789794500090251">

Defines the IUnknown implementation class.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2059445640090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1919228543090251">

Handler) (const Request *request, const Response*\ response)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p691786619090251">

typedef void(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p214877384090251">

Handles asynchronous responses.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1549273024090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1679518249090251">

BootMessage

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1207009928090251">

typedef enum BootMessage

.. raw:: html

   </p>

.. raw:: html

   <p id="p1182093202090251">

Enumerates the IDs of the message to be processed for starting the
bootstrap service.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row591448736090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1486203205090251">

SamgrLite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2073746405090251">

typedef struct SamgrLite

.. raw:: html

   </p>

.. raw:: html

   <p id="p2106179950090251">

Represents the system ability management class.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row452053792090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p236533271090251">

TaskType

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p573309501090251">

typedef enum TaskType

.. raw:: html

   </p>

.. raw:: html

   <p id="p926357161090251">

Enumerates task types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row822093909090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1892982340090251">

SpecifyTag

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1212075030090251">

typedef enum SpecifyTag

.. raw:: html

   </p>

.. raw:: html

   <p id="p899307972090251">

Specifies the tag for the task shared by multiple services.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row59495320090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p671906240090251">

TaskPriority

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1718077584090251">

typedef enum TaskPriority

.. raw:: html

   </p>

.. raw:: html

   <p id="p1000751757090251">

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

   <tr id="row1671966725090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1083420467090251">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p591266479090251">

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

   <tr id="row232057888090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1850461181090251">

BootMessage { BOOT_SYS_COMPLETED, BOOT_APP_COMPLETED, BOOT_REG_SERVICE,
BOOTSTRAP_BUTT }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p148427384090251">

Enumerates the IDs of the message to be processed for starting the
bootstrap service.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1239314926090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2132298402090251">

TaskType { SHARED_TASK = 0, SINGLE_TASK = 1, SPECIFIED_TASK = 2, NO_TASK
= 0xFF }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1252298568090251">

Enumerates task types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1635974821090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1401922982090251">

SpecifyTag { LEVEL_HIGH = 0, LEVEL_MIDDLE = 1, LEVEL_LOW = 2,
LEVEL_CUSTOM_BEGIN }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1580416024090251">

Specifies the tag for the task shared by multiple services.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1155328802090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1274186846090251">

TaskPriority { PRI_LOW = 9, PRI_BELOW_NORMAL = 16, PRI_NORMAL = 24,
PRI_ABOVE_NORMAL = 32, PRI_BUTT = 39 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1844021317090251">

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

   <tr id="row1457473510090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p992391663090251">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p355965946090251">

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

   <tr id="row1393981896090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1712340226090251">

VECTOR_Make (VECTOR_Key key, VECTOR_Compare compare)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p22909296090251">

Vector

.. raw:: html

   </p>

.. raw:: html

   <p id="p829171923090251">

Creates or initializes a vector object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row797479647090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p476563010090251">

VECTOR_Clear (Vector \*vector)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p453530426090251">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1216293216090251">

Destruct a vector object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1749273782090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p818402421090251">

VECTOR_Add (Vector *vector, void*\ element)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p438487713090251">

int16

.. raw:: html

   </p>

.. raw:: html

   <p id="p360672133090251">

Adds an element to the vector.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2012771576090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1208565096090251">

VECTOR_Size (Vector \*vector)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1786185710090251">

int16

.. raw:: html

   </p>

.. raw:: html

   <p id="p1823639713090251">

Obtains the number of elements in the vector, including elements that
have been set to NULL.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1247621836090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1974688218090251">

VECTOR_Num (Vector \*vector)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1512082388090251">

int16

.. raw:: html

   </p>

.. raw:: html

   <p id="p1248043151090251">

Obtains the number of valid elements in the vector, excluding elements
that have been set to NULL.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row959546128090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1242887967090251">

VECTOR_At (Vector \*vector, int16 index)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1296913045090251">

void \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1829240686090251">

Obtains the element at a specified position.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1102282513090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1499802438090251">

VECTOR_Swap (Vector *vector, int16 index, void*\ element)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1885708610090251">

void \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p313693973090251">

Swaps the element at a specified position in a vector with another
element.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row962769553090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1865149794090251">

VECTOR_Find (Vector *vector, const void*\ element)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p209570894090251">

int16

.. raw:: html

   </p>

.. raw:: html

   <p id="p1159407766090251">

Checks the position of an element.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row986056407090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p728934019090251">

VECTOR_FindByKey (Vector *vector, const void*\ key)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p128844508090251">

int16

.. raw:: html

   </p>

.. raw:: html

   <p id="p1974386226090251">

Checks the position of the element with a specified key.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1049225753090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p744846362090251">

IUNKNOWN_AddRef (IUnknown \*iUnknown)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2024727768090251">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p2134401529090251">

Increments the reference count in this IUnknown interface.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1653093334090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p50183179090251">

IUNKNOWN_QueryInterface (IUnknown \*iUnknown, int ver, void \**target)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1230713787090251">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p771393535090251">

Queries the IUnknown interfaces of a specified version (downcasting).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1497238672090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1170978906090251">

IUNKNOWN_Release (IUnknown \*iUnknown)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1493993492090251">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1719071053090251">

Releases a reference to an IUnknown interface that is no longer used.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2071601977090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1096801232090251">

SAMGR_SendRequest (const Identity *identity, const Request*\ request,
Handler handler)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1342487079090251">

int32

.. raw:: html

   </p>

.. raw:: html

   <p id="p1495268878090251">

Sends a request to a service or feature of a specified identity.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2014465149090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1913916835090251">

SAMGR_SendSharedRequest (const Identity *identity, const
Request*\ request, uint32 \*token, Handler handler)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1792842355090251">

uint32 \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1065800656090251">

Sends a request to multiple services or features to save memory.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2067371477090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1585004814090251">

SAMGR_SendSharedDirectRequest (const Identity *id, const Request*\ req,
const Response \*resp, uint32 \**ref, Handler handler)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1337028684090251">

int32

.. raw:: html

   </p>

.. raw:: html

   <p id="p352395311090251">

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

   <tr id="row1959048863090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1299787508090251">

SAMGR_SendResponse (const Request *request, const Response*\ response)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1244401644090251">

int32

.. raw:: html

   </p>

.. raw:: html

   <p id="p662626517090251">

Sends a response after processing a request.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1721952813090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1085117495090251">

SAMGR_SendResponseByIdentity (const Identity *id, const
Request*\ request, const Response \*response)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1357478251090251">

int32

.. raw:: html

   </p>

.. raw:: html

   <p id="p1956977053090251">

Sends a response to a specified service or feature after processing the
original request. (Customized function for bootstrap)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1567962255090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2067783248090251">

SAMGR_GetInstance (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1635963009090251">

SamgrLite \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p432777252090251">

Obtains the singleton Samgr instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1269219194090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p842163964090251">

SAMGR_Bootstrap (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p560445270090251">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1507353627090251">

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

   Values: .QueryInterface = [IUNKNOWN_QueryInterface](samgr.md#gac857d12648500c7dab1cb43e85ae2ed4), \

    .AddRef = [IUNKNOWN_AddRef](samgr.md#ga9abef49ec89bf913c3bed03faf478c1e), \

    .Release = [IUNKNOWN_Release](samgr.md#gabd462f8a5e6460a68760cd0719982296)

**Description:**

Defines the default marco for initializing the
`IUnknown <iunknown.md>`__ interface.

When creating a subclass object of the `IUnknown <iunknown.md>`__
interface, you can use this macro to initialize members of the
`IUnknown <iunknown.md>`__ interface to their default values.

DEFAULT_VERSION
---------------

::

   #define DEFAULT_VERSION   0x20

**Description:**

Defines the default `IUnknown <iunknown.md>`__ version. You can
customize the version.

The `IUnknown <iunknown.md>`__ interface of the default version can be
called only in the current process. Inter-process communication is not
supported.

GET_IUNKNOWN
------------

::

   #define GET_IUNKNOWN( T)   ([IUnknown](iunknown.md) *)(&((T).iUnknown))

**Description:**

Obtains the pointer of the `IUnknown <iunknown.md>`__ interface object
from the subclass object T (generic macro) of the
`IUnknown <iunknown.md>`__ implementation class.

Use this macro when registering `IUnknown <iunknown.md>`__ interfaces
with Samgr so that you can obtain the interfaces from the subclass
objects of different `IUnknown <iunknown.md>`__ implementation classes.

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

   <tr id="row947316109090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1526311938090251">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p492333796090251">

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

   <tr id="row724526608090251">

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

   <tr id="row541021051090251">

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

   Values: const char *(*GetName)([Feature](feature.md) *feature); \

    void (*OnInitialize)([Feature](feature.md) *feature, [Service](service.md) *parent, [Identity](identity.md) identity); \

    void (*OnStop)([Feature](feature.md) *feature, [Identity](identity.md) identity); \

    BOOL (*OnMessage)([Feature](feature.md) *feature, [Request](request.md) *request)

**Description:**

Inherits from the macro of the feature class.

This macro provides the capability of inheriting the feature lifecycle.

INHERIT_IUNKNOWN
----------------

::

   #define INHERIT_IUNKNOWN

::

   Values: int (*QueryInterface)([IUnknown](iunknown.md) *iUnknown, int version, void **target); \

    int (*AddRef)([IUnknown](iunknown.md) *iUnknown); \

    int (*Release)([IUnknown](iunknown.md) *iUnknown)

**Description:**

Defines the macro for inheriting the `IUnknown <iunknown.md>`__
interface.

When developing a subclass of the `IUnknown <iunknown.md>`__ class, you
can use this macro to inherit the structures of the
`IUnknown <iunknown.md>`__ interface.

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
`IUnknown <iunknown.md>`__ interface.

When developing a subclass of a class that implements the
`IUnknown <iunknown.md>`__ interface, you can use this macro to inherit
the structures of the `IUnknown <iunknown.md>`__ implementation class.

INHERIT_SERVICE
---------------

::

   #define INHERIT_SERVICE

::

   Values: const char *(*GetName)([Service](service.md) * service); \

    BOOL (*Initialize)([Service](service.md) * service, [Identity](identity.md) identity); \

    BOOL (*MessageHandle)([Service](service.md) * service, [Request](request.md) * request); \

    TaskConfig (*GetTaskConfig)([Service](service.md) * service)

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
`IUnknown <iunknown.md>`__ interface.

When creating a subclass object of a class that implements the
`IUnknown <iunknown.md>`__ interface, you can use this macro to
initialize members of the `IUnknown <iunknown.md>`__ implementation
class to their default values. You need to add the initialization of the
customized member variable.

IUNKNOWN_ENTRY_END
------------------

::

   #define IUNKNOWN_ENTRY_END   }

**Description:**

`IUnknown <iunknown.md>`__ Defines the end macro for initializing the
`IUnknown <iunknown.md>`__ implementation object.

This macro is used when a subclass object of the
`IUnknown <iunknown.md>`__ implementation class is initialized.

**Typedef Documentation**\ 
---------------------------

BootMessage
-----------

::

   typedef enum [BootMessage](samgr.md#gaf39e482610dca95f0dba85613755eb40) [BootMessage](samgr.md#gaf39e482610dca95f0dba85613755eb40)

**Description:**

Enumerates the IDs of the message to be processed for starting the
bootstrap service.

This function is implemented by developers of the system service.
Messages sent to the bootstrap service when Samgr is started.

Handler
-------

::

   typedef void(* Handler) (const [Request](request.md) *request, const [Response](response.md) *response)

**Description:**

Handles asynchronous responses.

This function will be used when a service or feature uses
`IUnknown <iunknown.md>`__ to send a request. If the caller is a
feature, this function is used to handle the response that is sent after
the feature processes a request. If the caller is a service, **Handler**
will run in the service thread.

IUnknownEntry
-------------

::

   typedef struct [IUnknownEntry](iunknownentry.md) [IUnknownEntry](iunknownentry.md)

**Description:**

Defines the `IUnknown <iunknown.md>`__ implementation class.

You need to inherit this structure when developing a subclass of the
`IUnknown <iunknown.md>`__ implementation class. Each
`IUnknown <iunknown.md>`__ interface must correspond to one or more
`IUnknown <iunknown.md>`__ implementation classes.

SamgrLite
---------

::

   typedef struct [SamgrLite](samgrlite.md) [SamgrLite](samgrlite.md)

**Description:**

Represents the system ability management class.

This class is used for registering and discovering services, features,
and functions.

SpecifyTag
----------

::

   typedef enum [SpecifyTag](samgr.md#ga704a59a45a705ef7a15d16e3cab8c1b0) [SpecifyTag](samgr.md#ga704a59a45a705ef7a15d16e3cab8c1b0)

**Description:**

Specifies the tag for the task shared by multiple services.

These enumerations are used for specifying a multi-service sharing task.

TaskPriority
------------

::

   typedef enum [TaskPriority](samgr.md#gaee057e5f06a7b2533e6f58bde34d15fa) [TaskPriority](samgr.md#gaee057e5f06a7b2533e6f58bde34d15fa)

**Description:**

Enumerates task priority.

These enumerations are used for configuring the task priority. The valid
range of the priority is (9, 39).

TaskType
--------

::

   typedef enum [TaskType](samgr.md#ga026844c14ab62f42a2e19b54d622609b) [TaskType](samgr.md#ga026844c14ab62f42a2e19b54d622609b)

**Description:**

Enumerates task types.

These enumerations are used for configuring the task type.

Vector
------

::

   typedef struct [SimpleVector](simplevector.md) [Vector](samgr.md#ga255ca81c214b8a94a90f786ceef94514)

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

   enum [BootMessage](samgr.md#gaf39e482610dca95f0dba85613755eb40)

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

   <tr id="row947724544090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p436492665090251">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p897636635090251">

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

   <tr id="row2117310933090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

BOOT_SYS_COMPLETED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1894481283090251">

Message indicating that the core system service is initialized

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row836553795090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

BOOT_APP_COMPLETED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1232863397090251">

Message indicating that the system and application-layer services are
initialized

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1247837705090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

BOOT_REG_SERVICE

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1628140731090251">

Message indicating service registration during running

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1406519059090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

BOOTSTRAP_BUTT

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p645293632090251">

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

   enum [SpecifyTag](samgr.md#ga704a59a45a705ef7a15d16e3cab8c1b0)

**Description:**

Specifies the tag for the task shared by multiple services.

These enumerations are used for specifying a multi-service sharing task.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row528105841090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1920091288090251">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1745238769090251">

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

   <tr id="row541115062090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

LEVEL_HIGH

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p734543630090251">

Preset tag

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row656745566090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

LEVEL_MIDDLE

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1310710628090251">

Preset tag

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1000984084090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

LEVEL_LOW

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p60765292090251">

Preset tag

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row994026916090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

LEVEL_CUSTOM_BEGIN

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p85149525090251">

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

   enum [TaskPriority](samgr.md#gaee057e5f06a7b2533e6f58bde34d15fa)

**Description:**

Enumerates task priority.

These enumerations are used for configuring the task priority. The valid
range of the priority is (9, 39).

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1316398369090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1187457994090251">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1252812569090251">

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

   <tr id="row1771927474090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PRI_LOW

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p57230093090251">

Low-priority: (9, 15)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1452179012090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PRI_BELOW_NORMAL

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1338560472090251">

Lower than the normal priority: [16, 23)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row626429694090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PRI_NORMAL

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p668769884090251">

Normal priority: [24, 31). The log service is available.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1867972967090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PRI_ABOVE_NORMAL

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p984415169090251">

Higher than the normal priority: [32, 39). The communication service is
available.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1326124243090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PRI_BUTT

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2051676968090251">

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

   enum [TaskType](samgr.md#ga026844c14ab62f42a2e19b54d622609b)

**Description:**

Enumerates task types.

These enumerations are used for configuring the task type.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1685905641090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2025684354090251">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p977134890090251">

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

   <tr id="row1826480641090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

SHARED_TASK

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p136205250090251">

Tasks shared based on their priority by services

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row268702970090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

SINGLE_TASK

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1654484694090251">

Task exclusively occupied by a service

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row859542571090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

SPECIFIED_TASK

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p140548709090251">

A specified task shared by multiple services

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1843825509090251">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

NO_TASK

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p668010185090251">

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

   int IUNKNOWN_AddRef ([IUnknown](iunknown.md) * iUnknown)

**Description:**

Increments the reference count in this `IUnknown <iunknown.md>`__
interface.

This function is called in **QueryInterface**. Do not call this function
in the `IUnknown <iunknown.md>`__ interface. When the **QueryInterface**
function is re-implemented, you need to call this function in the new
**QueryInterface**.***\*

\****The system does not provide a lock to protect functions. Therefore,
you need to re-implement functions if multiple developers are using
them. \***\*

**Parameters:**

IUNKNOWN_QueryInterface()
-------------------------

::

   int IUNKNOWN_QueryInterface ([IUnknown](iunknown.md) * iUnknown, int ver, void ** target )

**Description:**

Queries the `IUnknown <iunknown.md>`__ interfaces of a specified version
(downcasting).

After obtaining the `IUnknown <iunknown.md>`__ interface object, the
function caller uses **QueryInterface** to convert the object to the
required subclass type. The system converts
`DEFAULT_VERSION <samgr.md#ga13dae059206df8d2d9b9b42e694b3f9c>`__ into
the subclass type required by the caller. If the type conversion
requirements cannot be met, you need to re-implement this function.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row105581912090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p656629405090251">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p760583562090251">

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

   <tr id="row822542141090251">

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

   <tr id="row1669303117090251">

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

   <tr id="row1631904826090251">

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

   int IUNKNOWN_Release ([IUnknown](iunknown.md) * iUnknown)

**Description:**

Releases a reference to an `IUnknown <iunknown.md>`__ interface that is
no longer used.

In the default implementation provided by the system, if the reference
count is **0**, the memory of the `IUnknown <iunknown.md>`__ interface
object and implementation object is not released. If the memory of the
`IUnknown <iunknown.md>`__ interface object and implementation object is
dynamically allocated, this function needs to be re-implemented. If the
reference count is **0**, the memory of the `IUnknown <iunknown.md>`__
interface object and implementation object is released.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1252968894090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1962261185090251">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p492350853090251">

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

   <tr id="row112491798090251">

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

\***\* Indicates the number of `IUnknown <iunknown.md>`__ interface
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

   [SamgrLite](samgrlite.md)* SAMGR_GetInstance (void )

**Description:**

Obtains the singleton Samgr instance.

You need to call this function before using the Samgr capabilities.

**Returns:**

Returns the pointer to the singleton instance
`SamgrLite <samgrlite.md>`__.

SAMGR_SendRequest()
-------------------

::

   int32 SAMGR_SendRequest (const [Identity](identity.md) * identity, const [Request](request.md) * request, [Handler](samgr.md#ga5e13d943cc6a87a5c99fe604f3bc01e4) handler )

**Description:**

Sends a request to a service or feature of a specified identity.

This function is called by a service to send messages to its own
features through the asynchronous function of
`IUnknown <iunknown.md>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row351040454090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p670008735090251">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p995961987090251">

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

   <tr id="row1052999698090251">

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

   <tr id="row994889845090251">

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

   <tr id="row1485365702090251">

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

   int32 SAMGR_SendResponse (const [Request](request.md) * request, const [Response](response.md) * response )

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

   <tr id="row1810582354090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1844917566090251">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p350331469090251">

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

   <tr id="row1921776010090251">

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

   <tr id="row1722084287090251">

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

   int32 SAMGR_SendResponseByIdentity (const [Identity](identity.md) * id, const [Request](request.md) * request, const [Response](response.md) * response )

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

   <tr id="row485641331090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p507306099090251">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p10525329090251">

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

   <tr id="row220904329090251">

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

   <tr id="row450921479090251">

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

   <tr id="row715689479090251">

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

   int32 SAMGR_SendSharedDirectRequest (const [Identity](identity.md) * id, const [Request](request.md) * req, const [Response](response.md) * resp, uint32 ** ref, [Handler](samgr.md#ga5e13d943cc6a87a5c99fe604f3bc01e4) handler )

**Description:**

Sends a request and response of a caller to the feature thread. The
handler is directly called to process the request and response without
using the message processing functions. (Customized function for the
broadcast service)

This function is used to publish topics for the
`Broadcast <broadcast.md>`__ service to broadcast messages. The value of
reference counting is incremented by one each time this function is
called.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row751329307090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1794574380090251">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1337534818090251">

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

   <tr id="row1229926829090251">

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

   <tr id="row1264721591090251">

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

   <tr id="row2147327729090251">

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

   <tr id="row1548932120090251">

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

   <tr id="row790427849090251">

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

   uint32* SAMGR_SendSharedRequest (const [Identity](identity.md) * identity, const [Request](request.md) * request, uint32 * token, [Handler](samgr.md#ga5e13d943cc6a87a5c99fe604f3bc01e4) handler )

**Description:**

Sends a request to multiple services or features to save memory.

This function is used to publish topics for the
`Broadcast <broadcast.md>`__ service to broadcast messages.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row647618199090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1746216097090251">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p163918959090251">

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

   <tr id="row145796023090251">

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

   <tr id="row1068314224090251">

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

   <tr id="row1482008274090251">

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

   <tr id="row1769501324090251">

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

   int16 VECTOR_Add ([Vector](samgr.md#ga255ca81c214b8a94a90f786ceef94514) * vector, void * element )

**Description:**

Adds an element to the vector.

This function is used to add an element to the vector.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1593595227090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p62292398090251">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2074663425090251">

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

   <tr id="row639986577090251">

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

   <tr id="row846073089090251">

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

   void* VECTOR_At ([Vector](samgr.md#ga255ca81c214b8a94a90f786ceef94514) * vector, int16 index )

**Description:**

Obtains the element at a specified position.

This function is used to obtain the element at a specified position.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1530484190090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1133547827090251">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1874236448090251">

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

   <tr id="row144984992090251">

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

   <tr id="row315879884090251">

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

   void VECTOR_Clear ([Vector](samgr.md#ga255ca81c214b8a94a90f786ceef94514) * vector)

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

   <tr id="row1444891260090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2136077429090251">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p319605303090251">

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

   <tr id="row1209698915090251">

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

   int16 VECTOR_Find ([Vector](samgr.md#ga255ca81c214b8a94a90f786ceef94514) * vector, const void * element )

**Description:**

Checks the position of an element.

This function is used to check whether a vector has a specified element.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row977784952090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1650996307090251">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p238311038090251">

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

   <tr id="row804768399090251">

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

   <tr id="row2097072755090251">

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

   int16 VECTOR_FindByKey ([Vector](samgr.md#ga255ca81c214b8a94a90f786ceef94514) * vector, const void * key )

**Description:**

Checks the position of the element with a specified key.

This function is used to check an element based on its key value.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1483315555090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1854922059090251">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p722939948090251">

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

   <tr id="row510079002090251">

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

   <tr id="row1070626273090251">

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

   [Vector](samgr.md#ga255ca81c214b8a94a90f786ceef94514) VECTOR_Make (VECTOR_Key key, VECTOR_Compare compare )

**Description:**

Creates or initializes a vector object.

This function is used to create or initialize a vector object.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1825551265090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p789711233090251">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1153175451090251">

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

   <tr id="row1976615794090251">

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

   <tr id="row1864757177090251">

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

   int16 VECTOR_Num ([Vector](samgr.md#ga255ca81c214b8a94a90f786ceef94514) * vector)

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

   <tr id="row58039475090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1874895703090251">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p126619804090251">

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

   <tr id="row1053391398090251">

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

   int16 VECTOR_Size ([Vector](samgr.md#ga255ca81c214b8a94a90f786ceef94514) * vector)

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

   <tr id="row1902226744090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1161063466090251">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p306757255090251">

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

   <tr id="row736962300090251">

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

   void* VECTOR_Swap ([Vector](samgr.md#ga255ca81c214b8a94a90f786ceef94514) * vector, int16 index, void * element )

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

   <tr id="row1641012864090251">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1300222266090251">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1392510338090251">

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

   <tr id="row1485720599090251">

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

   <tr id="row1928563881090251">

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

   <tr id="row1006347094090251">

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

`VECTOR_Size <samgr.md#ga1432f30c136d14bc00414d883d8be3bd>`__
