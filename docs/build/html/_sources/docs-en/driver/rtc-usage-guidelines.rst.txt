RTC Usage Guidelines
====================

How to Use
----------

During the OS startup, the HDF loads the RTC driver based on the
configuration file. The RTC driver detects the RTC component and
initializes the driver.

`Figure 1 <#fig166181128151112>`__ illustrates the process of an RTC
device.

**Figure 1** Process of using an RTC device

|image1|

Creating an RTC Device Handle
-----------------------------

After the RTC driver is loaded successfully, you can use the API
provided by the HDF and call APIs of the RTC driver.

   |image2| **NOTE:** Currently, only one RTC device is supported in the
   OS.

struct DevHandle \*RtcOpen(void);

**Table 1** Description of **RtcOpen**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row580722985616">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.45%">

.. raw:: html

   <p id="p1280722911565">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.55%">

.. raw:: html

   <p id="p5807112965618">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row17807112935611">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.45%">

.. raw:: html

   <p id="p13807132915565">

void

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.55%">

.. raw:: html

   <p id="p15807429185612">

NA

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1980782911567">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.45%">

.. raw:: html

   <p id="p0807529165613">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.55%">

.. raw:: html

   <p id="p9808162935612">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2808192935615">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.45%">

.. raw:: html

   <p id="p380852915567">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.55%">

.. raw:: html

   <p id="p26881319114110">

Returns the pointer to if the operation is successful.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row4808142945615">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.45%">

.. raw:: html

   <p id="p188084291561">

NULL

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.55%">

.. raw:: html

   <p id="p780852912566">

The operation fails.

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

::

   struct DevHandle * handle = NULL;

   /* Obtain the RTC device handle. */
   handle = RtcOpen();
   if (handle  == NULL) {
       /* Process the error. */
   }

Releasing the RTC Device Handle
-------------------------------

You can call the following function to release the RTC device handle,
thereby releasing resources of the device:

void RtcClose(struct DevHandle \*handle);

**Table 2** Description of **RtcClose**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row10752134216114">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.45%">

.. raw:: html

   <p id="p1075217421019">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.55%">

.. raw:: html

   <p id="p117531421411">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row57531442914">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.45%">

.. raw:: html

   <p id="p8753164210119">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.55%">

.. raw:: html

   <p id="p17533425113">

Pointer to the RTC device handle

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

::

   /* Release the RTC device handle. */
   RtcClose(handle);

Registering RtcAlarmCallback
----------------------------

After the OS is started, call the following function to register
**RtcAlarmCallback**, which will be invoked when an alarm is generated
at the specified time:

int32_t RtcRegisterAlarmCallback(struct DevHandle \*handle, enum
RtcAlarmIndex alarmIndex, RtcAlarmCallback cb);

**Table 3** Description of **RtcRegisterAlarmCallback**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1060351914386">

.. raw:: html

   <th class="cellrowborder" valign="top" width="21.36%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p14603181917382">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="78.64%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p36031519183819">

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

   <tr id="row1181618191115">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p131811218131116">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p6181191851111">

Pointer to the RTC device handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row960361918383">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1775535165418">

alarmIndex

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p137551851185412">

Alarm index

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1960431983813">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p3604719123817">

cb

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1560441923818">

Callback that will be invoked when an alarm is generated at the
specified time.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row11410612183019">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p460381915385">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p96031619153812">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row15410111273017">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p133081510112813">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p530813107289">

The operation is successful.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1241081213303">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1123362173010">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1723362153010">

The operation fails.

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

The following is an example of registering **RtcAlarmCallback** for
processing alarm **RTC_ALARM_INDEX_A**:

::

   /* Register an RTC alarm callback. */
   int32_t RtcAlarmACallback(enum RtcAlarmIndex alarmIndex)
   {
       if (alarmIndex == RTC_ALARM_INDEX_A) {
           /* Process alarm A. */
       } else if (alarmIndex == RTC_ALARM_INDEX_B) {
           /* Process alarm B. */
       } else {
       /* Process the error. */
       }
       return 0;
   }
   int32_t ret;
   /* Register RtcAlarmCallback for alarm A. */
   ret = RtcRegisterAlarmCallback(handle, RTC_ALARM_INDEX_A, RtcAlarmACallback);
   if (ret != 0) {
       /* Process the error. */
   }

Performing RTC-related Operations
---------------------------------

-  Reading RTC time

Call the following function to read time information from the RTC
driver, including the year, month, the day fo the week, day, hour,
minute, second, and millisecond:

int32_t RtcReadTime(struct DevHandle \*handle, struct RtcTime \*time);

**Table 4** Description of **RtcReadTime**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row31848013417">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.45%">

.. raw:: html

   <p id="p1415816132411">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.55%">

.. raw:: html

   <p id="p11158111316410">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1246615200297">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.45%">

.. raw:: html

   <p id="p188871821142917">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.55%">

.. raw:: html

   <p id="p1788742182910">

Pointer to the RTC device handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row10184701945">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.45%">

.. raw:: html

   <p id="p104891871157">

time

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.55%">

.. raw:: html

   <p id="p204891671156">

Pointer to the time information read from the RTC driver. The time
information includes the year, month, the day of the week, day, hour,
minute, second, and millisecond.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row17393154515328">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.45%">

.. raw:: html

   <p id="p8158313248">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.55%">

.. raw:: html

   <p id="p161591413741">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row339324593215">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.45%">

.. raw:: html

   <p id="p139599615287">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.55%">

.. raw:: html

   <p id="p1895911611284">

The operation is successful.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row15393184519323">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.45%">

.. raw:: html

   <p id="p13521182309">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.55%">

.. raw:: html

   <p id="p1035216186309">

The operation fails.

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

::

   int32_t ret;
   struct RtcTime tm;

   /* Read time information from the RTC driver. */
   ret = RtcReadTime(handle, &tm);
   if (ret != 0) {
       /* Process the error. */
   }

-  Setting RTC time

Call the following function to set the RTC time:

int32_t RtcWriteTime(struct DevHandle \*handle, struct RtcTime \*time);

**Table 5** Description of **RtcWriteTime**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row924033173613">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.54%">

.. raw:: html

   <p id="p16240143143611">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.46%">

.. raw:: html

   <p id="p32401031113610">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row148011248153018">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.54%">

.. raw:: html

   <p id="p189641849113018">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.46%">

.. raw:: html

   <p id="p20964249123013">

Pointer to the RTC device handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row024043193619">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.54%">

.. raw:: html

   <p id="p157679281384">

time

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.46%">

.. raw:: html

   <p id="p167675286381">

Pointer to the time information written into the RTC driver. The time
information includes the year, month, the day of the week, day, hour,
minute, second, and millisecond.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row424093120369">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.54%">

.. raw:: html

   <p id="p1240143114366">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.46%">

.. raw:: html

   <p id="p18241173133619">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row18241531153610">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.54%">

.. raw:: html

   <p id="p8550174182810">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.46%">

.. raw:: html

   <p id="p145503417284">

The operation is successful.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row024153123616">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.54%">

.. raw:: html

   <p id="p5602191619300">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.46%">

.. raw:: html

   <p id="p12602131643015">

The operation fails.

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

   |image3| **NOTE:** The RTC start time is 1970/01/01 Thursday 00:00:00
   (UTC). The maximum value of **year** must be set based on the
   requirements specified in the product manual of the in-use component.
   You do not need to configure the day of the week.

::

   int32_t ret;
   struct RtcTime tm;

   /* Set the RTC time to UTC 2020/01/01 00:59:00 .000. */
   tm.year = 2020;
   tm.month = 01;
   tm.day = 01;
   tm.hour= 00;
   tm.minute = 59;
   tm.second = 00;
   tm.millisecond = 0;
   /* Write the RTC time information. */
   ret = RtcWriteTime(handle, &tm);
   if (ret != 0) {
       /* Process the error. */
   }

-  Reading the RTC alarm time

Call the following function to read the alarm time:

int32_t RtcReadAlarm(struct DevHandle \*handle, enum RtcAlarmIndex
alarmIndex, struct RtcTime \*time);

**Table 6** Description of **RtcReadAlarm**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row133429310140">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.54%">

.. raw:: html

   <p id="p9886411201416">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.46%">

.. raw:: html

   <p id="p2886411171417">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row13835647114113">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.54%">

.. raw:: html

   <p id="p1183011486412">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.46%">

.. raw:: html

   <p id="p1583074815413">

Pointer to the RTC device handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row113439391410">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.54%">

.. raw:: html

   <p id="p132281120194318">

alarmIndex

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.46%">

.. raw:: html

   <p id="p1022852034315">

Alarm index

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row193431836147">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.54%">

.. raw:: html

   <p id="p1926195164011">

time

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.46%">

.. raw:: html

   <p id="p112695144013">

Pointer to the RTC alarm time information. The time information includes
the year, month, the day of the week, day, hour, minute, second, and
millisecond.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row43438361419">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.54%">

.. raw:: html

   <p id="p388715117143">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.46%">

.. raw:: html

   <p id="p088719117143">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row17169595467">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.54%">

.. raw:: html

   <p id="p107751111283">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.46%">

.. raw:: html

   <p id="p87751917289">

The operation is successful.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row016911915461">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.54%">

.. raw:: html

   <p id="p6833213133013">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.46%">

.. raw:: html

   <p id="p168341213143015">

The operation fails.

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

::

   int32_t ret;
   struct RtcTime alarmTime;

   /* Read the RTC alarm time information of alarm RTC_ALARM_INDEX_A. */
   ret = RtcReadAlarm(handle, RTC_ALARM_INDEX_A, &alarmTime);
   if (ret != 0) {
       /* Process the error. */
   }

-  Setting RTC alarm time

Call the following function to set the RTC alarm time based on the alarm
index:

int32_t RtcWriteAlarm(struct DevHandle \*handle, enum RtcAlarmIndex
alarmIndex, struct RtcTime \*time);

**Table 7** Description of **RtcWriteAlarm**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row14793316131710">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p1891718412183">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p891712461814">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row18419611133117">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p075881210314">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p975811215317">

Pointer to the RTC device handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row11793151613176">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p562522145215">

alarmIndex

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p126257215217">

Alarm index

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row37932016201720">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p26269212527">

time

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p462602125211">

Pointer to the RTC alarm time information. The time information includes
the year, month, the day of the week, day, hour, minute, second, and
millisecond.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row586915225485">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p591712441810">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p1591720461810">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row19869122210483">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p10798105812717">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p1179817586276">

The operation is successful.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1686918225483">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p16246181033012">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p3246111019309">

The operation fails.

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

   |image4| **NOTE:** The RTC start time is 1970/01/01 Thursday 00:00:00
   (UTC). The maximum value of **year** must be set based on the
   requirements specified in the product manual of the in-use component.
   You do not need to configure the day of the week.

::

   int32_t ret;
   struct RtcTime alarmTime;

   /* Set the RTC alarm time to 2020/01/01 00:59:59 .000. */
   alarmTime.year = 2020;
   alarmTime.month = 01;
   alarmTime.day = 01;
   alarmTime.hour = 00;
   alarmTime.minute = 59;
   alarmTime.second = 59;
   alarmTime.millisecond = 0;
   /* Set the alarm time of alarm RTC_ALARM_INDEX_A. */
   ret = RtcWriteAlarm(handle, RTC_ALARM_INDEX_A, &alarmTime);
   if (ret != 0) {
       /* Process the error. */
   }

-  Enabling or disabling alarm interrupts

Before performing alarm operations, use this function to enable alarm
interrupts, so that **RtcAlarmCallback** will be called when the alarm
is not generated upon a timeout.

int32_t RtcAlarmInterruptEnable(struct DevHandle \*handle, enum
RtcAlarmIndex alarmIndex, uint8_t enable);

**Table 8** Description of **RtcAlarmInterruptEnable**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row5346853171519">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p143464533153">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p113461853171514">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2125652144213">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p3150105313422">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p9151653144212">

Pointer to the RTC device handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row153794518293">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p4259165518294">

alarmIndex

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p725985522917">

Alarm index

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row19346653141518">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p6346253101516">

enable

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p234655341511">

Whether to enable RTC alarm interrupts. Value 1 means to enable alarm
interrupts and value 0 means to disable alarm interrupts.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row18346953111513">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p53460537156">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p4346153171510">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1234685314151">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p8947195310279">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p99471953152712">

The operation is successful.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2347115321514">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p324855163018">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p7248857302">

The operation fails.

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

::

   int32_t ret;

   /* Enable the RTC alarm interrupts. */
   ret = RtcAlarmInterruptEnable(handle, RTC_ALARM_INDEX_A, 1);
   if (ret != 0) {
       /* Process the error. */
   }

-  Reading RTC external frequency

Call the following function to read the frequency of the external
crystal oscillator connected to the RTC driver:

int32_t RtcGetFreq(struct DevHandle \*handle, uint32_t \*freq);

**Table 9** Description of **RtcGetFreq**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row1458811241816">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p658820241813">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p758812261820">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row831259124219">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p171541407431">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p715413094314">

Pointer to the RTC device handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1358842171820">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p258814210188">

freq

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p165888211810">

Frequency to set for the external crystal oscillator, in Hz

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2058818281817">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p458872151810">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p155880251819">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row35883213183">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p8133145211272">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p13133352202719">

The operation is successful.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row135892261811">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p152692538292">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p327015313294">

The operation fails.

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

::

   int32_t ret;
   uint32_t freq = 0;

   /* Read frequency of the external crystal oscillator connected to the RTC driver */
   ret = RtcGetFreq(handle, &freq);
   if (ret != 0) {
       /* Process the error. */
   }

-  Setting the frequency of the external crystal oscillator connected to
   the RTC driver

Call the following function to set the frequency of the external crystal
oscillator connected to the RTC driver:

int32_t RtcSetFreq(struct DevHandle \*handle, uint32_t freq);

**Table 10** Description of **RtcSetFreq**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row270119432202">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p127011343132010">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p7701184372013">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row36067554319">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p881511716433">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p188157714432">

Pointer to the RTC device handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row127019437204">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p27019438207">

freq

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p167021043182011">

Frequency to set for the external crystal oscillator, in Hz

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row97022434205">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p1770218431208">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p1170217432201">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1670212432206">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p77021543152017">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p770214310209">

The operation is successful.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row10702194313201">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p165182216306">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p651815219302">

The operation fails.

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

::

   int32_t ret;
   uint32_t freq = 32768; /* 32768 Hz */

   /* Set the frequency of the external crystal oscillator. Note that the frequency must be configured in accordance with the requirements specified in the product manual of the in-use component. */
   ret = RtcSetFreq(handle, freq);
   if (ret != 0) {
       /* Process the error. */
   }

-  Resetting the RTC driver

Call the following function to perform a reset on the RTC driver. After
the reset, the registers are restored to the default values:

int32_t RtcReset(struct DevHandle \*handle);

**Table 11** Description of **RtcReset**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row179899311254">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p199899314257">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p179897315257">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row14989113118257">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p129018136436">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p290111304310">

Pointer to the RTC device handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row7989123111254">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p129894313251">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p799013112256">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row9990193142513">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p1999043111257">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p1799093182516">

The operation is successful.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row16990133152516">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.36%">

.. raw:: html

   <p id="p17536173573015">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.64%">

.. raw:: html

   <p id="p1153623503014">

The operation fails.

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

::

   int32_t ret;

   /* Reset the RTC driver. After the reset, the configuration registers are restored to the default values. */
   ret = RtcReset(handle);
   if (ret != 0) {
       /* Process the error. */
   }

-  Reading the configuration of a custom RTC register

Call the following function to read the configuration of a custom RTC
register based on the register index (one index corresponds to one byte
of the configuration value):

int32_t RtcReadReg(struct DevHandle \*handle, uint8_t usrDefIndex,
uint8_t \*value);

**Table 12** Description of **RtcReadReg**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row92469423320">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p102461548331">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p15246847331">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row171318200434">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p9895321184320">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p68951214436">

Pointer to the RTC device handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row324614143314">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p82466433320">

usrDefIndex

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p181671825470">

Index of the custom register

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row524716420334">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p8247844333">

value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p524711413319">

Register value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row112471143334">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p1124716483312">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p1524716443313">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row9247194183314">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p62476410334">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p152471433317">

The operation is successful.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1424719410333">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p112477417335">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p7247547338">

The operation fails.

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

::

   int32_t ret;
   uint8_t usrDefIndex = 0; /* Define index 0 for the first custom register. */
   uint8_t value = 0;

   /* Read the configuration of a custom RTC register based on the register index. One index corresponds to one byte of the configuration value. */
   ret = RtcReadReg(handle, usrDefIndex, &value);
   if (ret != 0) {
       /* Process the error. */
   }

-  Setting the configuration of a custom RTC register

Call the following function to configure a register based on the
specified register index (one index corresponds to one byte of the
configuration value):

int32_t RtcWriteReg(struct DevHandle \*handle, uint8_t usrDefIndex,
uint8_t value);

**Table 13** Description of **RtcWriteReg**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row187221648133611">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p2722184823617">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p1372374810367">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1675092612435">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p7783927144312">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p197831427134310">

Pointer to the RTC device handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1723174815367">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p1972364814366">

usrDefIndex

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p18723184819365">

Index of the custom register

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2723548163611">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p1772364893610">

value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p1772324803619">

Register value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1072314482361">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p6723194853618">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p1872314893614">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row20723148173617">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p12723348133615">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p472324873620">

The operation is successful.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row127231848123615">

.. raw:: html

   <td class="cellrowborder" valign="top" width="21.62%">

.. raw:: html

   <p id="p197231148173613">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="78.38000000000001%">

.. raw:: html

   <p id="p16723134823618">

The operation fails.

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

::

   int32_t ret;
   uint8_t usrDefIndex = 0; /* Define index 0 for the first custom register. */
   uint8_t value = 0x10;

   /* Configure a register based on the specified register index. One index corresponds to one byte of the configuration value. */
   ret = RtcWriteReg(handle, usrDefIndex, value);
   if (ret != 0) {
       /* Process the error. */
   }

.. |image1| image:: figures/en-us_image_0000001054728498.png
.. |image2| image:: public_sys-resources/icon-note.gif
.. |image3| image:: public_sys-resources/icon-note.gif
.. |image4| image:: public_sys-resources/icon-note.gif
