Registry
========

**Overview**\ 
--------------

Provides APIs for registering and discovering inter-process
communication (IPC) capabilities.

Based on the Samgr development framework, this module helps you to
develop system capabilities and implement cross-process calls. This
module is used when system capabilities need to be provided across
processes.

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

   <tr id="row112523827084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p819560436084827">

File Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1136875371084827">

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

   <tr id="row966121230084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p760668688084827">

iproxy_client.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1487505542084827">

Provides the client proxy class.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row462795068084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1616108859084827">

iproxy_server.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1330847962084827">

Provides the server proxy.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row735174859084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1879483444084827">

registry.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1052238857084827">

Provides basic APIs for remote service registration and discovery.

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

   <tr id="row1689214566084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2040265981084827">

Data Structure Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p838376888084827">

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

   <tr id="row406418592084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1843435540084827">

IClientProxy

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p489200166084827">

Defines the client proxy object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row823064937084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p282270800084827">

IServerProxy

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p128699271084827">

Defines the base class of the server proxy object.

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

   <tr id="row664104587084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2066816544084827">

Macro Name and Value

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p989331980084827">

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

   <tr id="row728499191084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1190737157084827">

INHERIT_CLIENT_IPROXY

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p955300597084827">

Indicates the inherited macro of the client proxy.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row895390647084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1219145845084827">

INHERIT_IPROXY_ENTRY(T) INHERIT_IUNKNOWNENTRY(T)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p956801964084827">

Inherits the server proxy class.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1893607541084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2132985730084827">

IPROXY_END IUNKNOWN_ENTRY_END

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1600849810084827">

Defines the end of the default initialization for the server proxy
class.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1061006930084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1817411649084827">

SERVER_PROXY_VER 0x80

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p791563653084827">

Defines the default version number of the server proxy.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row112252814084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p232443474084827">

INHERIT_SERVER_IPROXY

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p467422827084827">

Inherits the server proxy function.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2119385925084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p982839624084827">

SERVER_IPROXY_BEGIN IUNKNOWN_ENTRY_BEGIN(SERVER_PROXY_VER)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p50798851084827">

Defines the beginning of the default initialization for the server proxy
class.

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

   <tr id="row213166280084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1183586096084827">

Typedef Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1847727698084827">

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

   <tr id="row961452718084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p35474087084827">

INotify) (IOwner owner, int code, IpcIo \*reply)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1912193013084827">

typedef int(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p2046656237084827">

Called when a client request is responded.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2141509408084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p794523028084827">

Creator) (const char *service, const char*\ feature, uint32 size)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p562864898084827">

typedef void *(*

.. raw:: html

   </p>

.. raw:: html

   <p id="p419254573084827">

Indicates the creator of the customized client proxy.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1206785248084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1726427226084827">

Destroyer) (const char *service, const char*\ feature, void \*iproxy)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1669680763084827">

typedef void(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p2134877405084827">

Indicates the destroyer of the customized client proxy.

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

   <tr id="row284964100084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p748639525084827">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1333946739084827">

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

   <tr id="row1111232572084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p379448324084827">

SAMGR_GetRemoteIdentity (const char *service, const char*\ feature)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2108620922084827">

SvcIdentity

.. raw:: html

   </p>

.. raw:: html

   <p id="p1682349934084827">

Obtains the IPC address of a remote service and feature based on the
service name and feature name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row317447451084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2121296929084827">

SAMGR_RegisterFactory (const char *service, const char*\ feature,
Creator creator, Destroyer destroyer)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p304287369084827">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p601742178084827">

Registers the factory method of the client proxy object with the Samgr.

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

INHERIT_CLIENT_IPROXY
---------------------

::

   #define INHERIT_CLIENT_IPROXY

::

   Values: [INHERIT_IUNKNOWN](samgr.md#gab74532a22d6993d0ffc014d36253397f); \

    int (*Invoke)([IClientProxy](iclientproxy.md) *proxy, int funcId, IpcIo *request, IOwner owner, [INotify](registry.md#ga362a17c1bda1aace88d42dcbc88bdfac) notify)

**Description:**

Indicates the inherited macro of the client proxy.

This constant is used when a client proxy needs to be customized or
generated by a tool.

INHERIT_IPROXY_ENTRY
--------------------

::

   #define INHERIT_IPROXY_ENTRY( T)   [INHERIT_IUNKNOWNENTRY](samgr.md#gad6324fd90dd636180efa2a59b377e65c)(T)

**Description:**

Inherits the server proxy class.

When the server provides cross-process system capabilities, it uses
**INHERIT_IPROXY_ENTRY** to define the server proxy class.

INHERIT_SERVER_IPROXY
---------------------

::

   #define INHERIT_SERVER_IPROXY

::

   Values: [INHERIT_IUNKNOWN](samgr.md#gab74532a22d6993d0ffc014d36253397f); \

    int32 (*Invoke)([IServerProxy](iserverproxy.md) *iProxy, int funcId, void *origin, IpcIo *req, IpcIo *reply)

**Description:**

Inherits the server proxy function.

When the server provides cross-process system capabilities, it uses
**INHERIT_SERVER_IPROXY** to define the server proxy function.

IPROXY_END
----------

::

   #define IPROXY_END   [IUNKNOWN_ENTRY_END](samgr.md#ga4ef734474ece49aa938d8ebd5b54bdb3)

**Description:**

Defines the end of the default initialization for the server proxy
class.

This macro is used for developing the server proxy class. You can
inherit this macro to reduce the code amount and prevent class
definition inconsistency.

SERVER_IPROXY_BEGIN
-------------------

::

   #define SERVER_IPROXY_BEGIN   [IUNKNOWN_ENTRY_BEGIN](samgr.md#ga52ec6b5b03d56b0dfe7277785246bda1)([SERVER_PROXY_VER](registry.md#gad513d97bfb873f27c9b8f69a5a418d55))

**Description:**

Defines the beginning of the default initialization for the server proxy
class.

This macro is used for developing the server proxy class. You can
inherit this macro to reduce the code amount and prevent class
definition inconsistency.

SERVER_PROXY_VER
----------------

::

   #define SERVER_PROXY_VER   0x80

**Description:**

Defines the default version number of the server proxy.

The cross-process system capabilities are registered when Samgr uses
**SERVER_PROXY_VER** to query the registered server proxy.

**Typedef Documentation**\ 
---------------------------

Creator
-------

::

   typedef void*(* Creator) (const char *service, const char *feature, uint32 size)

**Description:**

Indicates the creator of the customized client proxy.

This macro creates a local client proxy for remote service APIs. If you
want to call the remote APIs in the way that local APIs are called,
implement this macro to encapsulate serialized data into the proxy. The
system automatically calls this macro when creating a proxy object.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2017480942084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2118264534084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p284304334084827">

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

   <tr id="row1788198904084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

service

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the name of the service to which the function
belongs.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1671598904084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

feature

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the name of the feature to which the function
belongs.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2010378390084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

size

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the size of the head to be added when a client proxy is
created. The required memory capacity is the head size plus the object
size.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

void \* Returns the applied memory capacity and initialize the memory
for the client proxy.

Destroyer
---------

::

   typedef void(* Destroyer) (const char *service, const char *feature, void *iproxy)

**Description:**

Indicates the destroyer of the customized client proxy.

This macro destroys local client proxy for remote service APIs. If you
want to call the remote APIs in the way that local APIs are called,
implement this macro to encapsulate serialized data into the proxy. The
system automatically calls this macro when destroying a proxy object.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1059402118084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1638408950084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p19697541084827">

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

   <tr id="row1250788881084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

service

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the name of the service to which the function
belongs.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row503561448084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

feature

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the name of the feature to which the function
belongs.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row276166625084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

iproxy

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the start address of the memory that is applied
by Creator.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

INotify
-------

::

   typedef int(* INotify) (IOwner owner, int code, IpcIo *reply)

**Description:**

Called when a client request is responded.

The client implements this **INotify** callback to receive response data
from the server. **owner** indicates the client proxy that receives the
response data; **code** indicates the error code of the response data
from the server; **reply** indicates the response data.

**Function Documentation**\ 
----------------------------

SAMGR_GetRemoteIdentity()
-------------------------

::

   SvcIdentity SAMGR_GetRemoteIdentity (const char * service, const char * feature )

**Description:**

Obtains the IPC address of a remote service and feature based on the
service name and feature name.

This function is used when `IClientProxy <iclientproxy.md>`__ cannot
meet your requirements for calling IPCs. For example, if you need to
receive the death notification of a remote service or feature, you can
call this function to obtain the address of the remote service or
feature and subscribe to the death notification from the IPC.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1241772755084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1095716672084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1984256719084827">

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

   <tr id="row525146671084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

service

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the name of the remote service.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row804508936084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

feature

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the name of the remote feature.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the IPC address of the remote service or feature. When the
handle of the obtained address structure **SvcIdentity** is
**0xFFFFFFFF**, the address is invalid.

**Attention:**

This function can be called only after **GetFeatureApi** in
`SamgrLite <samgrlite.md>`__ is successfully called. Otherwise, an
invalid address is returned. When the service or feature does not
support IPC communication, an invalid address will be returned.

SAMGR_RegisterFactory()
-----------------------

::

   int SAMGR_RegisterFactory (const char * service, const char * feature, [Creator](registry.md#ga0c8aa2ef9883bd97b4f1309895adaa4c) creator, [Destroyer](registry.md#ga1e6298b1246357f70ad0b581e0eb9305) destroyer )

**Description:**

Registers the factory method of the client proxy object with the Samgr.

If you want to call the remote APIs in the way that local APIs are
called, implement this function to encapsulate serialized data into the
proxy. During system initialization, the module that uses the remote
proxy calls the function as required.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row481271593084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p760675351084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p454843587084827">

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

   <tr id="row1428800229084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

service

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the service name of the client proxy.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1363604020084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

feature

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the feature name of the client proxy.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row150709120084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

creator

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the Creator function of the client proxy.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1754737552084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

destroyer

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the Destroyer function of the client proxy.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **EC_SUCCESS** if the registration is successful; returns other
error codes if the registration fails.
