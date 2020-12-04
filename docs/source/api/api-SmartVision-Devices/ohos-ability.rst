OHOS::Ability
=============

**Overview**\ 
--------------

**Related Modules:**

`AbilityKit <abilitykit.md>`__

**Description:**

Declares ability-related functions, including ability lifecycle
callbacks and functions for connecting to or disconnecting from Particle
Abilities.

As the fundamental unit of OpenHarmony applications, abilities are
classified into `Feature <feature.md>`__ Abilities and Particle
Abilities. `Feature <feature.md>`__ Abilities support the Page template,
and Particle Abilities support the `Service <service.md>`__ template. An
ability using the Page template is called Page ability for short and
that using the `Service <service.md>`__ template is called
`Service <service.md>`__ ability.

**Since:**

1.0

**Version:**

1.0

**Summary**\ 
-------------

Public Member Functions
-----------------------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row747119158084837">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1495269378084837">

Public Member Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p767278114084837">

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

   <tr id="row971666805084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p690889432084837">

OnStart (const Want &want)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1788330887084837">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p145900818084837">

Called when this ability is started. You must override this function if
you want to perform some initialization operations during ability
startup.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1338585118084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p112623444084837">

OnInactive ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p386250391084837">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p599241652084837">

Called when this ability enters the STATE_INACTIVE state.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row671970770084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2031938534084837">

OnActive (const Want &want)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p174036397084837">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p752864652084837">

Called when this ability enters the STATE_ACTIVE state.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1070790822084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p469568606084837">

OnBackground ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p663751035084837">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1310143183084837">

Called when this ability enters the STATE_BACKGROUND state.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2094378171084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2144839750084837">

OnStop ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p875820415084837">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1581105768084837">

Called when this ability enters the STATE_STOP state.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row405658473084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1188587476084837">

OnConnect (const Want &want)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1748393321084837">

virtual const SvcIdentity \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1835864863084837">

Called when this Service ability is connected for the first time.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1313397070084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1377842411084837">

OnDisconnect (const Want &want)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1005398939084837">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p512605013084837">

Called when all abilities connected to this Service ability are
disconnected.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1920744543084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p221374941084837">

SetMainRoute (const std::string &entry)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1108282235084837">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p122714624084837">

Sets the main route for this ability.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2121053054084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p266775000084837">

SetUIContent (RootView \*rootView)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p818064272084837">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1617442157084837">

Sets the UI layout for this ability. You can call GetWindowRootView() to
create a layout and add controls.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1066046894084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1499633864084837">

MsgHandle (uint32_t funcId, IpcIo *request, IpcIo*\ reply)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1694861028084837">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p457647083084837">

Handles a message sent by the client to this Service ability.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row886288679084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1620451875084837">

Dump (const std::string &extra)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p555050195084837">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1486207241084837">

Prints ability information to the console.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row816190004084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p274908703084837">

StartAbility (const Want &want)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p980821791084837">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1612307854084837">

Starts an Ability based on the specified Want information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1580946774084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p740363199084837">

StopAbility (const Want &want)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2113552500084837">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p384412316084837">

Stops an Ability based on the specified Want information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1579162740084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p572465098084837">

TerminateAbility ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1794873218084837">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1333508519084837">

Destroys this Ability.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1231299292084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1811799733084837">

ConnectAbility (const Want &want, const IAbilityConnection &conn, void
\*data)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p832510986084837">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1452465091084837">

Connects to a Service ability based on the specified Want information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row276336280084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p647846189084837">

DisconnectAbility (const IAbilityConnection &conn)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1575274384084837">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1808052809084837">

Disconnects from a Service ability.

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
