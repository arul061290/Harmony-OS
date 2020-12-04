Watchdog Overview
=================

Introduction
------------

A watchdog, also called a watchdog timer, is a hardware timing device.
If an error occurs in the main program of the system and fails to reset
the watchdog timer, the watchdog timer sends a reset signal to restore
the system to a normal state.

Available APIs
--------------

**Table 1** Watchdog APIs

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row4419501537">

.. raw:: html

   <th class="cellrowborder" valign="top" width="26.619999999999997%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p641050105320">

Capability

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="32.800000000000004%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p54150165315">

Function

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="40.58%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p941150145313">

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

   <tr id="row837081981712">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="26.619999999999997%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p681292481718">

Open/Close

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="32.800000000000004%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p183701419141710">

WatchdogOpen

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="40.58%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p17370161911710">

Opens a watchdog.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row5610415171719">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p661171510173">

WatchdogClose

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p11611715161713">

Closes a watchdog.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row337105133315">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="26.619999999999997%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p07631557153319">

Start/Stop

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="32.800000000000004%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p163765113337">

WatchdogStart

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="40.58%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p18376517332">

Starts a watchdog.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row18399184610337">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1740010461335">

WatchdogStop

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p19400194633318">

Stops a watchdog.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row34145016535">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="26.619999999999997%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p229610227124">

Timeout duration

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="32.800000000000004%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p8296182221219">

WatchdogSetTimeout

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="40.58%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p16297172213125">

Sets the watchdog timeout duration.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row11585016539">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1095722493616">

WatchdogGetTimeout

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p15297162215122">

Obtains the watchdog timeout duration.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row105701653185811">

.. raw:: html

   <td class="cellrowborder" valign="top" width="26.619999999999997%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2571145325819">

Status

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="32.800000000000004%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p175711953195814">

WatchdogGetStatus

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="40.58%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p331961319210">

Obtains the watchdog status.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1028182217215">

.. raw:: html

   <td class="cellrowborder" valign="top" width="26.619999999999997%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p182818227214">

Feeding

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="32.800000000000004%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p17281223219">

WatchdogFeed

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="40.58%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p62815221125">

Feeds a watchdog, or resets a watchdog timer.

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

..

   |image1| **NOTE:** All functions provided in this document can be
   called only in kernel mode.

.. |image1| image:: public_sys-resources/icon-note.gif
