SubtitleTrackInfo
=================

**Overview**\ 
--------------

**Related Modules:**

`Format <format.md>`__

**Description:**

Defines subtitle stream information.

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

   <tr id="row1387054851093537">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p450220337093537">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1670804223093537">

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

   <tr id="row1641854632093537">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p352900465093537">

format

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p679887282093537">

SubtitleFormat

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row342940954093537">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1601083183093537">

charSet

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1638937567093537">

uint32_t

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row654950707093537">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1840499981093537">

language [FORMAT_MAX_LANGUAGE_NUM][FORMAT_LANGUAGE_LEN]

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2083829945093537">

char

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1500367991093537">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1087957239093537">

originalFrameWidth

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1325418658093537">

uint16_t

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row862987752093537">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1914503094093537">

originalFrameHeight

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p622491950093537">

uint16_t

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

charSet
-------

::

   uint32_t SubtitleTrackInfo::charSet

**Description:**

Character encoding format

format
------

::

   [SubtitleFormat](format.md#gadac45ce4731516c262292c15433439b3) SubtitleTrackInfo::format

**Description:**

Subtitle encoding and decoding format. For details, see
`SubtitleFormat <format.md#gadac45ce4731516c262292c15433439b3>`__

language
--------

::

   char SubtitleTrackInfo::language[[FORMAT_MAX_LANGUAGE_NUM](format.md#gac2d2d077edb8e9bb9f85ab6350015c5b)][[FORMAT_LANGUAGE_LEN](format.md#gaa70508bb1089c99f9aa3d59fcbdfa8eb)]

**Description:**

Subtitle language

originalFrameHeight
-------------------

::

   uint16_t SubtitleTrackInfo::originalFrameHeight

**Description:**

Height of the original image. This variable is valid for the image
subtitle.

originalFrameWidth
------------------

::

   uint16_t SubtitleTrackInfo::originalFrameWidth

**Description:**

Width of the original image. This variable is valid for the image
subtitle.
