codec_interface.h
=================

**Overview**\ 
--------------

**Related Modules:**

`Codec <codec.rst>`__

**Description:**

Declares codec-related APIs, including functions for initializing audio
and video codecs, setting parameters, and controlling and transferring
data.

**Since:**

1.0

**Version:**

1.0

**Summary**\ 
-------------

Functions
---------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1481812303084828">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p80335669084828">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1751793269084828">

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

   <tr id="row1092937500084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1511487061084828">

CodecInit ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1649825339084828">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1417185605084828">

Initializes the internal audio and video submodules of the codec.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row144975403084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p649037662084828">

CodecDeinit ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2105676987084828">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p569541319084828">

Deinitializes the internal audio and video submodules of the codec.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1325922120084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1469175653084828">

CodecEnumerateCapbility (uint32_t index, CodecCapbility \*cap)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1402286556084828">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p635027781084828">

Obtains the capabilities of a specified media type based on an index.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1370421659084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p550278157084828">

CodecGetCapbility (AvCodecMime mime, CodecType type, uint32_t flags,
CodecCapbility \*cap)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p766284835084828">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p196418284084828">

Obtains the capabilities of a specified media type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1452887326084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1014366028084828">

CodecCreate (const char *name, const Param*\ attr, int len,
CODEC_HANDLETYPE \*handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1300827907084828">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p794927053084828">

Creates a specific codec component and returns the component context
through a handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1313569955084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p284329595084828">

CodecDestroy (CODEC_HANDLETYPE handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p288521609084828">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1756755568084828">

Destroys a codec component.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1988714031084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p298009415084828">

CodecSetPortMode (CODEC_HANDLETYPE handle, DirectionType type,
BufferMode mode)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p671788526084828">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1680293168084828">

Sets the input or output buffer mode.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2051453233084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1626249989084828">

CodecSetParameter (CODEC_HANDLETYPE handle, const Param \*params, int
paramCnt)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1899152405084828">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1514364229084828">

Sets parameters required by a codec component.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1180071879084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p87782646084828">

CodecGetParameter (CODEC_HANDLETYPE handle, Param \*params, int
paramCnt)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1793508265084828">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p434449871084828">

Obtains parameters from a codec component.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1010047897084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1066596118084828">

CodecStart (CODEC_HANDLETYPE handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p805826522084828">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1967925096084828">

Starts a codec component.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1459719554084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1451408430084828">

CodecStop (CODEC_HANDLETYPE handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1306291644084828">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1423777299084828">

Stops a codec component.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1191045045084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1796631862084828">

CodecFlush (CODEC_HANDLETYPE handle, DirectionType directType)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p475857428084828">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p273063746084828">

Clears the cache when the codec component is the running state.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1432737053084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p221226115084828">

CodecQueueInput (CODEC_HANDLETYPE handle, const InputInfo \*inputData,
uint32_t timeoutMs)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1046593519084828">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1637101078084828">

Queues input data.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row95602801084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p995660483084828">

CodecDequeInput (CODEC_HANDLETYPE handle, uint32_t timeoutMs, InputInfo
\*inputData)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2114703178084828">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p847755638084828">

Dequeues input data that has been used.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1230425643084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2020508747084828">

CodecQueueOutput (CODEC_HANDLETYPE handle, OutputInfo \*outInfo,
uint32_t timeoutMs, int releaseFenceFd)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1985980182084828">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1094765293084828">

Queues output data.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2041813342084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1870505306084828">

CodecDequeueOutput (CODEC_HANDLETYPE handle, uint32_t timeoutMs, int
*acquireFd, OutputInfo*\ outInfo)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p994733508084828">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p968528719084828">

Dequeues output data.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1673579581084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1848732106084828">

CodecSetCallback (CODEC_HANDLETYPE handle, const CodecCallback \*cb,
UINTPTR instance)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1556302023084828">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p357673905084828">

Sets the callback function.

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
