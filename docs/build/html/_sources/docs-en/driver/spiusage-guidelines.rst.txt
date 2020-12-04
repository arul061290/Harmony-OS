SPI Usage Guidelines
====================

How to Use
----------

`Figure 1 <#fig23885455594>`__ shows the process of using an SPI device.

**Figure 1** Process of using an SPI device

|image1|

Obtaining an SPI Device Handle
------------------------------

Before performing SPI communication, obtain an SPI device handle by
calling **SpiOpen**. This function returns an SPI device handle with a
specified bus number and CS number.

struct DevHandle \*SpiOpen(const struct SpiDevInfo \*info);

**Table 1** Description of **SpiOpen**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row1060351914386">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p14603181917382">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p36031519183819">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1960431983813">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p3604719123817">

info

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p1560441923818">

Pointer to the SPI device descriptor.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row380484160">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p460381915385">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

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

   <tr id="row5793818161">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p1060418195389">

NULL

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p760471912388">

Failed to obtain an SPI device handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row187914871618">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p5604719133811">

Device handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p3604181933818">

Returns the pointer to the SPI device handle.

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

The following example shows how to obtain an SPI device handle based on
the assumption that both the bus number and CS number of the SPI device
are **0**.

::

   struct SpiDevInfo spiDevinfo;       /* SPI device descriptor */
   struct DevHandle *spiHandle = NULL; /* SPI device handle */
   spiDevinfo.busNum = 0;              /* SPI device bus number */
   spiDevinfo.csNum = 0;               /* SPI device CS number */

   /* Obtain an SPI device handle. */
   spiHandle = SpiOpen(&spiDevinfo);
   if (spiHandle == NULL) {
       HDF_LOGE("SpiOpen: failed\n");
       return;
   }

Obtaining SPI Device Configuration Parameters
---------------------------------------------

After obtaining the SPI device handle, obtain the SPI device
configuration parameters by calling the following function:

int32_t SpiGetCfg(struct DevHandle \*handle, struct SpiCfg \*cfg);

**Table 2** Description of **SpiGetCfg**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row1420918529133">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p42091852141314">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p202099523137">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row142091352171310">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p1520915529131">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p720995291310">

Pointer to the SPI device handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row6209152161314">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p720916522139">

cfg

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p172091452131319">

Pointer to SPI device configuration parameters.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row12092522139">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p18209125211134">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p420975231318">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row8209155251310">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p13210145291312">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p152101952141315">

Succeeded in obtaining SPI device configuration parameters.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row102101452121320">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p10210175219134">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p72101252101312">

Failed to obtain SPI device configuration parameters.

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
   struct SpiCfg cfg = {0};                /* SPI configuration information */
   ret = PalSpiSetCfg(spiHandle, &cfg);       /* Set SPI device configuration parameters. */
   if (ret != 0) {
       HDF_LOGE("SpiGetCfg: failed, ret %d\n", ret);
   }

Setting SPI Device Configuration Parameters
-------------------------------------------

After obtaining the SPI device handle, set SPI device configuration
parameters by calling the following function:

int32_t SpiSetCfg(struct DevHandle \*handle, struct SpiCfg \*cfg);

**Table 3** Description of **SpiSetCfg**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row14191192918522">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p17424155016529">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p942512508520">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row219152915524">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p2191122985218">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p1519162913524">

Pointer to the SPI device handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1719110297526">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p181911292523">

cfg

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p91911729155216">

Pointer to SPI device configuration parameters.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row036524131716">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p6425165035214">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p18425650165215">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row43653411178">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p1319132918520">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p1719117292522">

Succeeded in setting SPI device configuration parameters.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row536594171715">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p719119296522">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p20191192925212">

Failed to set SPI device configuration parameters.

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
   struct SpiCfg cfg = {0};                     /* SPI configuration information */
   cfg.mode = SPI_MODE_LOOP;                    /* Communicate in loopback mode. */
   cfg.comMode = PAL_SPI_POLLING_TRANSFER; /* Communicate in polling mode. */
   cfg.maxSpeedHz = 115200;                     /* Maximum transmission frequency */
   cfg.bitsPerWord = 8;                         /* The width of per word to be read or written is 8 bits. */
   ret = SpiSetCfg(spiHandle, &cfg);            /* Set SPI device configuration parameters. */
   if (ret != 0) {
       HDF_LOGE("SpiSetCfg: failed, ret %d\n", ret);
   }

Performing SPI Communication
----------------------------

-  Writing data of a specified length into an SPI device

To write data into an SPI device only once, call the following function:

int32_t SpiWrite(struct DevHandle \*handle, uint8_t \*buf, uint32_t
len);

**Table 4** Description of **SpiWrite**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row31848013417">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p1415816132411">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

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

   <tr id="row10184701945">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p104891871157">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p204891671156">

Pointer to the SPI device handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row928111518418">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p4282955412">

buf

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p7282752412">

Pointer to the data to write.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row149041113651">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p139051213357">

len

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p16905313854">

Length of the data to write.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1148818622017">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p8158313248">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

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

   <tr id="row14488762202">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p103191916578">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p1231981611712">

Succeeded in writing data into an SPI device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row164881464201">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p531916166716">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p93191161174">

Failed to write data into an SPI device.

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
   uint8_t wbuff[4] = {0x12, 0x34, 0x56, 0x78};
   /* Write data of a specified length into an SPI device. */
   ret = SpiWrite(spiHandle, wbuff, 4);
   if (ret != 0) {
       HDF_LOGE("SpiWrite: failed, ret %d\n", ret);
   }

-  Reading data of a specified length from an SPI device

To read data from an SPI device only once, call the following function:

int32_t SpiRead(struct DevHandle \*handle, uint8_t \*buf, uint32_t len);

**Table 5** Description of **SpiRead**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row42651914141213">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p1483184123">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p9831871216">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1926651415123">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p389183129">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p168151817124">

Pointer to the SPI device handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row202661414201220">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p158161821210">

buf

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p98131811126">

Pointer to the data to read.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1926621451212">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p2918182124">

len

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p169718191220">

Length of the data to read.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row05841310206">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p38171818128">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p881918161220">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row15584173192016">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p14871820128">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p88118101211">

Succeeded in reading data from an SPI device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1058418317204">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p10841817125">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p986183127">

Failed to read data from an SPI device.

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
   uint8_t rbuff[4] = {0};
   /* Read data of a specified length from an SPI device. */
   ret = SpiRead(spiHandle, rbuff, 4);
   if (ret != 0) {
       HDF_LOGE("SpiRead: failed, ret %d\n", ret);
   }

-  Launching a custom transfer

To launch a custom transfer, call the following function:

int32_t SpiTransfer(struct DevHandle \*handle, struct SpiMsg \*msgs,
uint32_t count);

**Table 6** Description of **SpiTransfer**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row1134415176216">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p13295152320217">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p1295112352115">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row5344101702113">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p19295132382111">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p829510232213">

Pointer to the SPI device handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row17344171722117">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p9295122332113">

msgs

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p202951238218">

Pointer to the message array to be transferred.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row45812466213">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p1659246112117">

count

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p259124622119">

Length of the message array.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row45187318214">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p17295142322113">

Return Value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p142959232211">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row175186313217">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p929532313211">

0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p829512237217">

Succeeded in launching the custom transfer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1451803152114">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p12958234217">

Negative value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p1295192312112">

Failed to launch the custom transfer.

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
   uint8_t wbuff[1] = {0x12};
   uint8_t rbuff[1] = {0};
   struct SpiMsg msg;        /* Custom message to be transferred */
   msg.wbuf = wbuff;         /* Pointer to the data to read */
   msg.rbuf = rbuff;         /* Pointer to the data to read */
   msg.len = 1;              /* The length of the data to be read or written is 1 bit. */
   msg.csChange = 1;         /* Disable the CS before the next transfer. */
   msg.delayUs = 0;          /* No delay before the next transfer */
   msg.speed = 115200;       /* Speed of this transfer */
   /* Launch a custom transfer. The number of messages to be transferred is 1. */
   ret = SpiTransfer(spiHandle, &msg, 1);
   if (ret != 0) {
       HDF_LOGE("SpiTransfer: failed, ret %d\n", ret);
   }

Destroying the SPI Device Handle
--------------------------------

After the SPI communication, destroy the SPI device handle by calling
the following function:

void SpiClose(struct DevHandle \*handle);

This function will release the resources previously obtained.

**Table 7** Description of **SpiClose**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row1525793312">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p115402031153111">

Parameter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p65406313319">

Description

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1926109193116">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p105419317318">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%">

.. raw:: html

   <p id="p16541153110317">

Pointer to the SPI device handle

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

   PalHandleDestroy(spiHandle); /* Destroy the SPI device handle. */

.. |image1| image:: figures/en-us_image_0000001054726248.png
