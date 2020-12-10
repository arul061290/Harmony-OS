Kv_store
========

**Overview**\ 
--------------

Provides functions for obtaining, setting, and deleting a key-value
pair.

Key-value pairs can be permanently stored in the file system. If
`FEATURE_KV_CACHE <utils_config.rst#gad3d71669516ef0bb50e2b105507a6b29>`__
is enabled, key-value pairs can be stored in the cache. For details
about cache specifications, see
`MAX_CACHE_SIZE <utils_config.rst#ga6c8469dfe973ac952cf40394bd2c160b>`__.
For details about the number of key-value pairs that can be stored in an
application, see
`MAX_KV_SUM <utils_config.rst#ga4f258bd7d7d52c6770cce77f3e16ce72>`__.

**Since:**

1.0

**Version:**

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

   <tr id="row81307356093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p116958531093523">

File Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p776670871093523">

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

   <tr id="row1372341472093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p423909580093523">

kv_store.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1550572442093523">

Provides functions for obtaining, setting, and deleting a key-value
pair.

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

   <tr id="row823031703093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1509346248093523">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2057405299093523">

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

   <tr id="row1417798153093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p49307475093523">

UtilsGetValue (const char *key, char*\ value, unsigned int len)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p760301107093523">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p864377394093523">

Obtains the value matching a specified key from the file system or
cache.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row716465020093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2116782841093523">

UtilsSetValue (const char *key, const char*\ value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p699128253093523">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1288990351093523">

Adds or updates the value matching a specified key in the file system or
cache.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row233503164093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1246843873093523">

UtilsDeleteValue (const char \*key)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2071196472093523">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1007290304093523">

Deletes the value matching a specified key from the file system or
cache.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1184754742093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p807683216093523">

ClearKVCache (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p952916897093523">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p778710835093523">

Clears all key-value pairs from the cache.

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

**Function Documentation**\ 
----------------------------

ClearKVCache()
--------------

::

   int ClearKVCache (void )

**Description:**

Clears all key-value pairs from the cache.

**Attention:**

This function is available only if
`FEATURE_KV_CACHE <utils_config.rst#gad3d71669516ef0bb50e2b105507a6b29>`__
is enabled.

**Returns:**

Returns **0** if the operation is successful; returns **-1** otherwise.

UtilsDeleteValue()
------------------

::

   int UtilsDeleteValue (const char * key)

**Description:**

Deletes the value matching a specified key from the file system or
cache.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1250017617093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p985174083093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p202472848093523">

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

   <tr id="row1208464879093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

key

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the key whose value is to be deleted. It allows only lowercase
letters, digits, underscores (_), and dots (.). Its length cannot exceed
32 bytes (including the end-of-text character in the string).

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns **-9** if a
parameter is incorrect; returns **-1** in other scenarios.

UtilsGetValue()
---------------

::

   int UtilsGetValue (const char * key, char * value, unsigned int len )

**Description:**

Obtains the value matching a specified key from the file system or
cache.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row12309113093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1746431943093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2127740613093523">

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

   <tr id="row986534756093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

key

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the key to be indexed. It allows only lowercase letters,
digits, underscores (_), and dots (.). Its length cannot exceed 32 bytes
(including the end-of-text character in the string).

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2092775733093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

value

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the buffer for storing the value that matches the key. This is
an output parameter.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row835142831093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

len

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the size of the value space in the buffer.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the length of the value if the operation is successful; returns
**-9** if a parameter is incorrect; returns **-1** in other scenarios;
returns **0** if the value is obtained from the cache.

UtilsSetValue()
---------------

::

   int UtilsSetValue (const char * key, const char * value )

**Description:**

Adds or updates the value matching a specified key in the file system or
cache.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2083405762093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1384099041093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p946705848093523">

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

   <tr id="row1964164400093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

key

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the key whose value is to be added or updated. It allows only
lowercase letters, digits, underscores (_), and dots (.). Its length
cannot exceed 32 bytes (including the end-of-text character in the
string).

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row946893244093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

value

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the value to be added or updated. Its length cannot exceed 128
bytes (including the end-of-text character in the string).

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns **-9** if a
parameter is incorrect; returns **-1** in other scenarios.
