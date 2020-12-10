hdf_sbuf.h
==========

**Overview**\ 
--------------

**Related Modules:**

`Core <core.rst>`__

**Description:**

Defines functions related to a `HdfSBuf <hdfsbuf.rst>`__. The HDF
provides data serialization and deserialization capabilities for data
transmission between user-mode applications and kernel-mode drivers.

**Since:**

1.0

**Summary**\ 
-------------

Data Structures
---------------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1963680918093525">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p610745227093525">

Data Structure Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p350282944093525">

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

   <tr id="row679723314093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p56478790093525">

HdfSBuf

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1847271566093525">

Defines a HdfSBuf.

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

Functions
---------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row333962916093525">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2117354541093525">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1553731279093525">

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

   <tr id="row1380744630093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1191449868093525">

HdfSbufWriteBuffer (struct HdfSBuf *sbuf, const void*\ data, uint32_t
writeSize)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1889887859093525">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p507427361093525">

Writes a data segment to a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2033869018093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1349248705093525">

HdfSbufWriteUint64 (struct HdfSBuf \*sbuf, uint64_t value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p315042489093525">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p922055300093525">

Writes a 64-bit unsigned integer to a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row83099383093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p579815334093525">

HdfSbufWriteUint32 (struct HdfSBuf \*sbuf, uint32_t value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p13157914093525">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p625153944093525">

Writes a 32-bit unsigned integer to a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1031412069093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2000239414093525">

HdfSbufWriteUint16 (struct HdfSBuf \*sbuf, uint16_t value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1726966118093525">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p1074316879093525">

Writes a 16-bit unsigned integer to a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1868163630093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p847352381093525">

HdfSbufWriteUint8 (struct HdfSBuf \*sbuf, uint8_t value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p525672919093525">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p1364577541093525">

Writes an 8-bit unsigned integer to a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1828785687093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p223630812093525">

HdfSbufWriteInt64 (struct HdfSBuf \*sbuf, int64_t value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p736286603093525">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p373944113093525">

Writes a 64-bit signed integer to a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row674965776093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1978592643093525">

HdfSbufWriteInt32 (struct HdfSBuf \*sbuf, int32_t value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1816887351093525">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p1458849697093525">

Writes a 32-bit signed integer to a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1643912734093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1485439266093525">

HdfSbufWriteInt16 (struct HdfSBuf \*sbuf, int16_t value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p267807249093525">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p1959204909093525">

Writes a 16-bit signed integer to a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row535888297093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1997390184093525">

HdfSbufWriteInt8 (struct HdfSBuf \*sbuf, int8_t value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p176878630093525">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p1501857946093525">

Writes an 8-bit signed integer to a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1735133988093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p923758698093525">

HdfSbufWriteString (struct HdfSBuf *sbuf, const char*\ value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1597223282093525">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p160868697093525">

Writes a string to a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1189060265093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p325129206093525">

HdfSbufReadBuffer (struct HdfSBuf \*sbuf, const void \**data, uint32_t
\*readSize)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1327156958093525">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p761020251093525">

Reads a data segment from a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1718886941093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p946551273093525">

HdfSbufReadUint64 (struct HdfSBuf *sbuf, uint64_t*\ value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p668021138093525">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p955569390093525">

Reads a 64-bit unsigned integer from a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row774712945093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p197249974093525">

HdfSbufReadUint32 (struct HdfSBuf *sbuf, uint32_t*\ value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p811280258093525">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p1394903444093525">

Reads a 32-bit unsigned integer from a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1799962682093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p825993231093525">

HdfSbufReadUint16 (struct HdfSBuf *sbuf, uint16_t*\ value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p751353808093525">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p1852922860093525">

Reads a 16-bit unsigned integer from a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1852879170093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p165976566093525">

HdfSbufReadUint8 (struct HdfSBuf *sbuf, uint8_t*\ value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p486814607093525">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p419373455093525">

Reads an 8-bit unsigned integer from a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1636216150093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p42228230093525">

HdfSbufReadInt64 (struct HdfSBuf *sbuf, int64_t*\ value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p393585707093525">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p687014808093525">

Reads a 64-bit signed integer from a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row557183447093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p767847244093525">

HdfSbufReadInt32 (struct HdfSBuf *sbuf, int32_t*\ value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p631598318093525">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p1868574382093525">

Reads a 32-bit signed integer from a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row369630343093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p173539921093525">

HdfSbufReadInt16 (struct HdfSBuf *sbuf, int16_t*\ value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1472291015093525">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p368110273093525">

Reads a 16-bit signed integer from a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row550423098093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2116417723093525">

HdfSbufReadInt8 (struct HdfSBuf *sbuf, int8_t*\ value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p272734524093525">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p676542377093525">

Reads an 8-bit signed integer from a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1052882434093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1216535194093525">

HdfSbufReadString (struct HdfSBuf \*sbuf)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p71390371093525">

const char \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p737647854093525">

Reads a string from a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row748448988093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1097740748093525">

HdfSbufGetData (const struct HdfSBuf \*sbuf)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p9271406093525">

uint8_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1858930585093525">

Obtains the pointer to the data stored in aSBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1178357999093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p224816180093525">

HdfSbufFlush (struct HdfSBuf \*sbuf)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p972444178093525">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1939942266093525">

Clears the data stored in a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1647168979093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p298035364093525">

HdfSbufGetCapacity (const struct HdfSBuf \*sbuf)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p763823723093525">

size_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1348809198093525">

Obtains the capacity of a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1822472292093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p816942140093525">

HdfSbufGetDataSize (const struct HdfSBuf \*sbuf)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p253618620093525">

size_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p520982651093525">

Obtains the size of the data stored in a SBuf.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1551575615093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p242897082093525">

HdfSBufObtain (size_t capacity)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1636336211093525">

struct HdfSBuf \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1825696211093525">

Obtains a SBuf instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2051358946093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1183538243093525">

HdfSBufObtainDefaultSize (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p978386950093525">

struct HdfSBuf \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p988517038093525">

Obtains a SBuf instance of the default capacity (256 bytes).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row140948933093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2006883690093525">

HdfSBufBind (uintptr_t base, size_t size)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p575444769093525">

struct HdfSBuf \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p2147364148093525">

Creates a SBuf instance with the specified data and size. The pointer to
the data stored in the SBuf is released by the caller, and the written
data size should not exceed the specified value of size.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2083312985093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1453823374093525">

HdfSBufRecycle (struct HdfSBuf \*sbuf)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p545399945093525">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p266620797093525">

Releases a SBuf .

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1733619288093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p383764465093525">

HdfSBufMove (struct HdfSBuf \*sbuf)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1453777343093525">

struct HdfSBuf \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p359410378093525">

Creates a SBuf instance with an original SBuf. This function moves the
data stored in the original SBuf to the new one without memory copy.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row86060213093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p709082369093525">

HdfSBufCopy (const struct HdfSBuf \*sbuf)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1291900487093525">

struct HdfSBuf \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p40828725093525">

Creates a SBuf instance with an original SBuf. This function copies the
data stored in the original SBuf to the new one.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1418434977093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1900219461093525">

HdfSbufTransDataOwnership (struct HdfSBuf \*sbuf)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1723289234093525">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1024743160093525">

Transfers the data ownership to a SBuf. Once the SBuf is released, the
bound data memory is also released. This function is used together with
HdfSBufBind.

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
