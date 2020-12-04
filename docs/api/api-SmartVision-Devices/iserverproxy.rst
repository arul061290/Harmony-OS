IServerProxy
============

**Overview**\ 
--------------

**Related Modules:**

`Registry <registry.md>`__

**Description:**

Defines the base class of the server proxy object.

When the server provides cross-process system capabilities, it uses
**INHERIT_SERVER_IPROXY** to define the server proxy.

**Summary**\ 
-------------

Data Fields
-----------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row602411228093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1248951396093531">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p349887087093531">

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

   <tr id="row1515144113093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p86391199093531">

INHERIT_IUNKNOWN

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

  

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1596986543093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p439236462093531">

Invoke )(IServerProxy *iProxy, int funcId, void*\ origin, IpcIo *req,
IpcIo*\ reply)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1960918505093531">

int32(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p2087984609093531">

Unmarshals the IPC message received by the server.

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

**Field Documentation**\ 
-------------------------

INHERIT_IUNKNOWN
----------------

::

   IServerProxy::INHERIT_IUNKNOWN

**Description:**

This class inherits from `IUnknown <iunknown.md>`__.

Invoke
------

::

   int32(* IServerProxy::Invoke) ([IServerProxy](iserverproxy.md) *iProxy, int funcId, void *origin, IpcIo *req, IpcIo *reply)

**Description:**

Unmarshals the IPC message received by the server.

This function is implemented by developers and called by the system.
This function runs in the message processing thread of the service. Do
not block the message processing thread; otherwise, the function may
fail to be executed.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1187246595093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p967129292093531">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2099926678093531">

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

   <tr id="row1630857098093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

Proxy

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the server proxy object.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row742325200093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

funcId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the ID of the server function to be invoked by the client.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2072628977093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

origin

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the original IPC message, from which the header information
can be obtained.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2125531190093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

req

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

ipc Indicates the message body, from which data can be obtained.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1814045086093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

reply

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the output parameter, which is used to respond to the message.
The value can contain a maximum of five objects and 200 bytes.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **EC_SUCCESS** if the unmarshalling is successful; returns other
error codes if the unmarshalling fails.
