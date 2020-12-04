BufferStream
============

**Overview**\ 
--------------

**Related Modules:**

`Format <format.md>`__

**Description:**

Defines the function for reading stream data.

**Since:**

1.0

**Version:**

1.0

**Summary**\ 
-------------

Data Fields
-----------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1323234146093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p441301631093529">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1552533267093529">

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

   <tr id="row1997461826093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1323546637093529">

ReadData )(void *handle, uint8_t*\ data, int32_t size, int32_t
timeOutMs, DataFlags \*flags)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p766582115093529">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p387230513093529">

Reads data from streams, save the data to the buffer pointed by data
with the specified size, and returns the size of the read data and type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1216511084093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1406357602093529">

GetReadableSize )(const void \*handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1158899833093529">

int32_t(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1204108019093529">

Obtains the size of data that can be read.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row328899468093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p200010745093529">

handle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p697775831093529">

void \*

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

**Field Documentation**\ 
-------------------------

GetReadableSize
---------------

::

   int32_t(* BufferStream::GetReadableSize) (const void *[handle](bufferstream.md#ae2019a77aba73fa96d5a716155c7fb7f))

**Description:**

Obtains the size of data that can be read.

Before reading data, you should call this function to check whether
there is data to read.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1227170241093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p612879636093529">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p809849653093529">

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

   <tr id="row302141161093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the context handle.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the size of the read data.

handle
------

::

   void* BufferStream::handle

**Description:**

Context handle

ReadData
--------

::

   int32_t(* BufferStream::ReadData) (void *[handle](bufferstream.md#ae2019a77aba73fa96d5a716155c7fb7f), uint8_t *data, int32_t size, int32_t timeOutMs, [DataFlags](format.md#gacff079fdf8427c743f9197ea5be33a7f) *flags)

**Description:**

Reads data from streams, save the data to the buffer pointed by **data**
with the specified **size**, and returns the size of the read data and
type.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row669909289093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p335502138093529">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1662677005093529">

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

   <tr id="row1477108758093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the context handle.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1593245296093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

data

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the buffer to store the read data. The memory
is allocated by the caller.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1010827668093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

size

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the size of the available buffer memory.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1225687994093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

timeOutMs

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates read operation wait time. The value 0 means no wait time.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row962851156093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

flags

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the type of the read data, see DataFlags.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the size of the read data.
