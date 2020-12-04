AudioTrackSourceInfo
====================

**Overview**\ 
--------------

**Related Modules:**

`Format <format.md>`__

**Description:**

Defines information about the muxer audio source.

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

   <tr id="row925051241093529">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p322533423093529">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p777640612093529">

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

   <tr id="row1746888656093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p932178404093529">

codecType

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1957845399093529">

CodecFormat

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2046697984093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p146712789093529">

sampleRate

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p987839260093529">

uint32_t

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row83543201093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1454175371093529">

channelCount

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1032551836093529">

uint32_t

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row128718947093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2076488370093529">

sampleBitWidth

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p378014238093529">

AudioSampleFmt

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row389651622093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p368290494093529">

samplesPerFrame

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p915342283093529">

uint32_t

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1442958936093529">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p688473273093529">

avgBytesPerSec

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1545524476093529">

uint32_t

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

avgBytesPerSec
--------------

::

   uint32_t AudioTrackSourceInfo::avgBytesPerSec

**Description:**

Average bit rate, in byte/s

channelCount
------------

::

   uint32_t AudioTrackSourceInfo::channelCount

**Description:**

Number of audio channels

codecType
---------

::

   [CodecFormat](format.md#gaf7ed135f15d4b218d41705bac0122ba7) AudioTrackSourceInfo::codecType

**Description:**

Audio encoding type, for details, see
`CodecFormat <format.md#gaf7ed135f15d4b218d41705bac0122ba7>`__.

sampleBitWidth
--------------

::

   [AudioSampleFmt](format.md#gadf0700999998f587f0017c4d02977b22) AudioTrackSourceInfo::sampleBitWidth

**Description:**

Bit width

sampleRate
----------

::

   uint32_t AudioTrackSourceInfo::sampleRate

**Description:**

Sampling rate

samplesPerFrame
---------------

::

   uint32_t AudioTrackSourceInfo::samplesPerFrame

**Description:**

Number of samples per frame
