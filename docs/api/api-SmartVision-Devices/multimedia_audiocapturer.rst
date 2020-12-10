MultiMedia_AudioCapturer
========================

**Overview**\ 
--------------

Declares APIs in the **AudioCapturer** class for audio capture.

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

   <tr id="row281774126093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p760854080093523">

File Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p345087334093523">

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

   <tr id="row199056235093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p832030572093523">

audio_capturer.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1474215149093523">

Provides the AudioCapturer class to implement operations related to
audio capture.

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

   <tr id="row1716835199093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p654037235093523">

Data Structure Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1985363718093523">

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

   <tr id="row830400461093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1752177379093523">

OHOS::Audio::AudioCapturerInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1105439788093523">

Defines information about audio capture parameters, including the input
source, audio codec format,sampling rate (Hz), number of audio channels,
bit rate, and bit width.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row827083412093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p605063776093523">

OHOS::Audio::Timestamp

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1267127982093523">

Represents timestamp information, including the frame position
information and high-resolution time source.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1206130843093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2040341407093523">

OHOS::Audio::AudioCapturer

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p443405516093523">

Provides functions for applications to implement audio capturing.

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

   <tr id="row626598362093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1398233995093523">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p627791589093523">

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

   <tr id="row2097356607093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p16627530093523">

OHOS::Audio::Timestamp::Timebase : int32_t {
OHOS::Audio::Timestamp::Timebase::MONOTONIC = 0,
OHOS::Audio::Timestamp::Timebase::BOOTTIME = 1 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1108117676093523">

Enumerates the time base of this Timestamp. Different timing methods are
supported.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row318899774093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p978432195093523">

OHOS::Audio::State : uint32_t { OHOS::Audio::PREPPARED,
OHOS::Audio::RECORDING, OHOS::Audio::STOPPED, OHOS::Audio::RELEASED }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1384403572093523">

Enumerates the recording states of the current device.

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

   <tr id="row832474254093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p741521712093523">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p767002807093523">

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

   <tr id="row697549128093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p105092068093523">

OHOS::Audio::AudioCapturer::GetMinFrameCount (int32_t sampleRate,
int32_t channelCount, AudioCodecFormat audioFormat, size_t &frameCount)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1099112656093523">

static bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p587438504093523">

Obtains the minimum number of frames required in a specified condition,
in bytes per sample.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1849680075093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p185550020093523">

OHOS::Audio::AudioCapturer::GetFrameCount ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p281355757093523">

uint64_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1488176989093523">

Obtains the number of frames required in the current condition, in bytes
per sample.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1380145864093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p410400896093523">

OHOS::Audio::AudioCapturer::SetCapturerInfo (const AudioCapturerInfo
info)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1453853380093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1930998009093523">

Sets audio capture parameters.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2570519093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p318887357093523">

OHOS::Audio::AudioCapturer::GetCapturerInfo (AudioCapturerInfo &info)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p373789560093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p929522756093523">

Obtains audio capture parameters.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2122078084093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p233934175093523">

OHOS::Audio::AudioCapturer::Start ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p423486984093523">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p675042620093523">

Starts audio recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row246760640093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1078306546093523">

OHOS::Audio::AudioCapturer::Read (uint8_t \*buffer, size_t userSize,
bool isBlockingRead)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p779980697093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p528029247093523">

Reads audio data.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row399772575093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1706221505093523">

OHOS::Audio::AudioCapturer::GetStatus ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p881850132093523">

State

.. raw:: html

   </p>

.. raw:: html

   <p id="p464111639093523">

Obtains the audio capture state.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row528923932093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p922758720093523">

OHOS::Audio::AudioCapturer::GetAudioTime (Timestamp &timestamp,
Timestamp::Timebase base)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p267444225093523">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p1500676067093523">

Obtains the timestamp.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1944334400093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2025601546093523">

OHOS::Audio::AudioCapturer::Stop ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2383751093523">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p1682546041093523">

Stops audio recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row648029978093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p860836606093523">

OHOS::Audio::AudioCapturer::Release ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1792460741093523">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p1751164000093523">

Releases a local AudioCapturer object.

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

**Enumeration Type Documentation**\ 
------------------------------------

State
-----

::

   enum [OHOS::Audio::State](multimedia_audiocapturer.rst#ga3d8d6798a2346e57e241d16da673d508) : uint32_t

**Description:**

Enumerates the recording states of the current device.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1555772384093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2018640151093523">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p266795546093523">

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

   <tr id="row1783391805093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PREPPARED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p831794065093523">

Prepared

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row396975875093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

RECORDING

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1032019183093523">

Recording

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1571220907093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

STOPPED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1762684314093523">

Stopped

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row762332383093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

RELEASED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2088942821093523">

Released

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

Timebase
--------

::

   enum [OHOS::Audio::Timestamp::Timebase](multimedia_audiocapturer.rst#gacdafb362a7da91799fa96163bca2a619) : int32_t

**Description:**

Enumerates the time base of this
`Timestamp <ohos-audio-timestamp.rst>`__. Different timing methods are
supported.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row452738220093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1077304416093523">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p57268637093523">

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

   <tr id="row413882644093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

MONOTONIC

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2043101740093523">

Monotonically increasing time, excluding the system sleep time

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row619950405093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

BOOTTIME

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p672856329093523">

Monotonically increasing time, including the system sleep time

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

GetAudioTime()
--------------

::

   bool OHOS::Audio::AudioCapturer::GetAudioTime ([Timestamp](ohos-audio-timestamp.rst) & timestamp, [Timestamp::Timebase](multimedia_audiocapturer.rst#gacdafb362a7da91799fa96163bca2a619) base )

**Description:**

Obtains the timestamp.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row59864883093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p275390714093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1323865753093523">

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

   <tr id="row21396200093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

timestamp

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates a Timestamp instance reference provided by the caller.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row431460639093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

base

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the time base, which can be Timestamp.Timebase.BOOTTIME or
Timestamp.Timebase.MONOTONIC.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **true** if the timestamp is successfully obtained; returns
**false** otherwise.

GetCapturerInfo()
-----------------

::

   int32_t OHOS::Audio::AudioCapturer::GetCapturerInfo ([AudioCapturerInfo](ohos-audio-audiocapturerinfo.rst) & info)

**Description:**

Obtains audio capture parameters.

This function can be called after
`SetCapturerInfo <multimedia_audiocapturer.rst#gae2cf055c840ece71e22cb64c98c68a19>`__
is successful.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1251500454093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1520900266093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1145789336093523">

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

   <tr id="row1230004267093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

info

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates information about audio capture parameters. For details, see
AudioCapturerInfo.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **SUCCESS** if the parameter information is successfully
obtained; returns an error code defined in
`media_errors.h <media_errors-h.rst>`__ otherwise.

GetFrameCount()
---------------

::

   uint64_t OHOS::Audio::AudioCapturer::GetFrameCount ()

**Description:**

Obtains the number of frames required in the current condition, in bytes
per sample.

**Returns:**

Returns the number of frames (in bytes per sample) if the operation is
successful; returns **-1** if an exception occurs.

GetMinFrameCount()
------------------

::

   static bool OHOS::Audio::AudioCapturer::GetMinFrameCount (int32_t sampleRate, int32_t channelCount, [AudioCodecFormat](multimedia_mediacommon.rst#gaa4ea6f314644ed287e0704be26c768b7) audioFormat, size_t & frameCount )

**Description:**

Obtains the minimum number of frames required in a specified condition,
in bytes per sample.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1818033582093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p185118153093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p678619483093523">

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

   <tr id="row1016102165093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

sampleRate

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the audio sampling rate, in Hz.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1302503898093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

channelCount

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the number of audio recording channels.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1233161577093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

audioFormat

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the audio data format.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row38715845093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

frameCount

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the minimum number of frames, in bytes per sample.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **true** if the minimum number of frames is successfully
obtained; returns **false** otherwise.

GetStatus()
-----------

::

   [State](multimedia_audiocapturer.rst#ga3d8d6798a2346e57e241d16da673d508) OHOS::Audio::AudioCapturer::GetStatus ()

**Description:**

Obtains the audio capture state.

**Returns:**

Returns the audio capture state defined in
`State <abilitykit.rst#ga5d74787dedbc4e11c1ab15bf487e61f8>`__.

Read()
------

::

   int32_t OHOS::Audio::AudioCapturer::Read (uint8_t * buffer, size_t userSize, bool isBlockingRead )

**Description:**

Reads audio data.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1929616111093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p421312409093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p611743463093523">

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

   <tr id="row1859611739093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

buffer

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the buffer into which the audio data is to be
written.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1484100718093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

userSize

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the size of the buffer into which the audio data is to be
written, in bytes. userSize >= frameCount \* channelCount \*
BytesPerSample must evaluate to true. You can call GetFrameCount to
obtain the frameCount value.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row613347253093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

isBlockingRead

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Specifies whether data reading will be blocked.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the size of the audio data read from the device. The value
ranges from **0** to **userSize**. If the reading fails, one of the
following error codes is returned: **ERR_INVALID_PARAM**: The input
parameter is incorrect. **ERR_ILLEGAL_STATE**: The
`AudioCapturer <ohos-audio-audiocapturer.rst>`__ instance is not
initialized. **ERR_SOURCE_NOT_SET**: The state of hardware device
instance is abnormal.

Release()
---------

::

   bool OHOS::Audio::AudioCapturer::Release ()

**Description:**

Releases a local `AudioCapturer <ohos-audio-audiocapturer.rst>`__ object.

**Returns:**

Returns **true** if the object is successfully released; returns
**false** otherwise.

SetCapturerInfo()
-----------------

::

   int32_t OHOS::Audio::AudioCapturer::SetCapturerInfo (const [AudioCapturerInfo](ohos-audio-audiocapturerinfo.rst) info)

**Description:**

Sets audio capture parameters.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row540741535093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1435211864093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p785800262093523">

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

   <tr id="row585017297093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

info

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates information about audio capture parameters to set. For
details, see AudioCapturerInfo.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **SUCCESS** if the setting is successful; returns an error code
defined in `media_errors.h <media_errors-h.rst>`__ otherwise.

Start()
-------

::

   bool OHOS::Audio::AudioCapturer::Start ()

**Description:**

Starts audio recording.

**Returns:**

Returns **true** if the recording is successfully started; returns
**false** otherwise.

Stop()
------

::

   bool OHOS::Audio::AudioCapturer::Stop ()

**Description:**

Stops audio recording.

**Returns:**

Returns **true** if the recording is successfully stopped; returns
**false** otherwise.

**Variable Documentation**\ 
----------------------------

audioFormat
-----------

::

   [AudioCodecFormat](multimedia_mediacommon.rst#gaa4ea6f314644ed287e0704be26c768b7) OHOS::Audio::AudioCapturerInfo::audioFormat = [AUDIO_DEFAULT](multimedia_mediacommon.rst#ggaa4ea6f314644ed287e0704be26c768b7a4c4c5829b054bc468274700c56d65546)

**Description:**

Audio codec format

bitRate
-------

::

   int32_t OHOS::Audio::AudioCapturerInfo::bitRate = 0

**Description:**

Bit rate

bitWidth
--------

::

   [AudioBitWidth](multimedia_mediacommon.rst#gae3e35ee2a2222a667fdebbc5b793ca7c) OHOS::Audio::AudioCapturerInfo::bitWidth = [BIT_WIDTH_16](multimedia_mediacommon.rst#ggae3e35ee2a2222a667fdebbc5b793ca7ca036f0b45813f96cb6b0f90de1722a780)

**Description:**

Bit width

channelCount
------------

::

   int32_t OHOS::Audio::AudioCapturerInfo::channelCount = 0

**Description:**

Number of audio channels

inputSource
-----------

::

   [AudioSourceType](multimedia_mediacommon.rst#gadc3158e093b995ca7b9b6aa32388ccdd) OHOS::Audio::AudioCapturerInfo::inputSource = [AUDIO_MIC](multimedia_mediacommon.rst#ggadc3158e093b995ca7b9b6aa32388ccdda732604b3a24d137429e2b83b31849bce)

**Description:**

Audio source type

sampleRate
----------

::

   int32_t OHOS::Audio::AudioCapturerInfo::sampleRate = 0

**Description:**

Sampling rate

streamType
----------

::

   [AudioStreamType](multimedia_mediacommon.rst#gae7077e4211e48131ae544adb20fc494a) OHOS::Audio::AudioCapturerInfo::streamType = [TYPE_MEDIA](multimedia_mediacommon.rst#ggae7077e4211e48131ae544adb20fc494aa431e273affaa22e18ec5a2a548b70e90)

**Description:**

Audio stream type
