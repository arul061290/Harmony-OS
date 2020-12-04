mqueue.h
========

**Overview**\ 
--------------

**Related Modules:**

`IPC <ipc.md>`__

**Description:**

Provides message queue operation functions and related structures.

For example, you can use the functions to create, open, close, delete,
read, and write a message queue, and to obtain and set its attributes.

**Since:**

1.0

**Version:**

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

   <tr id="row1357532096084831">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1126610916084831">

Data Structure Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p598848476084831">

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

   <tr id="row1623340061084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1853045994084831">

mq_attr

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1589392064084831">

Describes message queue attributes.

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

   <tr id="row1586553151084831">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p557343322084831">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p542346034084831">

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

   <tr id="row528002848084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p963714008084831">

mq_close (mqd_t mqdes)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1652431109084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p156856598084831">

Closes a message queue that is no longer used.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1749386662084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p164735842084831">

mq_getattr (mqd_t mqdes, struct mq_attr \*attr)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p839744025084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1347121667084831">

Obtains the attributes of the message queue specified by the descriptor.
The values of mq_maxmsg, mq_msgsize, and mq_curmsgs are fixed.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1837364552084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1509502087084831">

mq_open (const char \*name, int oflag,…)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p388697709084831">

mqd_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p304639038084831">

Creates a message queue or opens an existing message queue.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1351135507084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p492271851084831">

mq_receive (mqd_t mqdes, char *buffer, size_t size, unsigned*\ prioptr)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1624789446084831">

ssize_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p393717103084831">

Receives a message from a specified message queue.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1898195847084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1407021360084831">

mq_send (mqd_t mqdes, const char \*buffer, size_t size, unsigned prio)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p740878554084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p245727963084831">

Sends a message to a specified message queue.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1800643802084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1847885701084831">

mq_setattr (mqd_t mqdes, const struct mq_attr \*__restrict newattr,
struct mq_attr \*__restrict oldattr)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p986131364084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1356206786084831">

Sets the attributes of the message queue specified by the descriptor.
The mq_maxmsg, mq_msgsize, and mq_curmsgs attributes cannot be modified.
mq_flags supports the O_NONBLOCK attribute only.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1970642142084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1238632493084831">

mq_timedreceive (mqd_t mqdes, char \*__restrict buffer, size_t size,
unsigned \*__restrict prioptr, const struct timespec \*__restrict
timeout)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p251191204084831">

ssize_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p515032415084831">

Receives a message from the message queue, with a timeout period
specified.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row703504034084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1911150045084831">

mq_timedsend (mqd_t mqdes, const char *buffer, size_t size, unsigned
prio, const struct timespec*\ timeout)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1313176928084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p946847412084831">

Sends a message to a specified message queue, with a timeout period
specified.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2127330527084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p551784950084831">

mq_unlink (const char \*name)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p443714017084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p775559004084831">

Decreases the reference count of the message queue by 1, or deletes the
message queue if the reference count is 0.

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
