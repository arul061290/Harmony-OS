uio.h
=====

**Overview**\ 
--------------

**Related Modules:**

`IO <io.rst>`__

**Description:**

Provides functions and structures related to input/output (I/O) to a
file or buffer.

You can use the functions provided in this file to read files to the
buffer or read information from the buffer to files.

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

   <tr id="row1839212327084833">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p749819170084833">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1844508993084833">

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

   <tr id="row192483031084833">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1603613644084833">

readv (int fd, const struct iovec \*iov, int iovcnt)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p922484154084833">

ssize_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p769354411084833">

Reads the data of fd to iov.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row722201382084833">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p783301121084833">

writev (int fd, const struct iovec \*iov, int iovcnt)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1481184841084833">

ssize_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1792103177084833">

Writes a given length of data into a file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1136210918084833">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p590329727084833">

preadv (int fd, const struct iovec \*iov, int iovcnt, off_t offset)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1382048568084833">

ssize_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1978634881084833">

Reads the data in a file whose fd offset is offset to the multi-group
buffer space pointed to by iov.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1934060607084833">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1552336291084833">

pwritev (int fd, const struct iovec \*iov, int iovcnt, off_t offset)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p704913409084833">

ssize_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p57694973084833">

Writes the data of a multi-group buffer space pointed to by iov to the
offset of fd.

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
