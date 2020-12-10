OHOS::Media::StreamCallback
===========================

**Overview**\ 
--------------

**Related Modules:**

`MultiMedia_MediaCommon <multimedia_mediacommon.rst>`__

**Description:**

Provides functions to obtain the address of a buffer memory and write
the filled buffers into the playback queue. You need to implement the
`StreamCallback <ohos-media-streamcallback.rst>`__ functions in a player
object.

**Since:**

1.0

**Version:**

1.0

**Summary**\ 
-------------

Public Types
------------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1204165414093532">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1298451830093532">

Public Type Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p227328659093532">

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

   <tr id="row1357337895093532">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p408322624093532">

BufferFlags : uint32_t { STREAM_FLAG_SYNCFRAME = 1,
STREAM_FLAG_CODECCONFIG = 2, STREAM_FLAG_EOS = 4,
STREAM_FLAG_PARTIAL_FRAME = 8, STREAM_FLAG_ENDOFFRAME = 16,
STREAM_FLAG_MUXER_DATA = 32 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1826002100093532">

Enumerates buffer types of stream sources.

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

Public Member Functions
-----------------------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1960562158093532">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p280666664093532">

Public Member Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p692400253093532">

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

   <tr id="row906499042093532">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p28755524093532">

GetBuffer (size_t index)=0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1402970513093532">

virtual uint8_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1094987232093532">

Obtains the virtual address of a buffer memory block based on its index.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row210011413093532">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p409138702093532">

QueueBuffer (size_t index, size_t offset, size_t size, int64_t
timestampUs, uint32_t flags)=0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p181696310093532">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p575845046093532">

Writes the filled buffer memory block into the player memory.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row504220373093532">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1120357178093532">

SetParameters (const Format &params)=0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2000203206093532">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1627319576093532">

Sets additional information about a stream.

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
