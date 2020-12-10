Watchdog Usage Guidelines
=========================

How to Use
----------

`Figure 1 <#fig19134125410189>`__ illustrates the process of using a
watchdog.

**Figure 1** Process of using a watchdog

|image1|

Opening a Watchdog
------------------

Use **WatchdogOpen** to open a watchdog. A system may have multiple
watchdogs. You can open a specified watchdog by using the ID.

int32_t WatchdogOpen(int16_t wdtId);

**Table 1** Description of WatchdogOpen

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row131371325142819">

.. raw:: html

   <th class="cellrowborder" valign="top" width="44.99%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p191372254283">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="55.010000000000005%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p113819255284">

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

   <tr id="row813812259282">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p101381625162813">

wdtId

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p191381425142813">

Watchdog ID.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2138202515281">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p141387252287">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p12138192512281">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row9138182519287">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p5138102532814">

NULL

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p3138192512815">

Failed to open the watchdog.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row15138192518283">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1850115512916">

struct DevHandle pointer

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p16138122512817">

Pointer to the watchdog handle.

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

   struct DevHandle *handle = NULL;
   handle = WatchdogOpen(0); /* Open watchdog 0.*/
   if (handle == NULL) {
       HDF_LOGE("WatchdogOpen: failed, ret %d\n", ret);
       return;
   }

Obtaining the Watchdog Status
-----------------------------

int32_t WatchdogGetStatus(struct DevHandle \*handle, int32_t \*status);

**Table 2** Description of WatchdogGetStatus

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row31848013417">

.. raw:: html

   <th class="cellrowborder" valign="top" width="44.99%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p1415816132411">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="55.010000000000005%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p11158111316410">

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

   <tr id="row3264122711222">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p15264727182211">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p2026452772210">

Watchdog handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row928111518418">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p4282955412">

status

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p7282752412">

Pointer to the watchdog status.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row17393154515328">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p8158313248">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

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

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p103191916578">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1231981611712">

The watchdog status is obtained.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row15393184519323">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p531916166716">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p93191161174">

Failed to obtain the watchdog status.

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
   int32_t status;
   /* Obtain the watchdog status. */
   ret = WatchdogGetStatus(handle, &status);
   if (ret != 0) {
       HDF_LOGE("WatchdogGetStatus: failed, ret %d\n", ret);
       return;
   }

Setting the Timeout Duration
----------------------------

int32_t WatchdogSetTimeout(PalHandle \*handle, uint32_t seconds);

**Table 3** Description of WatchdogSetTimeout

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1216012212212">

.. raw:: html

   <th class="cellrowborder" valign="top" width="44.99%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p1416017262215">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="55.010000000000005%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p16160182192213">

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

   <tr id="row199536232314">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p17685481236">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p196852811232">

Watchdog handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row141601729228">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p191601126226">

seconds

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p5160172182214">

Timeout duration, in seconds.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row18160192172212">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p101601123222">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p17160192182212">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row171600202220">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p121601226224">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p151607218222">

The setting is successful.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row916012252211">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p19160026224">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p816092142210">

Setting failed.

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
   uint32_t timeOut = 60;
   /* Set the timeout duration, in seconds. */
   ret = WatchdogSetTimeout(handle, timeOut);
   if (ret != 0) {
       HDF_LOGE("WatchdogSetTimeout: failed, ret %d\n", ret);
       return;
   }

Obtaining the Timeout Duration
------------------------------

int32_t WatchdogGetTimeout(PalHandle \*handle, uint32_t \*seconds);

**Table 4** Description of WatchdogGetTimeout

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row14147848142313">

.. raw:: html

   <th class="cellrowborder" valign="top" width="44.99%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p4147124892316">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="55.010000000000005%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p12147144817232">

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

   <tr id="row8147124819230">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p21471248142313">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p12147134815233">

Watchdog handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row514754818232">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1614713484235">

seconds

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p71478484238">

Pointer to the timeout duration, in seconds.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row214784814239">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p5147848152314">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p914724811236">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row714744892312">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1014764832315">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1314824872310">

The timeout duration is obtained.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1514884815230">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p10148114822319">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1314864822311">

Failed to obtain the watchdog status.

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
   uint32_t timeOut;
   /* Obtain the timeout duration, in seconds. */
   ret = WatchdogGetTimeout(handle, &timeOut);
   if (ret != 0) {
       HDF_LOGE("WatchdogGetTimeout: failed, ret %d\n", ret);
       return;
   }

Starting a Watchdog
-------------------

int32_t WatchdogStart(struct DevHandle \*handle);

**Table 5** Description of WatchdogStart

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row92915122513">

.. raw:: html

   <th class="cellrowborder" valign="top" width="44.99%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p5292582517">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="55.010000000000005%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p929554258">

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

   <tr id="row629852250">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p22975122515">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p7290515256">

Watchdog handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row183035162514">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p8302511255">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p16307522515">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row12305552510">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1730175132513">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p630754259">

The watchdog is started.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row4306516252">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p15304502515">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p0301559254">

Failed to start the watchdog.

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
   /* Start the watchdog. */
   ret = WatchdogStart(handle);
   if (ret != 0) {
       HDF_LOGE("WatchdogStart: failed, ret %d\n", ret);
       return;
   }

Feeding a Watchdog
------------------

int32_t WatchdogFeed(struct DevHandle \*handle);

**Table 6** Description of WatchdogFeed

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row891133515393">

.. raw:: html

   <th class="cellrowborder" valign="top" width="44.99%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p1911143513918">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="55.010000000000005%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p1191173553917">

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

   <tr id="row189111635143918">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p189111435173917">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p11911143511397">

Watchdog handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row15911835173916">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p7911123516396">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p169118356399">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row189119352393">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1391113513917">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p149111435143911">

The watchdog is fed.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row5911123520392">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p49111335143920">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1891216356391">

Failed to feed the watchdog.

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
   /* Feed the watchdog. */
   ret = WatchdogFeed(handle);
   if (ret != 0) {
       HDF_LOGE("WatchdogFeed: failed, ret %d\n", ret);
       return;
   }

Stopping a Watchdog
-------------------

int32_t WatchdogStop(struct DevHandle \*handle);

**Table 7** Description of WatchdogStop

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row28687517259">

.. raw:: html

   <th class="cellrowborder" valign="top" width="44.99%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p6868185120254">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="55.010000000000005%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p15868185114252">

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

   <tr id="row1868165114256">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p6869105115256">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p19869951202513">

Watchdog handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row68696510259">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p2869165114256">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p158691551142517">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row9869851192516">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p686916516252">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p7869115192510">

The watchdog is stopped.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row15869951122519">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p486925112518">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p086945172518">

Stopping the watchdog failed.

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
   /* Stop the watchdog. */
   ret = WatchdogStop(handle);
   if (ret != 0) {
       HDF_LOGE("WatchdogStop: failed, ret %d\n", ret);
       return;
   }

Closing a Watchdog
------------------

If the watchdog is no longer required, call **WatchdogClose** to close
the watchdog handle.

void WatchdogClose(struct DevHandle \*handle);

**Table 8** Description of WatchdogClose

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row417314182327">

.. raw:: html

   <th class="cellrowborder" valign="top" width="44.99%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p117310184320">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="55.010000000000005%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p7173191812324">

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

   <tr id="row1617331823211">

.. raw:: html

   <td class="cellrowborder" valign="top" width="44.99%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p17173191811326">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="55.010000000000005%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p538814308323">

Watchdog handle.

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

   /* Close the watchdog. */
   ret = WatchdogClose(handle);

.. |image1| image:: figures/en-us_image_0000001054058088.png
