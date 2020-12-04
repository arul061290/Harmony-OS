AudioManager
============

**Overview**\ 
--------------

**Related Modules:**

`Audio <audio.md>`__

**Description:**

Manages audio adapters through a specific adapter driver program loaded
based on the given audio adapter descriptor.

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

   <tr id="row713939675093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p273140907093529">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1021554312093529">

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

   <tr id="row748406243093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1733388767093529">

GetAllAdapters )(struct AudioManager \*manager, struct
AudioAdapterDescriptor \**descs, int32_t \*size)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2083020219093529">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1351898503093529">

Obtains the list of all adapters supported by an audio driver.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row668891931093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p813377886093529">

LoadAdapter )(struct AudioManager *manager, const struct
AudioAdapterDescriptor*\ desc, struct AudioAdapter \**adapter)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1268650350093529">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p104197628093529">

Loads the driver for an audio adapter.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row698057735093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p317899072093529">

UnloadAdapter )(struct AudioManager *manager, struct
AudioAdapter*\ adapter)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1982866854093529">

void(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1868168070093529">

Unloads the driver of an audio adapter.

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

GetAllAdapters
--------------

::

   int32_t(* AudioManager::GetAllAdapters) (struct [AudioManager](audiomanager.md) *manager, struct [AudioAdapterDescriptor](audioadapterdescriptor.md) **descs, int32_t *size)

**Description:**

Obtains the list of all adapters supported by an audio driver.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row729588104093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p551971613093529">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p546930465093529">

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

   <tr id="row160433142093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

manager

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the audio adapter manager to operate.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row523725233093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

descs

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the double pointer to the audio adapter list.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1066925309093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

size

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the length of the list.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the list is obtained successfully; returns a negative
value otherwise.

**See also:**

`LoadAdapter <audiomanager.md#ab090e9c760a2888b55acc7baa4222ccb>`__

LoadAdapter
-----------

::

   int32_t(* AudioManager::LoadAdapter) (struct [AudioManager](audiomanager.md) *manager, const struct [AudioAdapterDescriptor](audioadapterdescriptor.md) *desc, struct [AudioAdapter](audioadapter.md) **adapter)

**Description:**

Loads the driver for an audio adapter.

For example, to load a USB driver, you may need to load a dynamic-link
library (*.so) in specific implementation.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1525628476093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2042036607093529">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p548932665093529">

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

   <tr id="row753263546093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

manager

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the audio adapter manager to operate.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row382506739093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

desc

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the descriptor of the audio adapter.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row552897463093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

adapter

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the double pointer to the audio adapter.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the driver is loaded successfully; returns a negative
value otherwise.

**See also:**

`GetAllAdapters <audiomanager.md#a93a0ffb0df907fabcfca827d31dadf39>`__

UnloadAdapter
-------------

::

   void(* AudioManager::UnloadAdapter) (struct [AudioManager](audiomanager.md) *manager, struct [AudioAdapter](audioadapter.md) *adapter)

**Description:**

Unloads the driver of an audio adapter.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1008245406093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1894088234093529">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p502549433093529">

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

   <tr id="row455725036093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

manager

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the audio adapter manager to operate.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1902824982093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

adapter

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the audio adapter whose driver will be
unloaded.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**See also:**

`LoadAdapter <audiomanager.md#ab090e9c760a2888b55acc7baa4222ccb>`__
