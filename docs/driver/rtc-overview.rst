RTC Overview
============

Introduction
------------

The real-time clock (RTC) driver provides precise real time for the
operating system (OS). If the OS is powered off, the RTC driver
continues to keep track of the system time using an external battery.

Available APIs
--------------

**Table 1** APIs provided by the RTC driver

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row4419501537">

.. raw:: html

   <th class="cellrowborder" valign="top" width="21.902190219021904%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p641050105320">

Capability

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="24.98249824982498%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p54150165315">

Function

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="53.11531153115312%" id="mcps1.2.4.1.3">

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

   <tr id="row17550163418501">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="21.902190219021904%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p11670643205012">

RTC handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="24.98249824982498%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p16550143465015">

RtcOpen

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.11531153115312%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p9550103415015">

Opens the RTC device to obtain its handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1879052755020">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1479062716506">

RtcClose

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1579142745012">

Releases a specified handle of the RTC device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row34145016535">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="21.902190219021904%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p229610227124">

RTC time

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="24.98249824982498%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p19389143041518">

RtcReadTime

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.11531153115312%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p8738101941716">

Reads time information from the RTC driver, including the year, month,
the day of the week, day, hour, minute, second, and millisecond.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row5632152611414">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p143890309153">

RtcWriteTime

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p573815197171">

Writes time information from the RTC driver, including the year, month,
the day of the week, day, hour, minute, second, and millisecond.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1468016592416">

.. raw:: html

   <td class="cellrowborder" rowspan="4" valign="top" width="21.902190219021904%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p36817591648">

RTC alarm

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="24.98249824982498%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p968116598418">

RtcReadAlarm

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.11531153115312%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p768110592416">

Reads the RTC alarm time that was set last time.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row19313155514">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p73141951155">

RtcWriteAlarm

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p15314656511">

Writes the RTC alarm time based on the alarm index.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row138283422555">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2829142165513">

RtcRegisterAlarmCallback

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p118291242155518">

Registers RtcAlarmCallback that will be invoked when an alarm is
generated at the specified time.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row13344113914568">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2344103915616">

RtcAlarmInterruptEnable

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p034415397565">

Enables or disables RTC alarm interrupts.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row11801203517565">

.. raw:: html

   <td class="cellrowborder" rowspan="3" valign="top" width="21.902190219021904%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p17261458942">

RTC configuration

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="24.98249824982498%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p15801153515561">

RtcGetFreq

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.11531153115312%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p980133515566">

Reads the frequency of the external crystal oscillator connected to the
RTC driver.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row111502322563">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1615073225618">

RtcSetFreq

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p10150832165613">

Sets the frequency of the external crystal oscillator connected to the
RTC driver.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row21771259145618">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1717725916562">

RtcReset

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p517712598569">

Resets the RTC.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row917116425716">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="21.902190219021904%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p144765201754">

Custom register

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="24.98249824982498%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1117110418570">

RtcReadReg

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.11531153115312%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1517114410578">

Reads the configuration of a custom RTC register based on the register
index.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row46738190576">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1567331910573">

RtcWriteReg

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1967391913576">

Writes the configuration of a custom RTC register based on the register
index.

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
