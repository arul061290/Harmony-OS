SDIO Usage Guidelines
=====================

How to Use
----------

`Figure 1 <spiusage-guidelines.rst#fig23885455594>`__ illustrates the
process of using an SDIO.

**Figure 1** Process of using an SDIO

|image1|

Opening an SDIO Controller
--------------------------

Before performing SDIO communication, obtain the device handle of an
SDIO controller by calling **SdioOpen**. This function returns the
device handle of the SDIO controller with a specified bus number.

struct DevHandle \*SdioOpen(int16_t busNum);

**Table 1** Parameters and return values of SdioOpen

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1011212598452">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p141124595457">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p1111214593455">

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

   <tr id="row19112195918454">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p11121759124515">

busNum

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p111121459194519">

SDIO bus number.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row6112659184518">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1112105919453">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p6112659114518">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row3113559164519">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p51121159104517">

NULL

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1811313597458">

Failed to obtain the device handle of an SDIO controller.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row201131059194512">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1311375919456">

Device handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1911312599450">

Device handle of an SDIO controller.

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

The following example shows how to open an SDIO controller.

::

   struct DevHandle *handle = NULL;
   int16_t busNum = 1;
   /* Open an SDIO controller whose bus number is 1. */
   handle = SdioOpen(busNum);
   if (handle == NULL) {
       HDF_LOGE("SdioOpen: failed!\n");
   }

Claiming a Host Exclusively
---------------------------

After obtaining the device handle of an SDIO controller, exclusively
claim the host before performing subsequent operations on the SDIO
device.

void SdioClaimHost(struct DevHandle \*handle);

**Table 2** Parameter description of SdioClaimHost

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1211325914459">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p611365954517">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p1711365954510">

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

   <tr id="row3114205920451">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p181141592457">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p41144595458">

Device handle of an SDIO controller

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

The following example shows how to exclusively claim a host.

::

   SdioClaimHost(handle); /* Claim a host exclusively. */

Enabling the SDIO Device
------------------------

Before accessing a register, enable the SDIO device.

int32_t SdioEnableFunc(struct DevHandle \*handle);

**Table 3** Parameters and return values of SdioEnableFunc

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row8487204184815">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p1648611415486">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p19487134124820">

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

   <tr id="row16487044480">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p74878414810">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p17487184194819">

Device handle of an SDIO controller.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row13487748487">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p24873424811">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p4487174134813">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1748814494812">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p84878410488">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p948715410483">

The SDIO device is enabled.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row54881416482">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p24881645489">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p10488247487">

Failed to enable the SDIO device.

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

The following example shows how to enable the SDIO device.

::

   int32_t ret;
   /* Enable the SDIO device. */
   ret = SdioEnableFunc(handle);
   if (ret != 0) {
       HDF_LOGE("SdioEnableFunc: failed, ret %d\n", ret);
   }

Claiming an SDIO IRQ
--------------------

Before SDIO communication, claim an SDIO IRQ.

int32_t SdioClaimIrq(struct DevHandle \*handle, SdioIrqHandler
\*handler);

**Table 4** Parameters and return values of SdioClaimIrq

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row114891042488">

.. raw:: html

   <th class="cellrowborder" valign="top" width="49.980000000000004%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p1348864164811">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50.019999999999996%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p14885410486">

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

   <tr id="row048911404820">

.. raw:: html

   <td class="cellrowborder" valign="top" width="49.980000000000004%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p248974174814">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.019999999999996%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1848915494813">

Device handle of an SDIO controller.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row204894454813">

.. raw:: html

   <td class="cellrowborder" valign="top" width="49.980000000000004%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p17489944488">

handler

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.019999999999996%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1548984174813">

Pointer to the SDIO IRQ function.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row44898413488">

.. raw:: html

   <td class="cellrowborder" valign="top" width="49.980000000000004%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1548934124815">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.019999999999996%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p54891444485">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row748994144811">

.. raw:: html

   <td class="cellrowborder" valign="top" width="49.980000000000004%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p448918415484">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.019999999999996%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p174892412489">

The SDIO IRQ is claimed.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row448914420489">

.. raw:: html

   <td class="cellrowborder" valign="top" width="49.980000000000004%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p248912464817">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.019999999999996%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p34891645485">

Failed to claim an SDIO IRQ.

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

The following example shows how to claim an SDIO IRQ.

::

   /* Implement the SDIO IRQ function based on the application. */
   static void SdioIrqFunc(void *data)
   {
       if (data == NULL) {
           HDF_LOGE("SdioIrqFunc: data is NULL.\n");
           return;
       }
       /* You need to add specific implementations. */
   }

   int32_t ret;
   /* Claim an SDIO IRQ. */
   ret = SdioClaimIrq(handle, SdioIrqFunc);
   if (ret != 0) {
       HDF_LOGE("SdioClaimIrq: failed, ret %d\n", ret);
   }

Performing SDIO Communication
-----------------------------

-  Incrementally write a given length of data into the SDIO device.

The corresponding function is as follows:

int32_t SdioWriteBytes(struct DevHandle \*handle, uint8_t \*data,
uint32_t addr, uint32_t size, uint32_t timeOut);

**Table 5** Parameters and return values of SdioWriteBytes

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row10887144111419">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p181381751164113">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p19138115184116">

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

   <tr id="row4887341174114">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1534612017427">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p8179347434">

Device handle of an SDIO controller.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row18881041144120">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p10888154118412">

data

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1288854115413">

Pointer to the data to write.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row191054911432">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p91054994311">

addr

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p111024915432">

Start address where the data is written into.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row14888144124119">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1588814413412">

size

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1288813411413">

Length of the data to write.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row188213710445">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p08227154415">

timeOut

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p6821875446">

Timeout duration for writing data, in milliseconds. If the value is 0,
the default value is used.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row18247654163519">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p486155173610">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1686155113620">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row10574165663512">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p912141012364">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p51219107363">

Data is written into the SDIO device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1490635883519">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p10121510133617">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p131212106365">

Failed to write data into the SDIO device.

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

The following example shows how to incrementally write a given length of
data into the SDIO device.

::

   int32_t ret;
   uint8_t wbuff[] = {1,2,3,4,5};
   uint32_t addr = 0x100 + 0x09;
   /* Incrementally write 5-byte data into the start address 0x109 of the SDIO device. */
   ret = SdioWriteBytes(handle, wbuff, addr, sizeof(wbuff) / sizeof(wbuff[0]), 0);
   if (ret != 0) {
       HDF_LOGE("SdioWriteBytes: failed, ret %d\n", ret);
   }

-  Incrementally read a given length of data from the SDIO device.

The corresponding function is as follows:

int32_t SdioReadBytes(struct DevHandle \*handle, uint8_t \*data,
uint32_t addr, uint32_t size, uint32_t timeOut);

**Table 6** Parameters and return values of SdioReadBytes

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row19783355162116">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p635754142212">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p1035774182215">

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

   <tr id="row137831055192118">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p14783155192114">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p9676437202218">

Device handle of an SDIO controller.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row4784155102111">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1978455510217">

data

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p767683714223">

Pointer to the data to read.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row63651118499">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p73669113496">

addr

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p53661144916">

Start address where the data is read from.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row7784145510218">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1078413554219">

size

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p14676163782210">

Length of the data to read.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1823311517494">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p723314152499">

timeOut

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1323351515493">

Timeout duration for reading data, in milliseconds. If the value is 0,
the default value is used.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row964182643610">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p7833639163612">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p3833939113619">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row199479312363">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p567424413611">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p166741544113615">

Data is read from the SDIO device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row5166203418361">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1167416448361">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p9674114410364">

Failed to read data from the SDIO device.

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

The following example shows how to incrementally read a given length of
data from the SDIO device.

::

   int32_t ret;
   uint8_t rbuff[5] = {0};
   uint32_t addr = 0x100 + 0x09;
   /* Incrementally read 5-byte data from the start address 0x109 of the SDIO device. */
   ret = SdioReadBytes(handle, rbuff, addr, 5, 0);
   if (ret != 0) {
       HDF_LOGE("SdioReadBytes: failed, ret %d\n", ret);
   }

-  Write a given length of data into the fixed address of an SDIO
   device.

   The corresponding function is as follows:

   int32_t SdioWriteBytesToFixedAddr(struct DevHandle \*handle, uint8_t
   \*data, uint32_t addr, uint32_t size, uint32_t timeOut)

   **Table 7** Parameters and return values of SdioWriteBytesToFixedAddr

   .. raw:: html

      <table>

   .. raw:: html

      <thead align="left">

   .. raw:: html

      <tr id="row1582911114010">

   .. raw:: html

      <th class="cellrowborder" valign="top" width="48.43%" id="mcps1.2.3.1.1">

   .. raw:: html

      <p id="p28301411903">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </th>

   .. raw:: html

      <th class="cellrowborder" valign="top" width="51.57000000000001%" id="mcps1.2.3.1.2">

   .. raw:: html

      <p id="p1883019111018">

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

      <tr id="row10830141111014">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.43%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p470818551018">

   handle

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.57000000000001%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p18578510518">

   Device handle of an SDIO controller.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row48303111304">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.43%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p127081955502">

   data

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.57000000000001%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p1857841013110">

   Pointer to the data to write.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row9830111119019">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.43%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p187085555011">

   addr

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.57000000000001%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p257831016115">

   Fixed address where the data is written into.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row683091120012">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.43%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p370819555013">

   size

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.57000000000001%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p7578181015113">

   Length of the data to write.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row58301911309">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.43%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p570810551107">

   timeOut

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.57000000000001%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p17579910915">

   Timeout duration for writing data, in milliseconds. If the value is
   0, the default value is used.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row18215162810212">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.43%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p1521319452211">

   Return Value

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.57000000000001%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p162138457217">

   Description

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row2197123118210">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.43%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p1921413451212">

   0

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.57000000000001%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p32146451624">

   Data is written into the SDIO device.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row18629103314218">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.43%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p132141245622">

   Negative value

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.57000000000001%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p17214345328">

   Failed to write data into the SDIO device.

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

   The following example shows how to write a given length of data into
   the fixed address of an SDIO device.

   ::

      int32_t ret;
      uint8_t wbuff[] = {1, 2, 3, 4, 5};
      uint32_t addr = 0x100 + 0x09;
      /* Write 5-byte data into the fixed address 0x109 of the SDIO device. */
      ret = SdioWriteBytesToFixedAddr(handle, wbuff, addr, sizeof(wbuff) / sizeof(wbuff[0]), 0);
      if (ret != 0) {
          HDF_LOGE("SdioWriteBytesToFixedAddr: failed, ret %d\n", ret);
      }

-  Read a given length of data from the fixed address of an SDIO device.

   The corresponding function is as follows:

   int32_t SdioReadBytesFromFixedAddr(struct DevHandle \*handle, uint8_t
   \*data, uint32_t addr, uint32_t size, uint32_t timeOut)

   **Table 8** Parameters and return values of
   SdioReadBytesFromFixedAddr

   .. raw:: html

      <table>

   .. raw:: html

      <thead align="left">

   .. raw:: html

      <tr id="row8724142214115">

   .. raw:: html

      <th class="cellrowborder" valign="top" width="48.699999999999996%" id="mcps1.2.3.1.1">

   .. raw:: html

      <p id="p16752055131112">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </th>

   .. raw:: html

      <th class="cellrowborder" valign="top" width="51.300000000000004%" id="mcps1.2.3.1.2">

   .. raw:: html

      <p id="p914434191218">

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

      <tr id="row1372462214119">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.699999999999996%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2752175516113">

   handle

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.300000000000004%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p1353155020125">

   Device handle of an SDIO controller.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row197244220117">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.699999999999996%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p12752165581117">

   data

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.300000000000004%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p9540508121">

   Pointer to the data to read.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row172519228116">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.699999999999996%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p1675315521120">

   addr

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.300000000000004%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p05415501125">

   Start address where the data is read from.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row137251922131117">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.699999999999996%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p47531355111111">

   size

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.300000000000004%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p1954165031214">

   Length of the data to read.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row972552281111">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.699999999999996%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p2753755161114">

   timeOut

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.300000000000004%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p3541350111218">

   Timeout duration for reading data, in milliseconds. If the value is
   0, the default value is used.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row15725162210117">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.699999999999996%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p681073451314">

   Return Value

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.300000000000004%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p17810134121316">

   Description

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row1772511227119">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.699999999999996%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p78105346133">

   0

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.300000000000004%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p18810173411312">

   Data is read from the SDIO device.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row191829161138">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.699999999999996%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p1581012340131">

   Negative value

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.300000000000004%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p28101834161317">

   Failed to read data from the SDIO device.

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

   The following example shows how to read a given length of data from
   the fixed address of an SDIO device.

   ::

      int32_t ret;
      uint8_t rbuff[5] = {0};
      uint32_t addr = 0x100 + 0x09;
      /* Read 5-byte data from the fixed address 0x109 of the SDIO device. */
      ret = SdioReadBytesFromFixedAddr(handle, rbuff, addr, 5, 0);
      if (ret != 0) {
          HDF_LOGE("SdioReadBytesFromFixedAddr: failed, ret %d\n", ret);
      }

-  Write a given length of data into the address space of SDIO function
   0.

Currently, only 1-byte data can be written. The corresponding function
is as follows:

int32_t SdioWriteBytesToFunc0(struct DevHandle \*handle, uint8_t \*data,
uint32_t addr, uint32_t size, uint32_t timeOut);

**Table 9** Parameters and return values of SdioWriteBytesToFunc0

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2033991881120">

.. raw:: html

   <th class="cellrowborder" valign="top" width="49.94%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p1116916499117">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50.06%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p13169174971115">

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

   <tr id="row9339171871118">

.. raw:: html

   <td class="cellrowborder" valign="top" width="49.94%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p16169194914117">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.06%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p10169114921110">

Device handle of an SDIO controller.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row93401118171116">

.. raw:: html

   <td class="cellrowborder" valign="top" width="49.94%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p216919491118">

data

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.06%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p5169449121117">

Pointer to the data to write.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row534019182114">

.. raw:: html

   <td class="cellrowborder" valign="top" width="49.94%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p2016934941114">

addr

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.06%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p8169649101112">

Start address where the data is written into.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row334011871113">

.. raw:: html

   <td class="cellrowborder" valign="top" width="49.94%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p6169194913117">

size

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.06%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p71691449141119">

Length of the data to write.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1634015181114">

.. raw:: html

   <td class="cellrowborder" valign="top" width="49.94%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p9169049161114">

timeOut

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.06%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p51701849121115">

Timeout duration for writing data, in milliseconds. If the value is 0,
the default value is used.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row123407185111">

.. raw:: html

   <td class="cellrowborder" valign="top" width="49.94%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p294173071617">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.06%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p39421830111616">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row8950101811164">

.. raw:: html

   <td class="cellrowborder" valign="top" width="49.94%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p9942730181613">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.06%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p89421130141617">

Data is written into the SDIO device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row42485216168">

.. raw:: html

   <td class="cellrowborder" valign="top" width="49.94%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1194223012167">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.06%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p19942630121617">

Failed to write data into the SDIO device.

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

The following example shows how to write a given length of data into the
address space of SDIO function 0.

::

   int32_t ret;
   uint8_t wbuff = 1;
   /* Write 1-byte data into the address 0x2 of SDIO function 0. */
   ret = SdioWriteBytesToFunc0(handle, &wbuff, 0x2, 1, 0);
   if (ret != 0) {
       HDF_LOGE("SdioWriteBytesToFunc0: failed, ret %d\n", ret);
   }

-  Read a given length of data from the address space of SDIO function
   0.

Currently, only 1-byte data can be read. The corresponding function is
as follows:

int32_t SdioReadBytesFromFunc0(struct DevHandle \*handle, uint8_t
\*data, uint32_t addr, uint32_t size, uint32_t timeOut);

**Table 10** Parameters and return values of SdioReadBytesFromFunc0

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row771918171819">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p71291418171813">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p51291818101818">

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

   <tr id="row9720113186">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p121294185189">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p20129141815184">

Device handle of an SDIO controller.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row672017114185">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p171291186185">

data

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p8129118171820">

Pointer to the data to read.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row5720910188">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p8129121816184">

addr

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p21296189182">

Start address where the data is read from.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row172020115189">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p18129418191816">

size

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p612921851820">

Length of the data to read.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row147201613181">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p3130161831815">

timeOut

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1513031831816">

Timeout duration for reading data, in milliseconds. If the value is 0,
the default value is used.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row167202113189">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1813001881810">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1313081817184">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row17720151101818">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p131307185182">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p113019187182">

Data is read from the SDIO device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1972019118189">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p18130151815185">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1013001861815">

Failed to read data from the SDIO device.

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

The following example shows how to read a given length of data from the
address space of SDIO function 0.

::

   int32_t ret;
   uint8_t rbuff;
   /* Read 1-byte data from the address 0x2 of SDIO function 0. */
   ret = SdioReadBytesFromFunc0(handle, &rbuff, 0x2, 1, 0);
   if (ret != 0) {
       HDF_LOGE("SdioReadBytesFromFunc0: failed, ret %d\n", ret);
   }

Releasing the SDIO IRQ
----------------------

After the SDIO communication, release the SDIO IRQ.

int32_t SdioReleaseIrq(struct DevHandle \*handle);

**Table 11** Parameters and return values of SdioReleaseIrq

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row15499849482">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p1549964114814">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p749915484816">

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

   <tr id="row1499194104813">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p9499743481">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p184999434815">

Device handle of an SDIO controller.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row3499442485">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p649918414812">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p164991242486">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1349919494810">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p24994484820">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1649920414482">

The SDIO IRQ is released.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row17500204154810">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p194990415489">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p74997419484">

Failed to release the SDIO IRQ.

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

The following example shows how to release the SDIO IRQ.

::

   int32_t ret;
   /* Release the SDIO IRQ. */
   ret = SdioReleaseIrq(handle);
   if (ret != 0) {
       HDF_LOGE("SdioReleaseIrq: failed, ret %d\n", ret);
   }

Disabling the SDIO Device
-------------------------

After the SDIO communication, disable the SDIO device.

int32_t SdioDisableFunc(struct DevHandle \*handle);

**Table 12** Parameters and return values of SdioDisableFunc

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1050010474810">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p05002419488">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p17500114174811">

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

   <tr id="row65001946482">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1150054104814">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1850014184812">

Device handle of an SDIO controller.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row175013494817">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p350013434816">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1750184104813">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1850113413481">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p11501164114818">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1550116416489">

The SDIO device is disabled.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row45015444817">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p7501184154816">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p35011040484">

Failed to disable the SDIO device.

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

The following example shows how to disable the SDIO device.

::

   int32_t ret;
   /* Disable the SDIO device. */
   ret = SdioDisableFunc(handle);
   if (ret != 0) {
       HDF_LOGE("SdioDisableFunc: failed, ret %d\n", ret);
   }

Releasing the Exclusively Claimed Host
--------------------------------------

After the SDIO communication, release the exclusively claimed host.

void SdioReleaseHost(struct DevHandle \*handle);

**Table 13** Parameter description of SdioReleaseHost

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row6502134194814">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p18501945486">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p45028414817">

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

   <tr id="row135027411483">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p16502174204816">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p6502164184816">

Device handle of an SDIO controller

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

The following example shows how to release the exclusively claimed host.

::

   SdioReleaseHost(handle); /* Release the exclusively claimed host. */

Closing an SDIO Controller
--------------------------

After the SDIO communication, close the SDIO controller.

void SdioClose(struct DevHandle \*handle);

This function releases the resources requested.

**Table 14** Parameter description of SdioClose

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1050213424819">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p18502134194818">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p2502154104813">

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

   <tr id="row25035434810">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p175028434819">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p2050274194819">

Device handle of an SDIO controller

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

The following example shows how to close an SDIO controller.

::

   SdioClose(handle); /* Close an SDIO controller. */

.. |image1| image:: figures/en-us_image_0000001054440624.png
