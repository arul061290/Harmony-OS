OHOS::AbilitySlice
==================

**Overview**\ 
--------------

**Related Modules:**

`AbilityKit <abilitykit.rst>`__

**Description:**

Provides ability slice-related functions, including ability slice
lifecycle callbacks and functions for connecting to or disconnecting
from ability slices.

`AbilitySlice <ohos-abilityslice.rst>`__ instances, which are specific to
`Feature <feature.rst>`__ Abilities (abilities using the Page template),
are used to present different screens on an application’s user
interface. A `Feature <feature.rst>`__ `Ability <ohos-ability.rst>`__ can
have multiple ability slices.

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

   <tr id="row1663949583084837">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1400812627084837">

Public Member Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p37910540084837">

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

   <tr id="row1798588639084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p440301970084837">

OnStart (const Want &want)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p239140390084837">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1082765598084837">

Called when this ability slice is started. You must override this
function if you want to perform some initialization operations during
ability slice startup.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row785531619084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1167683978084837">

OnInactive ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p26951404084837">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1926189375084837">

Called when this ability slice enters the STATE_INACTIVE state.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2041052019084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1128450966084837">

OnActive (const Want &want)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p804268137084837">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p488575188084837">

Called when this ability slice enters the STATE_ACTIVE state.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1397836391084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1112691662084837">

OnBackground ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2069355139084837">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p714500478084837">

Called when this ability slice enters the STATE_BACKGROUND state.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row839857209084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1571662574084837">

OnStop ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1668413999084837">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1122191287084837">

Called when this ability slice enters the STATE_STOP state.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1810241435084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p730939495084837">

Present (AbilitySlice &abilitySlice, const Want &want)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p403061833084837">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p521673685084837">

Presents another ability slice, which can be an ability slice that is
not started or an existing ability slice in the host ability.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1629409147084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p895415330084837">

Terminate ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1855681230084837">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p907666617084837">

Destroys this ability slice.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2139516602084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1836873660084837">

SetUIContent (RootView \*rootView)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p192529349084837">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p794702795084837">

Sets the UI layout for the host ability of this ability slice.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1604649440084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1949670601084837">

StartAbility (const Want &want)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1945616858084837">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1003237868084837">

Starts an Ability based on the specified Want information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row245696537084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p200603645084837">

StopAbility (const Want &want)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p677624737084837">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p141337593084837">

Stops an Ability based on the specified Want information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row765954399084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1947372190084837">

TerminateAbility ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p746424397084837">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p516007695084837">

Destroys this Ability.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2094164944084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1287441996084837">

ConnectAbility (const Want &want, const IAbilityConnection &conn, void
\*data)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1468268496084837">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p229887534084837">

Connects to a Service ability based on the specified Want information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1366261528084837">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p864633735084837">

DisconnectAbility (const IAbilityConnection &conn)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1585533684084837">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1418375839084837">

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
