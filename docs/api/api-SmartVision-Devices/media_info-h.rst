media_info.h
============

**Overview**\ 
--------------

**Related Modules:**

`MultiMedia_MediaCommon <multimedia_mediacommon.rst>`__

**Description:**

Declares the **media_info** class and provides various audio, video, and
codec types.

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

   <tr id="row207189671093526">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1038546848093526">

Data Structure Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p87440933093526">

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

   <tr id="row359263745093526">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p316172890093526">

AudioDeviceDesc

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p28103282093526">

Defines the audio Device Descriptor.

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

   <tr id="row1206028194093526">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p768265632093526">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1848240648093526">

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

   <tr id="row612826305093526">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1015004773093526">

AudioSourceType { AUDIO_SOURCE_INVALID = -1, AUDIO_SOURCE_DEFAULT = 0,
AUDIO_MIC = 1, AUDIO_VOICE_UPLINK = 2, AUDIO_VOICE_DOWNLINK = 3,
AUDIO_VOICE_CALL = 4, AUDIO_CAMCORDER = 5, AUDIO_VOICE_RECOGNITION = 6,
AUDIO_VOICE_COMMUNICATION = 7, AUDIO_REMOTE_SUBMIX = 8,
AUDIO_UNPROCESSED = 9, AUDIO_VOICE_PERFORMANCE = 10,
AUDIO_ECHO_REFERENCE = 1997, AUDIO_RADIO_TUNER = 1998, AUDIO_HOTWORD =
1999, AUDIO_REMOTE_SUBMIX_EXTEND = 10007 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1412858286093526">

Enumerates audio source types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row568792149093526">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p122980251093526">

AudioStreamType { TYPE_DEFAULT = -1, TYPE_MEDIA = 0,
TYPE_VOICE_COMMUNICATION = 1, TYPE_SYSTEM = 2, TYPE_RING = 3, TYPE_MUSIC
= 4, TYPE_ALARM = 5, TYPE_NOTIFICATION = 6, TYPE_BLUETOOTH_SCO = 7,
TYPE_ENFORCED_AUDIBLE = 8, TYPE_DTMF = 9, TYPE_TTS = 10,
TYPE_ACCESSIBILITY = 11 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1801310808093526">

Enumerates audio stream types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1387382207093526">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1642583390093526">

VideoCodecFormat { VIDEO_DEFAULT = 0, H264 = 2, HEVC = 5 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1689123451093526">

Enumerates video codec formats.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1669022832093526">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p484769561093526">

AudioCodecFormat { AUDIO_DEFAULT = 0, AAC_LC = 1, AAC_HE_V1 = 2,
AAC_HE_V2 = 3, AAC_LD = 4, AAC_ELD = 5, FORMAT_BUTT }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p862118676093526">

Enumerates audio codec formats.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2029883957093526">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1509291216093526">

AudioBitWidth { BIT_WIDTH_8 = 8, BIT_WIDTH_16 = 16, BIT_WIDTH_24 = 24,
BIT_WIDTH_BUTT }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p810860874093526">

Enumerates audio bit widths.

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
