KAL
===

**Overview**\ 
--------------

Defines the kernel adaptation layer (KAL), which provides compatible
interfaces across different types of OpenHarmony devices.

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

   <tr id="row1279671087090250">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p168151700090250">

File Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2010788671090250">

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

   <tr id="row946968834090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p899763654090250">

kal.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p291437502090250">

Defines the kernel adaptation layer (KAL), which provides compatible
interfaces across different types of OpenHarmony devices.

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

   <tr id="row1539818328090250">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1619231771090250">

Data Structure Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p18258118090250">

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

   <tr id="row1588051321090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1568692327090250">

ThreadInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1172898798090250">

Describes a thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1594931788090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1638947350090250">

MemInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p743878453090250">

Describes a memory pool.

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

   <tr id="row2024385192090250">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1733199826090250">

Macro Name and Value

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1608692438090250">

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

   <tr id="row837841792090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p972708954090250">

KAL_TASK_NAME_LEN 32

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p875345772090250">

Indicates the maximum length of a thread name.

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

   <tr id="row876615543090250">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p39172838090250">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1647185032090250">

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

   <tr id="row51807949090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1155384547090250">

KalTimerType { KAL_TIMER_ONCE = 0, KAL_TIMER_PERIODIC = 1 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1925187365090250">

Enumerates timer types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row62757079090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p496220096090250">

KalErrCode { KAL_OK = 0, KAL_ERR_PARA = 1, KAL_ERR_INNER = 2,
KAL_ERR_TIMER_STATE = 0x100 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1470168769090250">

Enumerates return values of the KAL function.

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

   <tr id="row1485283083090250">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p160108447090250">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p661992638090250">

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

   <tr id="row1341192174090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p773017751090250">

KalThreadGetInfo (unsigned int threadId, ThreadInfo \*info)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p143674785090250">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p349672349090250">

Obtains thread information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row193746428090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2091595061090250">

KalDelayUs (unsigned int us)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1673294868090250">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1083838878090250">

Delays a thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1582032518090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1392107112090250">

KalTimerCreate (KalTimerProc func, KalTimerType type, void \*arg,
unsigned int ticks)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1327550482090250">

KalTimerId

.. raw:: html

   </p>

.. raw:: html

   <p id="p1323777792090250">

Creates a timer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1051518793090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p387785760090250">

KalTimerStart (KalTimerId timerId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p705703207090250">

KalErrCode

.. raw:: html

   </p>

.. raw:: html

   <p id="p1110952124090250">

Starts a timer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1708085358090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1571623932090250">

KalTimerChange (KalTimerId timerId, unsigned int ticks)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p405299670090250">

KalErrCode

.. raw:: html

   </p>

.. raw:: html

   <p id="p1724878930090250">

Changes the duration of a timer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row583760966090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p369584604090250">

KalTimerStop (KalTimerId timerId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p747521935090250">

KalErrCode

.. raw:: html

   </p>

.. raw:: html

   <p id="p2004415637090250">

Stops a timer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1980928763090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1283503038090250">

KalTimerDelete (KalTimerId timerId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1706798424090250">

KalErrCode

.. raw:: html

   </p>

.. raw:: html

   <p id="p1346894623090250">

Deletes a timer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row409991002090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1836721559090250">

KalTimerIsRunning (KalTimerId timerId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p858486404090250">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p2113773278090250">

Checks whether a timer is running.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2137173366090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1918730907090250">

KalTickToMs (unsigned int ticks)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p459689953090250">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1285882106090250">

Converts system ticks into milliseconds.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row468227279090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p328827607090250">

KalMsToTick (unsigned int millisec)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p722263099090250">

unsigned int

.. raw:: html

   </p>

.. raw:: html

   <p id="p472525132090250">

Converts milliseconds into system ticks.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row716309176090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1713488711090250">

KalGetMemInfo (MemInfo \*pmemInfo)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p801026788090250">

KalErrCode

.. raw:: html

   </p>

.. raw:: html

   <p id="p1090848409090250">

Obtains memory information.

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

**Enumeration Type Documentation**\ 
------------------------------------

KalErrCode
----------

::

   enum [KalErrCode](kal.md#ga595e811b5dcad5dc834be507d6839c36)

**Description:**

Enumerates return values of the KAL function.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row288199108090250">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1657223263090250">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2016480901090250">

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

   <tr id="row781539680090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry1587560209090250p0">

KAL_OK

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p497584006090250">

A successful execution

.. raw:: html

   </p>

.. raw:: html

   <p id="p11440164110316">

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1485168917090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry21551412090250p0">

KAL_ERR_PARA

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2070007331090250">

Incorrect parameter

.. raw:: html

   </p>

.. raw:: html

   <p id="p1144010419313">

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1406949664090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry641308078090250p0">

KAL_ERR_INNER

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p539868235090250">

Internal execution error

.. raw:: html

   </p>

.. raw:: html

   <p id="p1544015411732">

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1850551987090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry592386261090250p0">

KAL_ERR_TIMER_STATE

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1767284033090250">

Timer status error

.. raw:: html

   </p>

.. raw:: html

   <p id="p6440241631">

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

KalTimerType
------------

::

   enum [KalTimerType](kal.md#gacde4b0c553c297f66311b87c4bbbb27d)

**Description:**

Enumerates timer types.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row329519887090250">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p627432540090250">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1360280359090250">

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

   <tr id="row323851035090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry1676693334090250p0">

KAL_TIMER_ONCE

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1919223126090250">

One-shot timer

.. raw:: html

   </p>

.. raw:: html

   <p id="p1544854112318">

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row232535340090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry1464454772090250p0">

KAL_TIMER_PERIODIC

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1168641856090250">

Repetitive timer

.. raw:: html

   </p>

.. raw:: html

   <p id="p6448841430">

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

KalDelayUs()
------------

::

   void KalDelayUs (unsigned int us)

**Description:**

Delays a thread.

The delay unit is microsecond. The actual delay precision can reach only
the tick level.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row357148926090250">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p956450764090250">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1134305722090250">

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

   <tr id="row45825837090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry537415473090250p0">

us

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="entry104061947090250p0">

Indicates the number of microseconds to delay. The actual delay
precision is one tick.

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

KalGetMemInfo()
---------------

::

   [KalErrCode](kal.md#ga595e811b5dcad5dc834be507d6839c36) KalGetMemInfo ([MemInfo](meminfo.md) * pmemInfo)

**Description:**

Obtains memory information.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row991660390090250">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p299526827090250">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1383934611090250">

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

   <tr id="row1222934779090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry1937117894090250p0">

pmemInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="entry315786093090250p0">

Indicates the pointer to the memory information.

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

**Returns:**

Returns an enumerated value defined by
`KalErrCode <kal.md#ga595e811b5dcad5dc834be507d6839c36>`__, where
`KAL_OK <kal.md#gga595e811b5dcad5dc834be507d6839c36a249642877a22187565c646fcb4c43228>`__
indicates a success.

KalMsToTick()
-------------

::

   unsigned int KalMsToTick (unsigned int millisec)

**Description:**

Converts milliseconds into system ticks.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1808476861090250">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p195586487090250">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2029168273090250">

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

   <tr id="row1612627690090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry229984854090250p0">

millisec

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="entry62392545090250p0">

Indicates the milliseconds to convert.

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

**Returns:**

Returns the system ticks generated.

KalThreadGetInfo()
------------------

::

   unsigned int KalThreadGetInfo (unsigned int threadId, [ThreadInfo](threadinfo.md) * info )

**Description:**

Obtains thread information.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row157772410090250">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p517328145090250">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p320788349090250">

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

   <tr id="row635552821090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry1075927755090250p0">

threadId

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="entry559539319090250p0">

Indicates the thread ID.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1074772122090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry750154741090250p0">

info

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="entry1525186157090250p0">

Indicates the pointer to the buffer for storing the obtained thread
information.

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

**Returns:**

Returns **0** if the thread information is obtained; returns a negative
value otherwise.

KalTickToMs()
-------------

::

   unsigned int KalTickToMs (unsigned int ticks)

**Description:**

Converts system ticks into milliseconds.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1394740911090250">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1405376294090250">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1399565358090250">

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

   <tr id="row1086265717090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry1312544656090250p0">

ticks

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="entry387467238090250p0">

Indicates the number of ticks to convert.

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

**Returns:**

Returns the milliseconds generated.

KalTimerChange()
----------------

::

   [KalErrCode](kal.md#ga595e811b5dcad5dc834be507d6839c36) KalTimerChange (KalTimerId timerId, unsigned int ticks )

**Description:**

Changes the duration of a timer.

The timer duration can be changed only before the timer is started.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row837457968090250">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p306638110090250">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1010028081090250">

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

   <tr id="row221792356090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry794316212090250p0">

timerId

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="entry632643054090250p0">

Indicates the ID of the timer whose duration is to change, which is the
value returned by KalTimerCreate.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1115890167090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry166423821090250p0">

ticks

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="entry763994554090250p0">

Indicates the new duration of the timer.

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

**Returns:**

Returns an enumerated value defined by
`KalErrCode <kal.md#ga595e811b5dcad5dc834be507d6839c36>`__, where
`KAL_OK <kal.md#gga595e811b5dcad5dc834be507d6839c36a249642877a22187565c646fcb4c43228>`__
indicates a success.

KalTimerCreate()
----------------

::

   KalTimerId KalTimerCreate (KalTimerProc func, [KalTimerType](kal.md#gacde4b0c553c297f66311b87c4bbbb27d) type, void * arg, unsigned int ticks )

**Description:**

Creates a timer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row495685141090250">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1356842829090250">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1517717949090250">

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

   <tr id="row1666700858090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry226656396090250p0">

func

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="entry580079398090250p0">

Indicates the entry to timer callback. The callback is triggered when
the timer expires.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1723323089090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry1477381166090250p0">

type

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="entry1519720414090250p0">

Indicates the timer type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row572683528090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry786468104090250p0">

arg

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="entry1024218162090250p0">

Indicates the pointer to the argument used in timer callback.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row638953725090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry807210750090250p0">

ticks

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="entry1544463044090250p0">

Indicates the duration of the timer to create.

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

**Returns:**

Returns the timer ID; returns **NULL** in the case of an error.

KalTimerDelete()
----------------

::

   [KalErrCode](kal.md#ga595e811b5dcad5dc834be507d6839c36) KalTimerDelete (KalTimerId timerId)

**Description:**

Deletes a timer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row241534207090250">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1478794303090250">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1618646052090250">

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

   <tr id="row1064898631090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry194406456090250p0">

timerId

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="entry1655546368090250p0">

Indicates the ID of the timer to delete, which is the value returned by
KalTimerCreate.

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

**Returns:**

Returns an enumerated value defined by
`KalErrCode <kal.md#ga595e811b5dcad5dc834be507d6839c36>`__, where
`KAL_OK <kal.md#gga595e811b5dcad5dc834be507d6839c36a249642877a22187565c646fcb4c43228>`__
indicates a success.

KalTimerIsRunning()
-------------------

::

   unsigned int KalTimerIsRunning (KalTimerId timerId)

**Description:**

Checks whether a timer is running.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1285460878090250">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1575744244090250">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1006271401090250">

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

   <tr id="row1453707987090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry1047186589090250p0">

timerId

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="entry1421223117090250p0">

Indicates the ID of the timer to check, which is the value returned by
KalTimerCreate.

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

**Returns:**

Returns **1** if the timer is running; returns **0** if the timer is not
running or the input parameter is incorrect.

KalTimerStart()
---------------

::

   [KalErrCode](kal.md#ga595e811b5dcad5dc834be507d6839c36) KalTimerStart (KalTimerId timerId)

**Description:**

Starts a timer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row15726364090250">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p313569381090250">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p792177544090250">

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

   <tr id="row91856712090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry385879940090250p0">

timerId

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="entry377521522090250p0">

Indicates the ID of the timer to start, which is the value returned by
KalTimerCreate.

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

**Returns:**

Returns an enumerated value defined by
`KalErrCode <kal.md#ga595e811b5dcad5dc834be507d6839c36>`__, where
`KAL_OK <kal.md#gga595e811b5dcad5dc834be507d6839c36a249642877a22187565c646fcb4c43228>`__
indicates a success.

KalTimerStop()
--------------

::

   [KalErrCode](kal.md#ga595e811b5dcad5dc834be507d6839c36) KalTimerStop (KalTimerId timerId)

**Description:**

Stops a timer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1103151354090250">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1293557509090250">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2106193107090250">

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

   <tr id="row560498489090250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="entry334876843090250p0">

timerId

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="entry1806602586090250p0">

Indicates the ID of the timer to stop, which is the value returned by
KalTimerCreate.

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

**Returns:**

Returns an enumerated value defined by
`KalErrCode <kal.md#ga595e811b5dcad5dc834be507d6839c36>`__, where
`KAL_OK <kal.md#gga595e811b5dcad5dc834be507d6839c36a249642877a22187565c646fcb4c43228>`__
indicates a success.

**Variable Documentation**\ 
----------------------------

bottomOfStack
-------------

::

   unsigned int ThreadInfo::bottomOfStack

**Description:**

Thread stack bottom

currUsed
--------

::

   unsigned int ThreadInfo::currUsed

**Description:**

Current stack space usage

eventMask
---------

::

   unsigned int ThreadInfo::eventMask

**Description:**

Thread event mask

eventStru
---------

::

   unsigned int ThreadInfo::eventStru[3]

**Description:**

Thread event

free
----

::

   unsigned int MemInfo::free

**Description:**

Available space of the memory pool, in bytes

freeLmp
-------

::

   unsigned int MemInfo::freeLmp

**Description:**

Available space of the small memory pool, in bytes

freeNodeNum
-----------

::

   unsigned int MemInfo::freeNodeNum

**Description:**

Number of available nodes in the memory pool

id
--

::

   unsigned int ThreadInfo::id

**Description:**

Thread ID

mallocFailCount
---------------

::

   unsigned int MemInfo::mallocFailCount

**Description:**

Number of memory allocation failures

maxFreeNodeSize
---------------

::

   unsigned int MemInfo::maxFreeNodeSize

**Description:**

Size of the largest available node in the memory pool, in bytes

mepc
----

::

   unsigned int ThreadInfo::mepc

**Description:**

Current thread MEPC

mstatus
-------

::

   unsigned int ThreadInfo::mstatus

**Description:**

Current thread status

name
----

::

   char ThreadInfo::name[[KAL_TASK_NAME_LEN](kal.md#ga5c36b53bd6e8cbdbcd79f702eda94fdc)]

**Description:**

Thread name

overflowFlag
------------

::

   unsigned int ThreadInfo::overflowFlag

**Description:**

Thread stack overflow flag

peakUsed
--------

::

   unsigned int ThreadInfo::peakUsed

**Description:**

Peak stack space usage

peekSize
--------

::

   unsigned int MemInfo::peekSize

**Description:**

Peak memory usage of the memory pool

priority
--------

::

   unsigned short ThreadInfo::priority

**Description:**

Thread priority

ra
--

::

   unsigned int ThreadInfo::ra

**Description:**

Current thread RA

sp
--

::

   unsigned int ThreadInfo::sp

**Description:**

Thread stack pointer

stackSize
---------

::

   unsigned int ThreadInfo::stackSize

**Description:**

Thread stack size

status
------

::

   unsigned short ThreadInfo::status

**Description:**

Thread status

taskMutex
---------

::

   void* ThreadInfo::taskMutex

**Description:**

Thread mutex

taskSem
-------

::

   void* ThreadInfo::taskSem

**Description:**

Thread semaphore

topOfStack
----------

::

   unsigned int ThreadInfo::topOfStack

**Description:**

Thread stack top

total
-----

::

   unsigned int MemInfo::total

**Description:**

Total space of the memory pool, in bytes

totalLmp
--------

::

   unsigned int MemInfo::totalLmp

**Description:**

Total space of the small memory pool, in bytes

tp
--

::

   unsigned int ThreadInfo::tp

**Description:**

Current thread TP

used
----

::

   unsigned int MemInfo::used

**Description:**

Used space of the memory pool, in bytes

usedLmp
-------

::

   unsigned int MemInfo::usedLmp

**Description:**

Used space of the small memory pool, in bytes

usedNodeNum
-----------

::

   unsigned int MemInfo::usedNodeNum

**Description:**

Number of used nodes in the memory pool
