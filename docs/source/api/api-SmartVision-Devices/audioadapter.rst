AudioAdapter
============

**Overview**\ 
--------------

**Related Modules:**

`Audio <audio.md>`__

**Description:**

Provides audio adapter capabilities, including initializing ports,
creating rendering and capturing tasks, and obtaining the port
capability set.

**Since:**

1.0

**Version:**

1.0

**Summary**\ 
-------------

Data Fields
-----------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1588744881093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2091697081093529">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p120274640093529">

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

   <tr id="row248311549093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1232248440093529">

InitAllPorts )(struct AudioAdapter \*adapter)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p598107548093529">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1979261033093529">

Initializes all ports of an audio adapter.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1578919531093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2095483610093529">

CreateRender )(struct AudioAdapter *adapter, const struct
AudioDeviceDescriptor*\ desc, const struct AudioSampleAttributes
\*attrs, struct AudioRender \**render)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1321298553093529">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p2051413093529">

Creates an AudioRender object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1930427928093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1979069192093529">

DestroyRender )(struct AudioAdapter *adapter, struct
AudioRender*\ render)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p433030640093529">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1511403336093529">

Destroys an AudioRender object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row394017211093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1141353875093529">

CreateCapture )(struct AudioAdapter *adapter, const struct
AudioDeviceDescriptor*\ desc, const struct AudioSampleAttributes
\*attrs, struct AudioCapture \**capture)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p702542483093529">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p283582026093529">

Creates an AudioCapture object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1131785240093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p17211529093529">

DestroyCapture )(struct AudioAdapter *adapter, struct
AudioCapture*\ capture)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2030831733093529">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p2047373094093529">

Destroys an AudioCapture object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1923185202093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p168289033093529">

GetPortCapability )(struct AudioAdapter *adapter, const struct
AudioPort*\ port, struct AudioPortCapability \*capability)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2025521960093529">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p2137140893093529">

Obtains the capability set of the port driver for the audio adapter.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row5611995093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1207872433093529">

SetPassthroughMode )(struct AudioAdapter *adapter, const struct
AudioPort*\ port, enum AudioPortPassthroughMode mode)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1701476356093529">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1891670679093529">

Sets the passthrough data transmission mode of the audio port driver.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row708431657093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1105861462093529">

GetPassthroughMode )(struct AudioAdapter *adapter, const struct
AudioPort*\ port, enum AudioPortPassthroughMode \*mode)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p984756588093529">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p635110041093529">

Obtains the passthrough data transmission mode of the audio port driver.

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

CreateCapture
-------------

::

   int32_t(* AudioAdapter::CreateCapture) (struct [AudioAdapter](audioadapter.md) *adapter, const struct [AudioDeviceDescriptor](audiodevicedescriptor.md) *desc, const struct [AudioSampleAttributes](audiosampleattributes.md) *attrs, struct [AudioCapture](audiocapture.md) **capture)

**Description:**

Creates an `AudioCapture <audiocapture.md>`__ object.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row741826260093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p53065450093529">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1121781333093529">

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

   <tr id="row595104207093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

adapter

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the audio adapter to operate.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1820488407093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

desc

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the descriptor of the audio adapter to start.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row152565446093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

attrs

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the audio sampling attributes to open.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1563208241093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

capture

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the double pointer to the AudioCapture object.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the `AudioCapture <audiocapture.md>`__ object is
created successfully; returns a negative value otherwise.

**See also:**

`GetPortCapability <audioadapter.md#a525ec7f3f3bb9975790e27f75145d0f6>`__

CreateRender
------------

::

   int32_t(* AudioAdapter::CreateRender) (struct [AudioAdapter](audioadapter.md) *adapter, const struct [AudioDeviceDescriptor](audiodevicedescriptor.md) *desc, const struct [AudioSampleAttributes](audiosampleattributes.md) *attrs, struct [AudioRender](audiorender.md) **render)

**Description:**

Creates an `AudioRender <audiorender.md>`__ object.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1990641944093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1884553925093529">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1170544726093529">

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

   <tr id="row577617420093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

adapter

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the audio adapter to operate.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1647166663093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

desc

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the descriptor of the audio adapter to start.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row813188173093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

attrs

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the audio sampling attributes to open.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1846563500093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

render

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the double pointer to the AudioRender object.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the `AudioRender <audiorender.md>`__ object is created
successfully; returns a negative value otherwise.

**See also:**

`GetPortCapability <audioadapter.md#a525ec7f3f3bb9975790e27f75145d0f6>`__

DestroyCapture
--------------

::

   int32_t(* AudioAdapter::DestroyCapture) (struct [AudioAdapter](audioadapter.md) *adapter, struct [AudioCapture](audiocapture.md) *capture)

**Description:**

Destroys an `AudioCapture <audiocapture.md>`__ object.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row147817294093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1914011374093529">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p603528269093529">

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

   <tr id="row134151341093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

adapter

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the audio adapter to operate.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1538219665093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

capture

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the AudioCapture object to operate.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Attention:**

Do not destroy the object during audio capturing.

**Returns:**

Returns **0** if the `AudioCapture <audiocapture.md>`__ object is
destroyed; returns a negative value otherwise.

**See also:**

`CreateCapture <audioadapter.md#a8a46358cdad8e0a9d15ac079713535f2>`__

DestroyRender
-------------

::

   int32_t(* AudioAdapter::DestroyRender) (struct [AudioAdapter](audioadapter.md) *adapter, struct [AudioRender](audiorender.md) *render)

**Description:**

Destroys an `AudioRender <audiorender.md>`__ object.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row363358699093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p343241280093529">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p677888803093529">

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

   <tr id="row1339057211093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

adapter

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the audio adapter to operate.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row551651422093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

render

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the AudioRender object to operate.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Attention:**

Do not destroy the object during audio rendering.

**Returns:**

Returns **0** if the `AudioRender <audiorender.md>`__ object is
destroyed; returns a negative value otherwise.

**See also:**

`CreateRender <audioadapter.md#a284ea2ad18ebac562ca7283652e61b50>`__

GetPassthroughMode
------------------

::

   int32_t(* AudioAdapter::GetPassthroughMode) (struct [AudioAdapter](audioadapter.md) *adapter, const struct [AudioPort](audioport.md) *port, enum [AudioPortPassthroughMode](audio.md#ga186d2d4f9a2ecacb80cd2cce2bd26f0e) *mode)

**Description:**

Obtains the passthrough data transmission mode of the audio port driver.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1839187508093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1167318499093529">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p511000365093529">

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

   <tr id="row955125389093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

adapter

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the audio adapter to operate.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row806029126093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

port

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the port.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1123463413093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

mode

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the passthrough transmission mode to obtain.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the mode is successfully obtained; returns a negative
value otherwise.

**See also:**

`SetPassthroughMode <audioadapter.md#ac4e77085cdcc853de832a2b16b8dc69a>`__

GetPortCapability
-----------------

::

   int32_t(* AudioAdapter::GetPortCapability) (struct [AudioAdapter](audioadapter.md) *adapter, const struct [AudioPort](audioport.md) *port, struct [AudioPortCapability](audioportcapability.md) *capability)

**Description:**

Obtains the capability set of the port driver for the audio adapter.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1848349352093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1063966956093529">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p290167071093529">

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

   <tr id="row690529570093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

adapter

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the audio adapter to operate.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row600527139093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

port

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the port.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1577303219093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

capability

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the capability set to obtain.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the capability set is successfully obtained; returns a
negative value otherwise.

InitAllPorts
------------

::

   int32_t(* AudioAdapter::InitAllPorts) (struct [AudioAdapter](audioadapter.md) *adapter)

**Description:**

Initializes all ports of an audio adapter.

Call this function before calling other driver functions to check
whether the initialization is complete. If the initialization is not
complete, wait for a while (for example, 100 ms) and perform the check
again until the port initialization is complete.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row303632622093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p720824060093529">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p182933896093529">

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

   <tr id="row1792937114093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

adapter

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the audio adapter to operate.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the initialization is successful; returns a negative
value otherwise.

SetPassthroughMode
------------------

::

   int32_t(* AudioAdapter::SetPassthroughMode) (struct [AudioAdapter](audioadapter.md) *adapter, const struct [AudioPort](audioport.md) *port, enum [AudioPortPassthroughMode](audio.md#ga186d2d4f9a2ecacb80cd2cce2bd26f0e) mode)

**Description:**

Sets the passthrough data transmission mode of the audio port driver.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1057469914093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1166340731093529">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1137241494093529">

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

   <tr id="row2107807824093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

adapter

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the audio adapter to operate.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1337795731093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

port

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the port.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2069723204093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

mode

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the passthrough transmission mode to set.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the setting is successful; returns a negative value
otherwise.

**See also:**

`GetPassthroughMode <audioadapter.md#ad4c41f3193c5ec3da254f33e24241ea6>`__
