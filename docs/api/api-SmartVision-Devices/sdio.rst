SDIO
====

**Overview**\ 
--------------

Declares standard APIs of basic secure digital input and output (SDIO)
capabilities.

You can use this module to access the SDIO and enable the driver to
operate an SDIO-compliant device. These capabilities include reading and
writing data based on SDIO, setting the block size, applying for and
releasing interrupts, enabling and disabling devices, and occupying and
releasing the bus.

**Since:**

1.0

**Summary**\ 
-------------

Files
-----

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1530939187093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1173097328093521">

File Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1026921565093521">

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

   <tr id="row1141730278093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1886511688093521">

sdio_if.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1700515241093521">

Declares the standard SDIO APIs.

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

Data Structures
---------------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row917125872093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p227473209093521">

Data Structure Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1637626164093521">

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

   <tr id="row712284064093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p940230443093521">

SdioFuncInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1199973939093521">

Defines the SDIO capabilities.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1937839706093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1880344750093521">

SdioCommonInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p800936819093521">

Defines SDIO common information.

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

Typedefs
--------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row204816141093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1057566833093521">

Typedef Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1004585508093521">

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

   <tr id="row739855849093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p996116088093521">

SdioIrqHandler(void \*)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1673184254093521">

typedef void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1165807439093521">

Defines the function type of an SDIO IRQ.

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

Enumerations
------------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1956670252093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p781209473093521">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p199347866093521">

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

   <tr id="row659342449093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p250620675093521">

SdioCommonInfoType { SDIO_FUNC_INFO = 0, SDIO_OTHER_INFO }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p491162443093521">

Enumerates SDIO common information types.

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

   <tr id="row1042110697093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1261466832093521">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1780200296093521">

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

   <tr id="row12113101093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p992391195093521">

SdioOpen (int16_t busNum)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1335213774093521">

struct DevHandle \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1665156749093521">

Opens an SDIO controller with a specified bus number.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2074470592093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1193210526093521">

SdioClose (struct DevHandle \*handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p115934128093521">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p820541544093521">

Closes an SDIO controller.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row246831540093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1292036525093521">

SdioReadBytes (struct DevHandle *handle, uint8_t*\ data, uint32_t addr,
uint32_t size, uint32_t timeOut)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p394512756093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p100187598093521">

Incrementally reads a given length of data from the specified SDIO
address.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row178475772093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1785212812093521">

SdioWriteBytes (struct DevHandle *handle, uint8_t*\ data, uint32_t addr,
uint32_t size, uint32_t timeOut)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2099986850093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1199546668093521">

Incrementally writes a given length of data into the specified SDIO
address.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1278083929093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1762187315093521">

SdioReadBytesFromFixedAddr (struct DevHandle *handle, uint8_t*\ data,
uint32_t addr, uint32_t size, uint32_t timeOut)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2063275176093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p498999545093521">

Reads a given length of data from the fixed SDIO address.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1883778016093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1943796427093521">

SdioWriteBytesToFixedAddr (struct DevHandle *handle, uint8_t*\ data,
uint32_t addr, uint32_t size, uint32_t timeOut)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1443139987093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p731405899093521">

Writes a given length of data into the fixed SDIO address.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2054189706093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p328763186093521">

SdioReadBytesFromFunc0 (struct DevHandle *handle, uint8_t*\ data,
uint32_t addr, uint32_t size, uint32_t timeOut)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p846143447093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p19637275093521">

Reads a given length of data from the address space of SDIO function 0.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row521019527093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p129199027093521">

SdioWriteBytesToFunc0 (struct DevHandle *handle, uint8_t*\ data,
uint32_t addr, uint32_t size, uint32_t timeOut)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p829617544093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p132557401093521">

Writes a given length of data into the address space of SDIO function 0.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1572140813093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1957228703093521">

SdioSetBlockSize (struct DevHandle \*handle, uint32_t blockSize)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p301642658093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p183444459093521">

Sets the block size.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row805217635093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p241444661093521">

SdioGetCommonInfo (struct DevHandle *handle, SdioCommonInfo*\ info,
SdioCommonInfoType infoType)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1936100396093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p25185804093521">

Obtains common information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row991461248093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p314052752093521">

SdioSetCommonInfo (struct DevHandle *handle, SdioCommonInfo*\ info,
SdioCommonInfoType infoType)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1941162057093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2061717887093521">

Sets common information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row282048750093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1466582138093521">

SdioFlushData (struct DevHandle \*handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1605730652093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2111394427093521">

Flushes data.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row268889763093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1578641189093521">

SdioClaimHost (struct DevHandle \*handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2133102691093521">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1493737635093521">

Claims a host exclusively.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1254701727093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p382167776093521">

SdioReleaseHost (struct DevHandle \*handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p172498001093521">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p940814814093521">

Releases the exclusively claimed host.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row262573471093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1037045944093521">

SdioEnableFunc (struct DevHandle \*handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1510520618093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2068308571093521">

Enables the SDIO device so that its register can be accessed.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1632671093093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2031699561093521">

SdioDisableFunc (struct DevHandle \*handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p854350571093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p338416749093521">

Disables the SDIO device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row661708051093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1410015653093521">

SdioClaimIrq (struct DevHandle *handle, SdioIrqHandler*\ irqHandler)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1875325263093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1717109204093521">

Claims an SDIO IRQ.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row389683943093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p358520322093521">

SdioReleaseIrq (struct DevHandle \*handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1902748560093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1760011885093521">

Releases an SDIO IRQ.

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

**Typedef Documentation**\ 
---------------------------

SdioIrqHandler
--------------

::

   typedef void SdioIrqHandler(void *)

**Description:**

Defines the function type of an SDIO IRQ.

This function is registered when you call
`SdioClaimIrq <sdio.md#ga81f98e541845c15a632cf59cd9c263f8>`__ to request
the SDIO IRQ.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row655106360093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1615362312093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1604471786093521">

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

   <tr id="row623759612093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

data

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the private data passed to this IRQ (The data is specified
when the IRQ is registered).

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Enumeration Type Documentation**\ 
------------------------------------

SdioCommonInfoType
------------------

::

   enum [SdioCommonInfoType](sdio.md#ga4037437ac001a9848dd242e8aa632678)

**Description:**

Enumerates SDIO common information types.

When obtaining SDIO common information by calling
`SdioGetCommonInfo <sdio.md#gac5c6bf733ea9e4408fd1109b18741ce8>`__ or
setting the information by calling
`SdioSetCommonInfo <sdio.md#ga563b67c90fbb88075bf5a05d9b5d5706>`__, you
need to pass the information type.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row105099053093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p453280380093521">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p472039072093521">

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

   <tr id="row936422258093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

SDIO_FUNC_INFO

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p674625696093521">

Functionality information

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row408912188093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

SDIO_OTHER_INFO

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1914756430093521">

Other information

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

**Function Documentation**\ 
----------------------------

SdioClaimHost()
---------------

::

   void SdioClaimHost (struct [DevHandle](devhandle.md) * handle)

**Description:**

Claims a host exclusively.

You can call this function to enable the SDIO module to exclusively
claim a host and then perform operations on the devices connected to the
host. After performing required operations, release the host by calling
`SdioReleaseHost <sdio.md#gabd2fe2d978e7fde51eba584f30dc8e7c>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2147008853093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2086040061093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p900061921093521">

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

   <tr id="row522622123093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the device handle of the SDIO controller
obtained by SdioOpen.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

SdioClaimIrq()
--------------

::

   int32_t SdioClaimIrq (struct [DevHandle](devhandle.md) * handle, [SdioIrqHandler](sdio.md#ga858bec274683a4f50d53d1f9f43d204b) * irqHandler )

**Description:**

Claims an SDIO IRQ.

When there is data, commands, or events, the IRQ function is executed.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row465971894093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1905903471093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1617545554093521">

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

   <tr id="row1034886858093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the device handle of the SDIO controller
obtained by SdioOpen.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1787715877093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

irqHandler

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the SDIO IRQ function. For details, see
SdioIrqHandler.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a negative value
if the operation fails.

SdioClose()
-----------

::

   void SdioClose (struct [DevHandle](devhandle.md) * handle)

**Description:**

Closes an SDIO controller.

After the SDIO interface is used, you can close the SDIO controller by
calling `SdioClose <sdio.md#ga15427d4b231423c6de812fedffbd61e3>`__. This
function is used in pair with
`SdioOpen <sdio.md#gadca7b0edcae3df85b3ade33704a306f8>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1658150651093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p355271575093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p618707820093521">

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

   <tr id="row1148892134093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the device handle of the SDIO controller.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

SdioDisableFunc()
-----------------

::

   int32_t SdioDisableFunc (struct [DevHandle](devhandle.md) * handle)

**Description:**

Disables the SDIO device.

This function is used in pair with
`SdioEnableFunc <sdio.md#ga2f31cd318990db879e827e3b8f9f2393>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row12515769093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1808583773093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p742498146093521">

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

   <tr id="row1951394195093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the device handle of the SDIO controller
obtained by SdioOpen.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a negative value
if the operation fails.

SdioEnableFunc()
----------------

::

   int32_t SdioEnableFunc (struct [DevHandle](devhandle.md) * handle)

**Description:**

Enables the SDIO device so that its register can be accessed.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1785098719093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1605563093093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2034352675093521">

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

   <tr id="row1672534765093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the device handle of the SDIO controller
obtained by SdioOpen.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a negative value
if the operation fails.

SdioFlushData()
---------------

::

   int32_t SdioFlushData (struct [DevHandle](devhandle.md) * handle)

**Description:**

Flushes data.

You can call this function when an SDIO needs to be reinitialized or an
unexpected error occurs.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1007800963093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1163141837093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p422772888093521">

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

   <tr id="row1977125136093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the device handle of the SDIO controller
obtained by SdioOpen.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a negative value
if the operation fails.

SdioGetCommonInfo()
-------------------

::

   int32_t SdioGetCommonInfo (struct [DevHandle](devhandle.md) * handle, [SdioCommonInfo](sdiocommoninfo.md) * info, [SdioCommonInfoType](sdio.md#ga4037437ac001a9848dd242e8aa632678) infoType )

**Description:**

Obtains common information.

You can call this function to obtain the capabilities and private data
of the I/O function.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row854623900093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p121177042093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1168811481093521">

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

   <tr id="row692197638093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the device handle of the SDIO controller
obtained by SdioOpen.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row869981547093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

info

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the common information to be obtained. For
details, see SdioCommonInfo.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2105866485093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

infoType

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the type of the common information to be obtained. For
details, see SdioCommonInfoType.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a negative value
if the operation fails.

SdioOpen()
----------

::

   struct [DevHandle](devhandle.md)* SdioOpen (int16_t busNum)

**Description:**

Opens an SDIO controller with a specified bus number.

Before using the SDIO interface, you can obtain the device handle of the
SDIO controller by calling
`SdioOpen <sdio.md#gadca7b0edcae3df85b3ade33704a306f8>`__. This function
is used in pair with
`SdioClose <sdio.md#ga15427d4b231423c6de812fedffbd61e3>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1022156567093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p195375023093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1036600373093521">

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

   <tr id="row909166475093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

busNum

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the bus number.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the device handle `DevHandle <devhandle.md>`__ of the SDIO
controller if the operation is successful; returns **NULL** otherwise.

SdioReadBytes()
---------------

::

   int32_t SdioReadBytes (struct [DevHandle](devhandle.md) * handle, uint8_t * data, uint32_t addr, uint32_t size, uint32_t timeOut )

**Description:**

Incrementally reads a given length of data from the specified SDIO
address.

If the length of the data to read is greater than the size of a block,
the data is read by block, and the remaining data that is smaller than
one block is read by byte. Otherwise, data is read by byte.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row539957154093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1406588321093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p546280427093521">

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

   <tr id="row1238652636093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the device handle of the SDIO controller
obtained by SdioOpen.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2113087413093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

data

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the data to read.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row391375230093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

addr

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the start address of the data to read.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1007713577093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

size

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the length of the data to read.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row50851260093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

timeOut

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the timeout duration for reading data, in milliseconds. If the
value is 0,the default value is used. The default value varies according
to the application. Generally, the default value is 1 second.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a negative value
if the operation fails.

SdioReadBytesFromFixedAddr()
----------------------------

::

   int32_t SdioReadBytesFromFixedAddr (struct [DevHandle](devhandle.md) * handle, uint8_t * data, uint32_t addr, uint32_t size, uint32_t timeOut )

**Description:**

Reads a given length of data from the fixed SDIO address.

If the length of the data to read is greater than the size of a block,
the data is read by block, and the remaining data that is smaller than
one block is read by byte. Otherwise, data is read by byte.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1186293101093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p506955628093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1575226023093521">

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

   <tr id="row236485686093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the device handle of the SDIO controller
obtained by SdioOpen.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row730848319093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

data

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the data to read.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1667016473093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

addr

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the fixed address of the data to read.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row876924867093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

size

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the length of the data to read.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row874519102093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

timeOut

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the timeout duration for reading data, in milliseconds. If the
value is 0, the default value is used. The default value varies
according to the application. Generally, the default value is 1 second.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a negative value
if the operation fails.

SdioReadBytesFromFunc0()
------------------------

::

   int32_t SdioReadBytesFromFunc0 (struct [DevHandle](devhandle.md) * handle, uint8_t * data, uint32_t addr, uint32_t size, uint32_t timeOut )

**Description:**

Reads a given length of data from the address space of SDIO function 0.

Currently, only one byte of data can be read.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row506852630093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p596417145093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p771038819093521">

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

   <tr id="row1025870798093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the device handle of the SDIO controller
obtained by SdioOpen.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row198642918093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

data

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the data to read.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row533646319093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

addr

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the start address of the data to read.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1979725897093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

size

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the length of the data to read.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1890045957093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

timeOut

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the timeout duration for reading data, in milliseconds. If the
value is 0, the default value is used. The default value varies
according to the application. Generally, the default value is 1 second.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a negative value
if the operation fails.

SdioReleaseHost()
-----------------

::

   void SdioReleaseHost (struct [DevHandle](devhandle.md) * handle)

**Description:**

Releases the exclusively claimed host.

This function is used in pair with
`SdioClaimHost <sdio.md#ga86e24b0480c860cfad8ff12fbc66bc9f>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1797607361093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1720927117093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p406098729093521">

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

   <tr id="row1978656463093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the device handle of the SDIO controller
obtained by SdioOpen.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

SdioReleaseIrq()
----------------

::

   int32_t SdioReleaseIrq (struct [DevHandle](devhandle.md) * handle)

**Description:**

Releases an SDIO IRQ.

This function is used in pair with
`SdioClaimIrq <sdio.md#ga81f98e541845c15a632cf59cd9c263f8>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1648083606093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p675509644093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1307012968093521">

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

   <tr id="row1485488927093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the device handle of the SDIO controller
obtained by SdioOpen.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a negative value
if the operation fails.

SdioSetBlockSize()
------------------

::

   int32_t SdioSetBlockSize (struct [DevHandle](devhandle.md) * handle, uint32_t blockSize )

**Description:**

Sets the block size.

If data to read or write is performed, use this function to set the
block size.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row649779753093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1153712898093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2064222067093521">

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

   <tr id="row844748385093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the device handle of the SDIO controller
obtained by SdioOpen.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1492693180093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

blockSize

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the block size to be set. If the value is 0, the default value
is used. The value ranges from 1 to 2048 bytes.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a negative value
if the operation fails.

SdioSetCommonInfo()
-------------------

::

   int32_t SdioSetCommonInfo (struct [DevHandle](devhandle.md) * handle, [SdioCommonInfo](sdiocommoninfo.md) * info, [SdioCommonInfoType](sdio.md#ga4037437ac001a9848dd242e8aa632678) infoType )

**Description:**

Sets common information.

You can call this function to set the maximum timeout duration and
private data.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1431464069093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p313469683093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1401177295093521">

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

   <tr id="row2094230835093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the device handle of the SDIO controller
obtained by SdioOpen.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row88000112093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

info

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the common information to be set. For details,
see SdioCommonInfo.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row505721311093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

infoType

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the type of the common information to be set. For details, see
SdioCommonInfoType.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a negative value
if the operation fails.

SdioWriteBytes()
----------------

::

   int32_t SdioWriteBytes (struct [DevHandle](devhandle.md) * handle, uint8_t * data, uint32_t addr, uint32_t size, uint32_t timeOut )

**Description:**

Incrementally writes a given length of data into the specified SDIO
address.

If the length of the data to write is greater than the size of a block,
the data is written by block first, and the remaining data that is
smaller than one block is written by byte. Otherwise, data is written by
byte.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1465973726093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1572153271093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1788496130093521">

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

   <tr id="row998619201093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the device handle of the SDIO controller
obtained by SdioOpen.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row938450147093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

data

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the data to write.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1871125226093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

addr

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the start address of the data to write.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row722659316093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

size

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the length of the data to write.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1594324977093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

timeOut

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the timeout duration for writing data, in milliseconds. If the
value is 0, the default value is used. The default value varies
according to the application. Generally, the default value is 1 second.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a negative value
if the operation fails.

SdioWriteBytesToFixedAddr()
---------------------------

::

   int32_t SdioWriteBytesToFixedAddr (struct [DevHandle](devhandle.md) * handle, uint8_t * data, uint32_t addr, uint32_t size, uint32_t timeOut )

**Description:**

Writes a given length of data into the fixed SDIO address.

If the length of the data to write is greater than the size of a block,
the data is written by block first, and the remaining data that is
smaller than one block is written by byte. Otherwise, data is written by
byte.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1550226375093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1950831094093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1130821132093521">

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

   <tr id="row1738347185093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the device handle of the SDIO controller
obtained by SdioOpen.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row38615993093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

data

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the data to write.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2109653110093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

addr

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the fixed address of the data to write.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row460442548093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

size

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the length of the data to write.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1362746796093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

timeOut

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the timeout duration for writing data, in milliseconds. If the
value is 0, the default value is used. The default value varies
according to the application. Generally, the default value is 1 second.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a negative value
if the operation fails.

SdioWriteBytesToFunc0()
-----------------------

::

   int32_t SdioWriteBytesToFunc0 (struct [DevHandle](devhandle.md) * handle, uint8_t * data, uint32_t addr, uint32_t size, uint32_t timeOut )

**Description:**

Writes a given length of data into the address space of SDIO function 0.

Currently, only one byte of data can be written.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1595079176093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p520761058093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1279188228093521">

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

   <tr id="row435996144093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

handle

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the device handle of the SDIO controller
obtained by SdioOpen.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row327099608093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

data

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the data to write.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2122130151093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

addr

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the start address of the data to write.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1956609249093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

size

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the length of the data to write.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row557957107093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

timeOut

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the timeout duration for writing data, in milliseconds. If the
value is 0, the default value is used. The default value varies
according to the application. Generally, the default value is 1 second.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a negative value
if the operation fails.
