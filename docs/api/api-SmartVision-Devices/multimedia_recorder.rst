MultiMedia_Recorder
===================

**Overview**\ 
--------------

Defines the **Recorder** class and provides functions for audio and
video recording.

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

   <tr id="row724422408093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p962291851093523">

File Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p887923986093523">

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

   <tr id="row358706440093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p509528581093523">

recorder.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1766380674093523">

Declares the Recorder class for audio and video recording.

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

   <tr id="row1381956710093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p361122150093523">

Data Structure Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p342510055093523">

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

   <tr id="row1428479655093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p654847711093523">

OHOS::Media::RecorderCallback

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p101469680093523">

Provides listeners for recording errors and information events.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1690965223093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1204898035093523">

OHOS::Media::Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1182251503093523">

Provides functions for audio and video recording.

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

   <tr id="row1064759830093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1221426325093523">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p364708938093523">

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

   <tr id="row1261026490093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1068013999093523">

OHOS::Media::VideoSourceType : int32_t {
OHOS::Media::VIDEO_SOURCE_SURFACE_YUV = 0,
OHOS::Media::VIDEO_SOURCE_SURFACE_RGB,
OHOS::Media::VIDEO_SOURCE_SURFACE_ES, OHOS::Media::VIDEO_SOURCE_BUTT }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2029982052093523">

Enumerates video source types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2045210593093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p475769915093523">

OHOS::Media::DataSourceType : int32_t { OHOS::Media::IMAGE = 0 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2088001454093523">

Enumerates data source types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1965596020093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1985802987093523">

OHOS::Media::OutputFormatType : int32_t { OHOS::Media::FORMAT_DEFAULT =
0, OHOS::Media::FORMAT_MPEG_4, OHOS::Media::FORMAT_TS }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1956812075093523">

Enumerates output file formats.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1063334872093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p498897192093523">

OHOS::Media::FileSplitType : int32_t { OHOS::Media::FILE_SPLIT_POST = 0,
OHOS::Media::FILE_SPLIT_PRE, OHOS::Media::FILE_SPLIT_NORMAL }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1341343376093523">

Enumerates file split types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row130781735093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1225608326093523">

OHOS::Media::RecorderCallback::RecorderInfoType : int32_t {
OHOS::Media::RecorderCallback::RECORDER_INFO_MAX_DURATION_APPROACHING =
0,
OHOS::Media::RecorderCallback::RECORDER_INFO_MAX_FILESIZE_APPROACHING,
OHOS::Media::RecorderCallback::RECORDER_INFO_MAX_DURATION_REACHED,
OHOS::Media::RecorderCallback::RECORDER_INFO_MAX_FILESIZE_REACHED,
OHOS::Media::RecorderCallback::RECORDER_INFO_NEXT_OUTPUT_FILE_STARTED,
OHOS::Media::RecorderCallback::RECORDER_INFO_FILE_SPLIT_FINISHED,
OHOS::Media::RecorderCallback::RECORDER_INFO_FILE_START_TIME_MS }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p393522808093523">

Enumerates recording information types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row672972126093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1733371720093523">

OHOS::Media::RecorderCallback::RecorderErrorType : int32_t {
OHOS::Media::RecorderCallback::RECORDER_ERROR_UNKNOWN = 0 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1370492358093523">

Enumerates recording error types.

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

   <tr id="row298029774093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1381964017093523">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1254649978093523">

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

   <tr id="row680952673093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p311949488093523">

OHOS::Media::RecorderCallback::OnError (int32_t errorType, int32_t
errorCode)=0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1313409662093523">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p278837618093523">

Called when an error occurs during recording. This callback is used to
report recording errors.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1070068931093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p619947014093523">

OHOS::Media::RecorderCallback::OnInfo (int32_t type, int32_t extra)=0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1994195754093523">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1348861506093523">

Called when an information event occurs during recording. This callback
is used to report recording information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1526380767093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p851817420093523">

OHOS::Media::Recorder::SetVideoSource (VideoSourceType source, int32_t
&sourceId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p861930323093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p342420130093523">

Sets a video source for recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1341511907093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p730635022093523">

OHOS::Media::Recorder::SetVideoEncoder (int32_t sourceId,
VideoCodecFormat encoder)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p511933924093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1129969036093523">

Sets a video encoder for recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row984175353093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1827890926093523">

OHOS::Media::Recorder::SetVideoSize (int32_t sourceId, int32_t width,
int32_t height)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1648761074093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p971937993093523">

Sets the width and height of the video to record.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1502358505093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1715099754093523">

OHOS::Media::Recorder::SetVideoFrameRate (int32_t sourceId, int32_t
frameRate)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p434750406093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1135465591093523">

Sets the frame rate of the video to record.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row659993171093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p754783501093523">

OHOS::Media::Recorder::SetVideoEncodingBitRate (int32_t sourceId,
int32_t rate)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1245304126093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p399229193093523">

Sets the encoding bit rate of the video to record.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row565451701093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p883876237093523">

OHOS::Media::Recorder::SetCaptureRate (int32_t sourceId, double fps)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1834500411093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2120855576093523">

Sets the video capture rate.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row746956947093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2092630755093523">

OHOS::Media::Recorder::GetSurface (int32_t sourceId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p824930314093523">

std::shared_ptr< OHOS::Surface >

.. raw:: html

   </p>

.. raw:: html

   <p id="p375303447093523">

Obtains the surface of the video source.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1637444827093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2106303438093523">

OHOS::Media::Recorder::SetAudioSource (AudioSourceType source, int32_t
&sourceId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1529812778093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1674163893093523">

Sets the audio source for recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1599143268093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p962667576093523">

OHOS::Media::Recorder::SetAudioEncoder (int32_t sourceId,
AudioCodecFormat encoder)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2145397412093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1256882371093523">

Sets an audio encoder for recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row41076208093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p44305558093523">

OHOS::Media::Recorder::SetAudioSampleRate (int32_t sourceId, int32_t
rate)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1017986136093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p233204830093523">

Sets the audio sampling rate for recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row340783059093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p314499125093523">

OHOS::Media::Recorder::SetAudioChannels (int32_t sourceId, int32_t num)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p348158986093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p986547458093523">

Sets the number of audio channels to record.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1620348805093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1018418847093523">

OHOS::Media::Recorder::SetAudioEncodingBitRate (int32_t sourceId,
int32_t bitRate)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p67726740093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1180978883093523">

Sets the encoding bit rate of the audio to record.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1010578046093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1837015058093523">

OHOS::Media::Recorder::SetMaxDuration (int32_t duration)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1712475210093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2006472955093523">

Sets the maximum duration of a recorded file, in seconds.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row822728472093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p636672898093523">

OHOS::Media::Recorder::SetOutputFormat (OutputFormatType format)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1205080832093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1723249559093523">

Sets the output file format.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row67569527093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p90666847093523">

OHOS::Media::Recorder::SetOutputPath (const string &path)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p105944087093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1194503349093523">

Sets the output file path.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1417224560093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1528642964093523">

OHOS::Media::Recorder::SetOutputFile (int32_t fd)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2096877714093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1736440839093523">

Sets the file descriptor (FD) of the output file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1597450936093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1012707093093523">

OHOS::Media::Recorder::SetNextOutputFile (int32_t fd)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p688967428093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1143389253093523">

Sets the FD of the next output file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row136176043093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1887364289093523">

OHOS::Media::Recorder::SetMaxFileSize (int64_t size)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p348672136093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2093166439093523">

Sets the maximum size of a recorded file, in bytes.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1310396059093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p462346016093523">

OHOS::Media::Recorder::SetRecorderCallback (const std::shared_ptr<
RecorderCallback > &callback)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2020418399093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1289408181093523">

Registers a recording listener.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1661232613093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p137661708093523">

OHOS::Media::Recorder::Prepare ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p801196611093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1600774546093523">

Prepares for recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row264294094093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p963314626093523">

OHOS::Media::Recorder::Start ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p744615776093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1226381872093523">

Starts recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row36417538093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1785094087093523">

OHOS::Media::Recorder::Pause ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1193676080093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p923942917093523">

Pauses recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row436389210093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1742531283093523">

OHOS::Media::Recorder::Resume ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1588446860093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1369556172093523">

Resumes recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row39152720093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1494107474093523">

OHOS::Media::Recorder::Stop (bool block)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1822612433093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2105484633093523">

Stops recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1327466878093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1935301857093523">

OHOS::Media::Recorder::Reset ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1916936186093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1782042779093523">

Resets the recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row526526578093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p662646081093523">

OHOS::Media::Recorder::Release ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p882489397093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1430619621093523">

Releases recording resources.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1538317046093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1021960870093523">

OHOS::Media::Recorder::SetFileSplitDuration (FileSplitType type, int64_t
timestamp, uint32_t duration)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p800583402093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1930024465093523">

Manually splits a video.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1985417361093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p889404626093523">

OHOS::Media::Recorder::SetParameter (int32_t sourceId, const Format
&format)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p154156846093523">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p422488051093523">

Sets an extended parameter for recording, for example,
RCORDER_PRE_CACHE_DURATION.

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

DataSourceType
--------------

::

   enum [OHOS::Media::DataSourceType](multimedia_recorder.rst#gaccc05bb178cecd760369ea096dceae4c) : int32_t

**Description:**

Enumerates data source types.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row770590823093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1910554636093523">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1042913223093523">

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

   <tr id="row12441992093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

IMAGE

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2053372660093523">

Image data source

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

FileSplitType
-------------

::

   enum [OHOS::Media::FileSplitType](multimedia_recorder.rst#ga8759c7e5a74964a584a716f4ec0b7edb) : int32_t

**Description:**

Enumerates file split types.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row362078692093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p300431219093523">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1922922311093523">

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

   <tr id="row1511002547093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

FILE_SPLIT_POST

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1831428027093523">

Delayed/Backward split

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1582277442093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

FILE_SPLIT_PRE

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1856106944093523">

Advanced/Forward split

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1612141546093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

FILE_SPLIT_NORMAL

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p448292730093523">

Normal split

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

OutputFormatType
----------------

::

   enum [OHOS::Media::OutputFormatType](multimedia_recorder.rst#ga3dfe2e61369bf1c081ce569e235354df) : int32_t

**Description:**

Enumerates output file formats.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2068157643093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p591443768093523">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1207949339093523">

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

   <tr id="row401334839093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

FORMAT_DEFAULT

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1474627517093523">

Default format

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row525711402093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

FORMAT_MPEG_4

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p724729632093523">

MPEG4 format

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row363534513093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

FORMAT_TS

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1729314644093523">

TS format

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

RecorderErrorType
-----------------

::

   enum [OHOS::Media::RecorderCallback::RecorderErrorType](multimedia_recorder.rst#ga5132172c298fc1497d12040b6bd511cf) : int32_t

**Description:**

Enumerates recording error types.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row131020063093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p595048386093523">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1746122499093523">

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

   <tr id="row1168494199093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

RECORDER_ERROR_UNKNOWN

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1068364417093523">

Unknown error

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

RecorderInfoType
----------------

::

   enum [OHOS::Media::RecorderCallback::RecorderInfoType](multimedia_recorder.rst#ga0db5cf9cc68d4b468e921a563248ffe0) : int32_t

**Description:**

Enumerates recording information types.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1068887372093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p125639071093523">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2108672840093523">

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

   <tr id="row2016374018093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

RECORDER_INFO_MAX_DURATION_APPROACHING

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1886640347093523">

The recording duration is reaching the threshold specified by
SetMaxDuration. This type of information is reported when only one
second or 10% is left to reach the allowed duration.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row453829915093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

RECORDER_INFO_MAX_FILESIZE_APPROACHING

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1853487662093523">

The recorded file size is reaching the threshold specified by
SetMaxFileSize. This type of information is reported when only 100 KB or
10% is left to reach the allowed size.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1054656266093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

RECORDER_INFO_MAX_DURATION_REACHED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p679522627093523">

The threshold specified by SetMaxDuration is reached, and the recording
ends. Before calling SetOutputFile, you must close the file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row114794316093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

RECORDER_INFO_MAX_FILESIZE_REACHED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1034691151093523">

The threshold specified by SetMaxFileSize is reached, and the recording
ends. Before calling SetOutputFile, you must close the file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1960269044093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

RECORDER_INFO_NEXT_OUTPUT_FILE_STARTED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1326591732093523">

Recording started for the next output file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1216758142093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

RECORDER_INFO_FILE_SPLIT_FINISHED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p91095480093523">

Manual file split completed.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1941101101093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

RECORDER_INFO_FILE_START_TIME_MS

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p245760745093523">

The start time position of the recording file is not supported.

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

VideoSourceType
---------------

::

   enum [OHOS::Media::VideoSourceType](multimedia_recorder.rst#gad252d27f9ce4b6ae0756bfeaa5f34490) : int32_t

**Description:**

Enumerates video source types.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1205861817093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1469195750093523">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1963925989093523">

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

   <tr id="row1528060699093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

VIDEO_SOURCE_SURFACE_YUV

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p444084281093523">

YUV video data provided through Surface

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1745386000093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

VIDEO_SOURCE_SURFACE_RGB

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1699753232093523">

RGB video data provided through Surface

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1876028535093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

VIDEO_SOURCE_SURFACE_ES

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p791679739093523">

Raw encoded data provided through Surface

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row649505798093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

VIDEO_SOURCE_BUTT

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p229968933093523">

Invalid value

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

GetSurface()
------------

::

   std::shared_ptr<[OHOS::Surface](ohos-surface.rst)> OHOS::Media::Recorder::GetSurface (int32_t sourceId)

**Description:**

Obtains the surface of the video source.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row945082100093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1393130046093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1802972058093523">

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

   <tr id="row124823954093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

sourceId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the video source ID, which can be obtained from
SetVideoSource.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the pointer to the surface.

OnError()
---------

::

   virtual void OHOS::Media::RecorderCallback::OnError (int32_t errorType, int32_t errorCode )

**Description:**

Called when an error occurs during recording. This callback is used to
report recording errors.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row122153233093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1553906841093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1099190524093523">

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

   <tr id="row1796503621093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

errorType

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the error type. For details, see RecorderErrorType.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row213208190093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

errorCode

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the error code.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

OnInfo()
--------

::

   virtual void OHOS::Media::RecorderCallback::OnInfo (int32_t type, int32_t extra )

**Description:**

Called when an information event occurs during recording. This callback
is used to report recording information.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row360780068093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p9950185093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1467462054093523">

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

   <tr id="row1563342110093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

type

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the information type. For details, see RecorderInfoType.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row529220958093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

extra

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates other information, for example, the start time position of a
recording file.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

Pause()
-------

::

   int32_t OHOS::Media::Recorder::Pause ()

**Description:**

Pauses recording.

After
`Start <multimedia_recorder.rst#gac3aaa32627f0799dea65e51356b91bfb>`__ is
called, you can call this function to pause recording. The audio and
video source streams are not paused, and source data is discarded.

**Returns:**

Returns **SUCCESS** if the recording is paused; returns an error code
defined in `media_errors.h <media_errors-h.rst>`__ otherwise.

Prepare()
---------

::

   int32_t OHOS::Media::Recorder::Prepare ()

**Description:**

Prepares for recording.

This function must be called before
`Start <multimedia_recorder.rst#gac3aaa32627f0799dea65e51356b91bfb>`__.

**Returns:**

Returns **SUCCESS** if the preparation is successful; returns an error
code defined in `media_errors.h <media_errors-h.rst>`__ otherwise.

Release()
---------

::

   int32_t OHOS::Media::Recorder::Release ()

**Description:**

Releases recording resources.

**Returns:**

Returns **SUCCESS** if recording resources are released; returns an
error code defined in `media_errors.h <media_errors-h.rst>`__ otherwise.

Reset()
-------

::

   int32_t OHOS::Media::Recorder::Reset ()

**Description:**

Resets the recording.

After the function is called, add a recording source by calling
`SetVideoSource <multimedia_recorder.rst#ga9e12ef9700d06c7620f9e3d7b4d844ca>`__
or
`SetAudioSource <multimedia_recorder.rst#gae287f59da8b3f1b6ca9f1c0e58a6565a>`__,
set related parameters, and call
`Start <multimedia_recorder.rst#gac3aaa32627f0799dea65e51356b91bfb>`__ to
start recording again after
`Prepare <multimedia_recorder.rst#ga15d2f3416bb735a0715e1e79be226387>`__
is called.

**Returns:**

Returns **SUCCESS** if the recording is reset; returns an error code
defined in `media_errors.h <media_errors-h.rst>`__ otherwise.

Resume()
--------

::

   int32_t OHOS::Media::Recorder::Resume ()

**Description:**

Resumes recording.

You can call this function to resume recording after
`Pause <multimedia_recorder.rst#ga71da5cc2720b336f0daadbe09d61c695>`__ is
called.

**Returns:**

Returns **SUCCESS** if the recording is resumed; returns an error code
defined in `media_errors.h <media_errors-h.rst>`__ otherwise.

SetAudioChannels()
------------------

::

   int32_t OHOS::Media::Recorder::SetAudioChannels (int32_t sourceId, int32_t num )

**Description:**

Sets the number of audio channels to record.

This function must be called after
`SetAudioSource <multimedia_recorder.rst#gae287f59da8b3f1b6ca9f1c0e58a6565a>`__
but before
`Prepare <multimedia_recorder.rst#ga15d2f3416bb735a0715e1e79be226387>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1686511852093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p664707833093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1087257130093523">

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

   <tr id="row1635462250093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

sourceId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the audio source ID, which can be obtained from
SetAudioSource.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2132087717093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

num

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the number of audio channels to set.

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

SetAudioEncoder()
-----------------

::

   int32_t OHOS::Media::Recorder::SetAudioEncoder (int32_t sourceId, [AudioCodecFormat](multimedia_mediacommon.rst#gaa4ea6f314644ed287e0704be26c768b7) encoder )

**Description:**

Sets an audio encoder for recording.

If this function is not called, the output file does not contain the
audio track. This function must be called after
`SetAudioSource <multimedia_recorder.rst#gae287f59da8b3f1b6ca9f1c0e58a6565a>`__
but before
`Prepare <multimedia_recorder.rst#ga15d2f3416bb735a0715e1e79be226387>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row740841607093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1277783970093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p728407760093523">

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

   <tr id="row1444556306093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

sourceId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the audio source ID, which can be obtained from
SetAudioSource.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1640399120093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

encoder

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the audio encoder to set.

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

SetAudioEncodingBitRate()
-------------------------

::

   int32_t OHOS::Media::Recorder::SetAudioEncodingBitRate (int32_t sourceId, int32_t bitRate )

**Description:**

Sets the encoding bit rate of the audio to record.

This function must be called after
`SetAudioSource <multimedia_recorder.rst#gae287f59da8b3f1b6ca9f1c0e58a6565a>`__
but before
`Prepare <multimedia_recorder.rst#ga15d2f3416bb735a0715e1e79be226387>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1352532493093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p577931526093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1368329758093523">

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

   <tr id="row805703230093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

sourceId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the audio source ID, which can be obtained from
SetAudioSource.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row356917711093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

bitRate

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the audio encoding bit rate, in bit/s.

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

SetAudioSampleRate()
--------------------

::

   int32_t OHOS::Media::Recorder::SetAudioSampleRate (int32_t sourceId, int32_t rate )

**Description:**

Sets the audio sampling rate for recording.

This function must be called after
`SetAudioSource <multimedia_recorder.rst#gae287f59da8b3f1b6ca9f1c0e58a6565a>`__
but before
`Prepare <multimedia_recorder.rst#ga15d2f3416bb735a0715e1e79be226387>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row436334477093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p41560066093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2117572107093523">

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

   <tr id="row2137761213093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

sourceId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the audio source ID, which can be obtained from
SetAudioSource.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row746044201093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

rate

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the sampling rate of the audio per second.

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

SetAudioSource()
----------------

::

   int32_t OHOS::Media::Recorder::SetAudioSource ([AudioSourceType](multimedia_mediacommon.rst#gadc3158e093b995ca7b9b6aa32388ccdd) source, int32_t & sourceId )

**Description:**

Sets the audio source for recording.

If this function is not called, the output file does not contain the
audio track.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1750629795093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p384507655093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p310601790093523">

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

   <tr id="row32836669093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

source

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the audio source type. For details, see AudioSourceType.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row61171699093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

sourceId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the audio source ID. The value -1 indicates an invalid ID and
the setting fails.

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

SetCaptureRate()
----------------

::

   int32_t OHOS::Media::Recorder::SetCaptureRate (int32_t sourceId, double fps )

**Description:**

Sets the video capture rate.

This function must be called after
`SetVideoSource <multimedia_recorder.rst#ga9e12ef9700d06c7620f9e3d7b4d844ca>`__
but before
`Prepare <multimedia_recorder.rst#ga15d2f3416bb735a0715e1e79be226387>`__.
It is valid when the video source is YUV or RGB.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row792612051093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p771839935093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p575443576093523">

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

   <tr id="row2005987896093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

sourceId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the video source ID, which can be obtained from
SetVideoSource.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row15655614093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

fps

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the rate at which frames are captured per second.

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

SetFileSplitDuration()
----------------------

::

   int32_t OHOS::Media::Recorder::SetFileSplitDuration ([FileSplitType](multimedia_recorder.rst#ga8759c7e5a74964a584a716f4ec0b7edb) type, int64_t timestamp, uint32_t duration )

**Description:**

Manually splits a video.

This function must be called after
`Start <multimedia_recorder.rst#gac3aaa32627f0799dea65e51356b91bfb>`__.
After this function is called, the file is split based on the manual
split type. After the manual split is complete, the initial split type
is used. This function can be called again only after
**RECORDER_INFO_FILE_SPLIT_FINISHED** is reported.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1077699032093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1036458169093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p880872691093523">

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

   <tr id="row505665887093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

type

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the file split type. For details, see FileSplitType.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row98495752093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

timestamp

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the file split timestamp. This parameter is not supported
currently and can be set to -1. The recording module splits a file based
on the call time.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row19983381093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

duration

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the duration for splitting the file.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **SUCCESS** if the video is manually split; returns an error
code defined in `media_errors.h <media_errors-h.rst>`__ otherwise.

SetMaxDuration()
----------------

::

   int32_t OHOS::Media::Recorder::SetMaxDuration (int32_t duration)

**Description:**

Sets the maximum duration of a recorded file, in seconds.

This method must be called before
`Prepare <multimedia_recorder.rst#ga15d2f3416bb735a0715e1e79be226387>`__.
If the setting is valid, **RECORDER_INFO_MAX_DURATION_APPROACHING** is
reported through **OnInfo** in the
`RecorderCallback <ohos-media-recordercallback.rst>`__ class when only
one second or 10% is left to reach the allowed duration. If the
recording output file is set by calling
`SetOutputFile <multimedia_recorder.rst#ga500d2bc895852fe292d7397d8450d091>`__,
call
`SetNextOutputFile <multimedia_recorder.rst#ga8545fe87eb4bd399525e4c5fb414d7cb>`__
to set the next output file. Otherwise, the current file will be
overwritten when the allowed duration is reached.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1854934959093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1165096509093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p140226050093523">

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

   <tr id="row810209637093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

duration

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the maximum recording duration to set. If the value is 0 or a
negative number, a failure message is returned. The default duration is
60s.

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

SetMaxFileSize()
----------------

::

   int32_t OHOS::Media::Recorder::SetMaxFileSize (int64_t size)

**Description:**

Sets the maximum size of a recorded file, in bytes.

This function must be called before
`Prepare <multimedia_recorder.rst#ga15d2f3416bb735a0715e1e79be226387>`__.
If the setting is valid, **RECORDER_INFO_MAX_DURATION_APPROACHING** is
reported through **OnInfo** in the
`RecorderCallback <ohos-media-recordercallback.rst>`__ class when only
100 KB or 10% is left to reach the allowed size. If the recording output
file is set by calling
`SetOutputFile <multimedia_recorder.rst#ga500d2bc895852fe292d7397d8450d091>`__,
call
`SetNextOutputFile <multimedia_recorder.rst#ga8545fe87eb4bd399525e4c5fb414d7cb>`__
to set the next output file. Otherwise, when the allowed size is
reached, the current file will be overwritten. If **MaxDuration** is
also set by calling
`SetMaxDuration <multimedia_recorder.rst#gaf2806f0fddd17a3e59eb7c5c740470d6>`__,
**MaxDuration** or **MaxFileSize** prevails depending on which of them
is first satisfied.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1078085092093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p735037982093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p100774930093523">

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

   <tr id="row2042170376093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

size

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the maximum file size to set. If the value is 0 or a negative
number, a failure message is returned. By default, the maximum size of a
single file supported by the current file system is used as the limit.

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

SetNextOutputFile()
-------------------

::

   int32_t OHOS::Media::Recorder::SetNextOutputFile (int32_t fd)

**Description:**

Sets the FD of the next output file.

If
`SetOutputFile <multimedia_recorder.rst#ga500d2bc895852fe292d7397d8450d091>`__
is successful, call this function to set the FD of the next output file
after **RECORDER_INFO_MAX_DURATION_APPROACHING** or
**RECORDER_INFO_MAX_FILESIZE_APPROACHING** is received.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2045085927093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1329728947093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1419581590093523">

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

   <tr id="row1717288422093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

fd

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the FD of the next output file.

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

SetOutputFile()
---------------

::

   int32_t OHOS::Media::Recorder::SetOutputFile (int32_t fd)

**Description:**

Sets the file descriptor (FD) of the output file.

This function must be called before
`Prepare <multimedia_recorder.rst#ga15d2f3416bb735a0715e1e79be226387>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row503903268093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p190854775093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p250561632093523">

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

   <tr id="row1577726309093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

fd

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the FD of the file.

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

SetOutputFormat()
-----------------

::

   int32_t OHOS::Media::Recorder::SetOutputFormat ([OutputFormatType](multimedia_recorder.rst#ga3dfe2e61369bf1c081ce569e235354df) format)

**Description:**

Sets the output file format.

This function must be called before
`Prepare <multimedia_recorder.rst#ga15d2f3416bb735a0715e1e79be226387>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1121026112093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2047003265093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p428555169093523">

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

   <tr id="row1373044642093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

format

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the output file format. For details, see OutputFormatType.

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

SetOutputPath()
---------------

::

   int32_t OHOS::Media::Recorder::SetOutputPath (const string & path)

**Description:**

Sets the output file path.

This function must be called before
`Prepare <multimedia_recorder.rst#ga15d2f3416bb735a0715e1e79be226387>`__
and One of them
`SetOutputFile <multimedia_recorder.rst#ga500d2bc895852fe292d7397d8450d091>`__
must be set.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row135672177093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2128402025093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p155107033093523">

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

   <tr id="row157074724093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

path

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the output file path.

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

SetParameter()
--------------

::

   int32_t OHOS::Media::Recorder::SetParameter (int32_t sourceId, const [Format](ohos-media-format.rst) & format )

**Description:**

Sets an extended parameter for recording, for example,
**RCORDER_PRE_CACHE_DURATION**.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2104769426093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p644415179093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1753167234093523">

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

   <tr id="row1964450030093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

sourceId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the data source ID. The value -1 indicates all sources.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1669866038093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

format

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the string key and value. For details, see Format and
RCORDER_PRE_CACHE_DURATION.

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

SetRecorderCallback()
---------------------

::

   int32_t OHOS::Media::Recorder::SetRecorderCallback (const std::shared_ptr< [RecorderCallback](ohos-media-recordercallback.rst) > & callback)

**Description:**

Registers a recording listener.

This function must be called before
`Prepare <multimedia_recorder.rst#ga15d2f3416bb735a0715e1e79be226387>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row746978212093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p634360728093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p250759816093523">

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

   <tr id="row145509120093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

callback

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the recording listener to register. For details, see
RecorderCallback.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **SUCCESS** if the listener is registered; returns an error code
defined in `media_errors.h <media_errors-h.rst>`__ otherwise.

SetVideoEncoder()
-----------------

::

   int32_t OHOS::Media::Recorder::SetVideoEncoder (int32_t sourceId, [VideoCodecFormat](multimedia_mediacommon.rst#ga797e6c5e38e23e730eff5bcc41427d7e) encoder )

**Description:**

Sets a video encoder for recording.

If this function is not called, the output file does not contain the
video track. This function must be called after
`SetVideoSource <multimedia_recorder.rst#ga9e12ef9700d06c7620f9e3d7b4d844ca>`__
but before
`Prepare <multimedia_recorder.rst#ga15d2f3416bb735a0715e1e79be226387>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row967941843093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1660095126093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1561263200093523">

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

   <tr id="row11419313093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

sourceId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the video source ID, which can be obtained from
SetVideoSource.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row755126316093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

encoder

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the video encoder to set.

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

SetVideoEncodingBitRate()
-------------------------

::

   int32_t OHOS::Media::Recorder::SetVideoEncodingBitRate (int32_t sourceId, int32_t rate )

**Description:**

Sets the encoding bit rate of the video to record.

This function must be called after
`SetVideoSource <multimedia_recorder.rst#ga9e12ef9700d06c7620f9e3d7b4d844ca>`__
but before
`Prepare <multimedia_recorder.rst#ga15d2f3416bb735a0715e1e79be226387>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1664726315093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1322866001093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p612793453093523">

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

   <tr id="row2105995456093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

sourceId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the video source ID, which can be obtained from
SetVideoSource.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1693311128093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

rate

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the encoding bit rate to set.

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

SetVideoFrameRate()
-------------------

::

   int32_t OHOS::Media::Recorder::SetVideoFrameRate (int32_t sourceId, int32_t frameRate )

**Description:**

Sets the frame rate of the video to record.

This function must be called after
`SetVideoSource <multimedia_recorder.rst#ga9e12ef9700d06c7620f9e3d7b4d844ca>`__
but before
`Prepare <multimedia_recorder.rst#ga15d2f3416bb735a0715e1e79be226387>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row479381084093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1466951526093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p146326872093523">

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

   <tr id="row2124305265093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

sourceId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the video source ID, which can be obtained from
SetVideoSource.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row548510772093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

frameRate

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the frame rate to set.

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

SetVideoSize()
--------------

::

   int32_t OHOS::Media::Recorder::SetVideoSize (int32_t sourceId, int32_t width, int32_t height )

**Description:**

Sets the width and height of the video to record.

This function must be called after
`SetVideoSource <multimedia_recorder.rst#ga9e12ef9700d06c7620f9e3d7b4d844ca>`__
but before
`Prepare <multimedia_recorder.rst#ga15d2f3416bb735a0715e1e79be226387>`__.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1906190270093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1310344516093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1346001596093523">

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

   <tr id="row1462903783093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

sourceId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the video source ID, which can be obtained from
SetVideoSource.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row389006095093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

width

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the video width to set.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1307566025093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

height

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the video height to set.

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

SetVideoSource()
----------------

::

   int32_t OHOS::Media::Recorder::SetVideoSource ([VideoSourceType](multimedia_recorder.rst#gad252d27f9ce4b6ae0756bfeaa5f34490) source, int32_t & sourceId )

**Description:**

Sets a video source for recording.

If this function is not called, the output file does not contain the
video track.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1191240458093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p386918077093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p355804425093523">

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

   <tr id="row2020819680093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

source

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the video source type. For details, see VideoSourceType.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1340469496093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

sourceId

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the video source ID. The value -1 indicates an invalid ID and
the setting fails.

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

   int32_t OHOS::Media::Recorder::Start ()

**Description:**

Starts recording.

This function must be called after
`Prepare <multimedia_recorder.rst#ga15d2f3416bb735a0715e1e79be226387>`__.

**Returns:**

Returns **SUCCESS** if the recording is started; returns an error code
defined in `media_errors.h <media_errors-h.rst>`__ otherwise.

Stop()
------

::

   int32_t OHOS::Media::Recorder::Stop (bool block)

**Description:**

Stops recording.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2130562099093523">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1182862657093523">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2087437999093523">

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

   <tr id="row1146062334093523">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

block

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the stop mode. The value true indicates that the processing
stops after all caches are processed, and false indicates that the
processing stops immediately and all caches are discarded.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **SUCCESS** if the recording is stopped; returns an error code
defined in `media_errors.h <media_errors-h.rst>`__ otherwise.

**Variable Documentation**\ 
----------------------------

RCORDER_PRE_CACHE_DURATION
--------------------------

::

   const string OHOS::Media::RCORDER_PRE_CACHE_DURATION = "pre-cache-duration"

**Description:**

This constant can be used as the value of
`Format <ohos-media-format.rst>`__ in
`SetParameter <parameter.rst#ga2779b5e59d43308c51f7be38b9c98ddb>`__ to
configure the duration for storing recorded data in the cache.
