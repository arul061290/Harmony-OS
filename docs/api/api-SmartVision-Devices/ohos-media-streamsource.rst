OHOS::Media::StreamSource
=========================

**Overview**\ 
--------------

**Related Modules:**

`MultiMedia_MediaCommon <multimedia_mediacommon.rst>`__

**Description:**

Provides functions related to the stream source for upper-layer
applications.

After the **SetSource** function is called, the player invokes
`OnBufferAvailable <multimedia_mediacommon.rst#gaaebd4fe9df44b434f410aec32cf23467>`__
to notify your application of the buffer memory block that can be filled
with data. The player can invoke
`SetStreamCallback <multimedia_mediacommon.rst#ga078516891396a86226c945e02c79c1f5>`__
to register a callback for your application. For example, the
**GetBuffer** callback obtains the address of the buffer block and sends
the filled buffer memory block to the player. The buffer memory block is
allocated and processed on the player.
`StreamSource <ohos-media-streamsource.rst>`__\ is available only for the
media source of the **SOURCE_TYPE_STREAM** type. For details, see
`SourceType <format.rst#ga3ae727773c367ac1041d72ac770a0ab1>`__.

**Since:**

1.0

**Version:**

1.0

**Summary**\ 
-------------

Public Member Functions
-----------------------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2073141114093532">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1109619490093532">

Public Member Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1843627956093532">

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

   <tr id="row717410358093532">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1832986306093532">

OnBufferAvailable (size_t index, size_t offset, size_t size)=0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1217160767093532">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p2070504676093532">

Notifies your application of the information about the buffer memory
block that can be filled with data.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row721469379093532">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1043998234093532">

SetStreamCallback (const std::shared_ptr< StreamCallback > &callback)=0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p763226835093532">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p2139923513093532">

Sets a callback function for your application.

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
