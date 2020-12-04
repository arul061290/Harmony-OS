AudioControl
============

**Overview**\ 
--------------

**Related Modules:**

`Audio <audio.md>`__

**Description:**

Provides control-related APIs for audio rendering or capturing,
including functions to start, stop, pause, and resume audio rendering or
capturing, and flush data in the audio buffer.

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

   <tr id="row105031931093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1376424132093529">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1206642964093529">

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

   <tr id="row1627808900093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p922727782093529">

Start )(AudioHandle handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1164116476093529">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p579336198093529">

Starts audio rendering or capturing.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row521428968093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1055060287093529">

Stop )(AudioHandle handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p380195099093529">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p74751282093529">

Stops audio rendering or capturing.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1037966422093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1543130650093529">

Pause )(AudioHandle handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1980836348093529">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1698706658093529">

Pauses audio rendering or capturing.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row339933741093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1087710218093529">

Resume )(AudioHandle handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1199755923093529">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1285224893093529">

Resumes audio rendering or capturing.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row742108357093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p286365082093529">

Flush )(AudioHandle handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p246705083093529">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1544741887093529">

Flushes data in the audio buffer.

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

Flush
-----

::

   int32_t(* AudioControl::Flush) ([AudioHandle](audio.md#ga18675ddb073465fdeac33a897f675d79) handle)

**Description:**

Flushes data in the audio buffer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2121388092093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p463612065093529">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1420316507093529">

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

   <tr id="row672252771093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the audio handle.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the flush is successful; returns a negative value
otherwise.

Pause
-----

::

   int32_t(* AudioControl::Pause) ([AudioHandle](audio.md#ga18675ddb073465fdeac33a897f675d79) handle)

**Description:**

Pauses audio rendering or capturing.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row705900441093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1153417946093529">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p267949451093529">

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

   <tr id="row1655868003093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the audio handle.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the rendering or capturing is successfully paused;
returns a negative value otherwise.

**See also:**

`Resume <audiocontrol.md#ac59c3e9a5ff9041989871f67253a1e8d>`__

Resume
------

::

   int32_t(* AudioControl::Resume) ([AudioHandle](audio.md#ga18675ddb073465fdeac33a897f675d79) handle)

**Description:**

Resumes audio rendering or capturing.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1196862347093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p683099292093529">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1743947570093529">

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

   <tr id="row1082952657093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the audio handle.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the rendering or capturing is successfully resumed;
returns a negative value otherwise.

**See also:**

`Pause <audiocontrol.md#a16a26deffa17b9f143f602763a260908>`__

Start
-----

::

   int32_t(* AudioControl::Start) ([AudioHandle](audio.md#ga18675ddb073465fdeac33a897f675d79) handle)

**Description:**

Starts audio rendering or capturing.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row719680072093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p543638970093529">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p756634070093529">

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

   <tr id="row75112197093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the audio handle.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the rendering or capturing is successfully started;
returns a negative value otherwise.

**See also:**

`Stop <audiocontrol.md#a62e385e391ba1efed35021ee67ab9449>`__

Stop
----

::

   int32_t(* AudioControl::Stop) ([AudioHandle](audio.md#ga18675ddb073465fdeac33a897f675d79) handle)

**Description:**

Stops audio rendering or capturing.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1309391234093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1218960347093529">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1312910437093529">

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

   <tr id="row144953910093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the audio handle.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the rendering or capturing is successfully stopped;
returns a negative value otherwise.

**See also:**

`Start <audiocontrol.md#a80ddae13819bb1eb348ad4b57597e930>`__
