WifiIotSdioIntcallback
======================

**Overview**\ 
--------------

**Related Modules:**

`Wifiiot <wifiiot.md>`__

**Description:**

SDIO interrupt callback structure.

**Summary**\ 
-------------

Data Fields
-----------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1831554242191905">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1095179541191905">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p476159290191905">

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

   <tr id="row36091202191905">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1274073348191905">

RdstartCallback )(unsigned int len, unsigned char \*admaTable)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1164058388191905">

int(\*

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1191083268191905">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p428972021191905">

RdoverCallback )(void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1431112239191905">

int(\*

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row608469975191905">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p677066270191905">

RderrCallback )(void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1380495948191905">

void(\*

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1098806938191905">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p661550921191905">

WrstartCallback )(unsigned int len, unsigned char \*admaTable)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1688357698191905">

int(\*

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2134155235191905">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p99368724191905">

WroverCallback )(void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p544566900191905">

int(\*

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1961554200191905">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p861846226191905">

ProcessmsgCallback )(unsigned int msg)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1059648816191905">

void(\*

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1081933303191905">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p459889357191905">

SoftRstCallback )(void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2099023843191905">

void(\*

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

ProcessmsgCallback
------------------

::

   void(* WifiIotSdioIntcallback::ProcessmsgCallback) (unsigned int msg)

**Description:**

Callback invoked when a message is received from the host

RderrCallback
-------------

::

   void(* WifiIotSdioIntcallback::RderrCallback) (void)

**Description:**

Callback invoked when a data read failure occurs on the host

RdoverCallback
--------------

::

   int(* WifiIotSdioIntcallback::RdoverCallback) (void)

**Description:**

Callback invoked when the host finishes a read operation

RdstartCallback
---------------

::

   int(* WifiIotSdioIntcallback::RdstartCallback) (unsigned int len, unsigned char *admaTable)

**Description:**

Callback invoked when the host starts a read operation

SoftRstCallback
---------------

::

   void(* WifiIotSdioIntcallback::SoftRstCallback) (void)

**Description:**

Callback invoked when a soft reset interrupt message is received from
the host

WroverCallback
--------------

::

   int(* WifiIotSdioIntcallback::WroverCallback) (void)

**Description:**

Callback invoked when the host finishes a write operation

WrstartCallback
---------------

::

   int(* WifiIotSdioIntcallback::WrstartCallback) (unsigned int len, unsigned char *admaTable)

**Description:**

Callback invoked when the host starts a write operation
