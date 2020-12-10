HiLog
=====

**Overview**\ 
--------------

Provides logging functions.

For example, you can use these functions to output logs of the specified
log type, service domain, log tag, and log level.

**Since:**

1.1

**Version:**

1.0

**Summary**\ 
-------------

Macros
------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1597104279084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p360427726084827">

Macro Name and Value

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p781327426084827">

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

   <tr id="row494168097084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2087081212084827">

LOG_DOMAIN 0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p432230658084827">

Defines the service domain for a log file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1457448999084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p346078490084827">

LOG_TAG NULL

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p35795194084827">

Defines a string constant used to identify the class, file, or service
behavior.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2089815523084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1984128748084827">

HILOG_DEBUG(type, …) ((void)HiLogPrint(LOG_CORE, LOG_DEBUG, LOG_DOMAIN,
LOG_TAG, **VA_ARGS**))

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p476398349084827">

Outputs debug logs. This is a function-like macro.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1192149447084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1525739635084827">

HILOG_INFO(type, …) ((void)HiLogPrint(LOG_CORE, LOG_INFO, LOG_DOMAIN,
LOG_TAG, **VA_ARGS**))

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1124421452084827">

Outputs informational logs. This is a function-like macro.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1216563751084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1933426784084827">

HILOG_WARN(type, …) ((void)HiLogPrint(LOG_CORE, LOG_WARN, LOG_DOMAIN,
LOG_TAG, **VA_ARGS**))

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1325637840084827">

Outputs warning logs. This is a function-like macro.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row245554825084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p157471024084827">

HILOG_ERROR(type, …) ((void)HiLogPrint(LOG_CORE, LOG_ERROR, LOG_DOMAIN,
LOG_TAG, **VA_ARGS**))

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p577267807084827">

Outputs error logs. This is a function-like macro.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row251719571084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1489444690084827">

HILOG_FATAL(type, …) ((void)HiLogPrint(LOG_CORE, LOG_FATAL, LOG_DOMAIN,
LOG_TAG, **VA_ARGS**))

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p313270110084827">

Outputs fatal logs. This is a function-like macro.

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

   <tr id="row291960135084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p671438605084827">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p205870319084827">

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

   <tr id="row2019900190084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p112840239084827">

HiLogModuleType { HILOG_MODULE_HIVIEW = 0, HILOG_MODULE_SAMGR,
HILOG_MODULE_ACE, HILOG_MODULE_APP, HILOG_MODULE_MAX }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2056166851084827">

Enumerates logging module types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row42520667084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p212367100084827">

LogType

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2053177400084827">

Enumerates log types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row907974405084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2130828095084827">

LogLevel { LOG_DEBUG = 3, LOG_INFO = 4, LOG_WARN = 5, LOG_ERROR = 6,
LOG_FATAL = 7 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p889425769084827">

Enumerates log levels.

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

   <tr id="row1004807576084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p600572699084827">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1685310778084827">

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

   <tr id="row746524058084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1468624123084827">

HiLogPrint (LogType type, LogLevel level, unsigned int domain, const
char *tag, const char*\ fmt,…) **attribute**\ ((format(os_log

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1715696236084827">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1106796328084827">

Outputs logs.

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

**Macro Definition Documentation**\ 
------------------------------------

HILOG_DEBUG
-----------

::

   #define HILOG_DEBUG( type,  ... )   ((void)[HiLogPrint](hilog.rst#ga4c59c13fccc59c5821b23865fbc6380f)(LOG_CORE, [LOG_DEBUG](hilog.rst#ggaca1fd1d8935433e6ba2e3918214e07f9ab9f002c6ffbfd511da8090213227454e), [LOG_DOMAIN](hilog.rst#ga95a1d08c807e0aada863b5298a61d08d), [LOG_TAG](hilog.rst#ga7ce0df38eb467e59f209470c8f5ac4e6), __VA_ARGS__))

**Description:**

Outputs debug logs. This is a function-like macro.

Before calling this function, define the log service domain and log tag.
Generally, you need to define them at the beginning of the source file.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1678536392084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2008776417084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1493622621084827">

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

   <tr id="row417851097084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

type

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the log type. The type for third-party applications is defined
by LOG_APP.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1266446706084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

fmt

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the format string, which is an enhancement of a printf format
string and supports the privacy identifier. Specifically, {public} or
{private} is added between the % character and the format specifier in
each parameter.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row875858090084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

…

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates a list of parameters. The number and type of parameters must
map onto the format specifiers in the format string.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** or a larger value if the operation is successful; returns
a value smaller than **0** otherwise.

**See also:**

`HiLogPrint <hilog.rst#ga4c59c13fccc59c5821b23865fbc6380f>`__

HILOG_ERROR
-----------

::

   #define HILOG_ERROR( type,  ... )   ((void)[HiLogPrint](hilog.rst#ga4c59c13fccc59c5821b23865fbc6380f)(LOG_CORE, [LOG_ERROR](hilog.rst#ggaca1fd1d8935433e6ba2e3918214e07f9a230506cce5c68c3bac5a821c42ed3473), [LOG_DOMAIN](hilog.rst#ga95a1d08c807e0aada863b5298a61d08d), [LOG_TAG](hilog.rst#ga7ce0df38eb467e59f209470c8f5ac4e6), __VA_ARGS__))

**Description:**

Outputs error logs. This is a function-like macro.

Before calling this function, define the log service domain and log tag.
Generally, you need to define them at the beginning of the source file.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row63496823084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p133184696084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p497802116084827">

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

   <tr id="row597599697084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

type

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the log type. The type for third-party applications is defined
by LOG_APP.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row369424745084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

fmt

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the format string, which is an enhancement of a printf format
string and supports the privacy identifier. Specifically, {public} or
{private} is added between the % character and the format specifier in
each parameter.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1729814713084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

…

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates a list of parameters. The number and type of parameters must
map onto the format specifiers in the format string.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** or a larger value if the operation is successful; returns
a value smaller than **0** otherwise.

**See also:**

`HiLogPrint <hilog.rst#ga4c59c13fccc59c5821b23865fbc6380f>`__

HILOG_FATAL
-----------

::

   #define HILOG_FATAL( type,  ... )   ((void)[HiLogPrint](hilog.rst#ga4c59c13fccc59c5821b23865fbc6380f)(LOG_CORE, [LOG_FATAL](hilog.rst#ggaca1fd1d8935433e6ba2e3918214e07f9ac630750884d91cb9767ef2200bbb048b), [LOG_DOMAIN](hilog.rst#ga95a1d08c807e0aada863b5298a61d08d), [LOG_TAG](hilog.rst#ga7ce0df38eb467e59f209470c8f5ac4e6), __VA_ARGS__))

**Description:**

Outputs fatal logs. This is a function-like macro.

Before calling this function, define the log service domain and log tag.
Generally, you need to define them at the beginning of the source file.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1501940866084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2132286342084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p431657838084827">

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

   <tr id="row1613055158084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

type

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the log type. The type for third-party applications is defined
by LOG_APP.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row926439810084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

fmt

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the format string, which is an enhancement of a printf format
string and supports the privacy identifier. Specifically, {public} or
{private} is added between the % character and the format specifier in
each parameter.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row858238183084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

…

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates a list of parameters. The number and type of parameters must
map onto the format specifiers in the format string.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** or a larger value if the operation is successful; returns
a value smaller than **0** otherwise.

**See also:**

`HiLogPrint <hilog.rst#ga4c59c13fccc59c5821b23865fbc6380f>`__

HILOG_INFO
----------

::

   #define HILOG_INFO( type,  ... )   ((void)[HiLogPrint](hilog.rst#ga4c59c13fccc59c5821b23865fbc6380f)(LOG_CORE, [LOG_INFO](hilog.rst#ggaca1fd1d8935433e6ba2e3918214e07f9a6e98ff471e3ce6c4ef2d75c37ee51837), [LOG_DOMAIN](hilog.rst#ga95a1d08c807e0aada863b5298a61d08d), [LOG_TAG](hilog.rst#ga7ce0df38eb467e59f209470c8f5ac4e6), __VA_ARGS__))

**Description:**

Outputs informational logs. This is a function-like macro.

Before calling this function, define the log service domain and log tag.
Generally, you need to define them at the beginning of the source file.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row517106689084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p21771485084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1802927426084827">

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

   <tr id="row2019006136084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

type

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the log type. The type for third-party applications is defined
by LOG_APP.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row730545452084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

fmt

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the format string, which is an enhancement of a printf format
string and supports the privacy identifier. Specifically, {public} or
{private} is added between the % character and the format specifier in
each parameter.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1224188890084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

…

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates a list of parameters. The number and type of parameters must
map onto the format specifiers in the format string.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** or a larger value if the operation is successful; returns
a value smaller than **0** otherwise.

**See also:**

`HiLogPrint <hilog.rst#ga4c59c13fccc59c5821b23865fbc6380f>`__

HILOG_WARN
----------

::

   #define HILOG_WARN( type,  ... )   ((void)[HiLogPrint](hilog.rst#ga4c59c13fccc59c5821b23865fbc6380f)(LOG_CORE, [LOG_WARN](hilog.rst#ggaca1fd1d8935433e6ba2e3918214e07f9ac8041ffa22bc823d4726701cdb13fc13), [LOG_DOMAIN](hilog.rst#ga95a1d08c807e0aada863b5298a61d08d), [LOG_TAG](hilog.rst#ga7ce0df38eb467e59f209470c8f5ac4e6), __VA_ARGS__))

**Description:**

Outputs warning logs. This is a function-like macro.

Before calling this function, define the log service domain and log tag.
Generally, you need to define them at the beginning of the source file.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1820236389084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p417644358084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2031018500084827">

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

   <tr id="row1949269778084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

type

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the log type. The type for third-party applications is defined
by LOG_APP.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row406823050084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

fmt

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the format string, which is an enhancement of a printf format
string and supports the privacy identifier. Specifically, {public} or
{private} is added between the % character and the format specifier in
each parameter.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row71363213084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

…

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates a list of parameters. The number and type of parameters must
map onto the format specifiers in the format string.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** or a larger value if the operation is successful; returns
a value smaller than **0** otherwise.

**See also:**

`HiLogPrint <hilog.rst#ga4c59c13fccc59c5821b23865fbc6380f>`__

LOG_DOMAIN
----------

::

   #define LOG_DOMAIN   0

**Description:**

Defines the service domain for a log file.

The service domain is used to identify the subsystem and module of a
service. Its value is a hexadecimal integer ranging from 0x0 to 0xFFFFF.
If the value is beyond the range, its significant bits are automatically
truncated. The recommended format is 0xAAABB, where AAA indicates the
subsystem and BB indicates the module.

LOG_TAG
-------

::

   #define LOG_TAG   [NULL](utils.rst#ga070d2ce7b6bb7e5c05602aa8c308d0c4)

**Description:**

Defines a string constant used to identify the class, file, or service
behavior.

**Enumeration Type Documentation**\ 
------------------------------------

HiLogModuleType
---------------

::

   enum [HiLogModuleType](hilog.rst#ga125ab0014dcc2b2152e0be2e39e31b9e)

**Description:**

Enumerates logging module types.

The module type must be globally unique. A maximum of 64 module types
can be defined.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1219911279084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p442036558084827">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p122844742084827">

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

   <tr id="row1535133220084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

HILOG_MODULE_HIVIEW

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p280027297084827">

DFX

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2060924800084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

HILOG_MODULE_SAMGR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p602131848084827">

System Ability Manager

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1065924164084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

HILOG_MODULE_ACE

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1568512999084827">

Update

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2091650652084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

HILOG_MODULE_APP

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1121223202084827">

Third-party applications

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1602445119084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

HILOG_MODULE_MAX

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1372799855084827">

Maximum number of modules

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

LogLevel
--------

::

   enum [LogLevel](hilog.rst#gaca1fd1d8935433e6ba2e3918214e07f9)

**Description:**

Enumerates log levels.

You are advised to select log levels based on their respective usage
scenarios:

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1139806334084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1832212840084827">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1787015858084827">

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

   <tr id="row1783454580084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

LOG_DEBUG

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p405042248084827">

Debug level to be used by HILOG_DEBUG

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row527818007084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

LOG_INFO

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2121325691084827">

Informational level to be used by HILOG_INFO

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1761459427084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

LOG_WARN

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p465774437084827">

Warning level to be used by HILOG_WARN

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1700369515084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

LOG_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1327730145084827">

Error level to be used by HILOG_ERROR

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row440800791084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

LOG_FATAL

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1927959394084827">

Fatal level to be used by HILOG_FATAL

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

LogType
-------

::

   enum [LogType](hilog.rst#gaf67907baa897e9fb84df0cb89795b87c)

**Description:**

Enumerates log types.

Currently, **LOG_APP** is available.

**Function Documentation**\ 
----------------------------

HiLogPrint()
------------

::

   int HiLogPrint ([LogType](hilog.rst#gaf67907baa897e9fb84df0cb89795b87c) type, [LogLevel](hilog.rst#gaca1fd1d8935433e6ba2e3918214e07f9) level, unsigned int domain, const char * tag, const char * fmt,  ... )

**Description:**

Outputs logs.

You can use this function to output logs based on the specified log
type, log level, service domain, log tag, and variable parameters
determined by the format specifier and privacy identifier in the printf
format.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row753631955084827">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1401461885084827">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p926523287084827">

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

   <tr id="row1063972814084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

type

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the log type. The type for third-party applications is defined
by LOG_APP.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row417439105084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

level

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the log level, which can be LOG_DEBUG, LOG_INFO, LOG_WARN,
LOG_ERROR, and LOG_FATAL.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1294437284084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

domain

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the service domain of logs. Its value is a hexadecimal integer
ranging from 0x0 to 0xFFFFF. The recommended format is 0xAAABB, where
AAA indicates the subsystem and BB indicates the module.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row394419364084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

tag

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the log tag, which is a string used to identify the class,
file, or service behavior.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1915564046084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

fmt

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the format string, which is an enhancement of a printf format
string and supports the privacy identifier. Specifically, {public} or
{private} is added between the % character and the format specifier in
each parameter.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1555026651084827">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

…

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates a list of parameters. The number and type of parameters must
map onto the format specifiers in the format string.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** or a larger value if the operation is successful; returns
a value smaller than **0** otherwise.
