Audio and Video Recording Development Guide
===========================================

When to Use
-----------

Audio and video recording is used to record audio and video and
encapsulate output files based on the configured encoding format,
sampling rate, and bit rate.

Available APIs
--------------

The audio and video recording APIs are as follows. For details about the
APIs, see the interface document.

**Table 1** Audio and Video Recording APIs

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row4419501537">

.. raw:: html

   <th class="cellrowborder" valign="top" width="7.5200000000000005%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p531591918714">

API

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="53.06999999999999%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p1325118401591">

Function

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="39.410000000000004%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p1251184013912">

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

   <tr id="row34145016535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p113157191379">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p425115401998">

static Recorder \*CreateRecorder()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p225104017920">

Creates a Recorder instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1746172917474">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1712917411310">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p925111401895">

int32_t SetVideoSource(VideoSourceType source, int32_t &sourceId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p152511640691">

Setting a Video Source for Recording

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row10992232154714">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p8129156111319">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1776173711119">

int32_t SetVideoEncoder(int32_t sourceId, VideoCodecFormat encoder)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p127623791116">

Sets the type of the video encoder for recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row933265824817">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p944717831310">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p6769371110">

int32_t SetVideoSize(int32_t sourceId, int32_t width, int32_t height)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p17761137181115">

Sets the width and height of the recorded video.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row124766591190">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p18795111319132">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p476113791113">

int32_t SetVideoFrameRate(int32_t sourceId, int32_t frameRate)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p107613711114">

Sets the frame rate of the video to be recorded.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row0260140101">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p149767151136">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1076203717112">

int32_t SetVideoEncodingBitRate(int32_t sourceId, int32_t rate)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p0761637141116">

Sets the encoding bit rate of the recorded video.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row22024106107">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p177997175138">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p5761737171112">

int32_t SetCaptureRate(int32_t sourceId, double fps)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1761737151111">

Sets the frame capture rate of video frames.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row82261213191012">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p94271121181318">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1129110237225">

std::shared_ptr<OHOS::Surface> GetSurface(int32_t sourceId);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1876163710115">

Obtains the surface of the corresponding input source.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1366261518102">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p13158202312139">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p4761377117">

int32_t SetAudioSource(AudioSourceType source, int32_t &sourceId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p5765377117">

Set the audio source for recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row7142161861017">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2897162514139">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p8766372113">

int32_t SetAudioEncoder(int32_t sourceId, AudioCodecFormat encoder)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p127693731115">

Sets the type of the audio encoder for recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2053832071012">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p952618270132">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p976937141112">

int32_t SetAudioSampleRate(int32_t sourceId, int32_t rate)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1476183781110">

Sets the audio sampling rate for recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row55394243108">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p677717304137">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p47703781114">

int32_t SetAudioChannels(int32_t sourceId, int32_t num)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p16772037121111">

Sets the number of audio channels to be recorded.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row191791427121015">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1759610327139">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p37723781118">

int32_t SetAudioEncodingBitRate(int32_t sourceId, int32_t bitRate)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p17771378113">

Sets the encoding bit rate of the recorded audio.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row83478305107">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p16968193391311">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1536305312114">

int32_t SetMaxDuration(int32_t duration)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p93634532118">

Sets the maximum duration of a recorded file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row592711339103">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p947593614139">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1436314531119">

int32_t SetOutputFormat(OutputFormatType format)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1936315331119">

Sets the output file format.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row15219377106">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p552463917132">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p33631253121116">

int32_t SetOutputFile(int32_t fd)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p336335351111">

Sets the FD of the output file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row18755438101013">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p121613438137">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p14363175317114">

int32_t SetNextOutputFile(int32_t fd);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p236375361119">

Sets the fd of the next output file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row14480241101010">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p07641457131">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2363145317112">

int32_t SetMaxFileSize(int64_t size)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p43646539114">

Sets the maximum file size of a recording session.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row835564418101">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2104174817136">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p15364195315118">

int32_t SetRecorderCallback(const std::shared_ptr<RecorderCallback>
&callback)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1636412538119">

Registers the recording listener callback function.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row780144661014">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p098351816145">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p173641153151110">

int32_t Prepare()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p636495341115">

Prepare for recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row11537184971012">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p12815320121418">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p53641053151113">

int32_t Start()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p53642536114">

Starts recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row158225271018">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p132682201410">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p936485351112">

int32_t Pause()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p183641253141110">

Pauses recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row15938254131016">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p12615824111414">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p123641153191115">

int32_t Resume()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p0364195331116">

Resumes recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row193212569102">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p15373202761415">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p63641653101116">

int32_t Stop(bool block)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1364053171112">

Stops recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1392185911103">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p199881728181420">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p143641539114">

int32_t Reset();

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p20364353131115">

Resets recording.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row816014171116">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p193259303141">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p183649535111">

int32_t Release()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1036420534111">

Releasing Recording Resources

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row115981253112">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1466416312142">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p17364053171110">

int32_t SetFileSplitDuration(FileSplitType type, int64_t timestamp,
uint32_t duration)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p8364205361117">

Setting Split Recording

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1677310915111">

.. raw:: html

   <td class="cellrowborder" valign="top" width="7.5200000000000005%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1028316364149">

Recorder

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="53.06999999999999%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1936411531111">

int32_t SetParameter(int32_t sourceId, const Format &format)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="39.410000000000004%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p13657530118">

Sets the extended recording parameters.

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

Limitations and Constraints
---------------------------

None

How to Develop
--------------

1. This API is used to create a Recorder instance.

   ::

      Recorder *recorder = Recorder::CreateRecorder();

2. Sets Recorder parameters, including the audio and video source
   information, audio and video encoding format, sampling rate, bit
   rate, and video width and height.

   ::

      int32_t sampleRate = 48000; 
      int32_t channelCount = 1;
      AudioCodecFormat audioFormat = AAC_LC;
      AudioSourceType inputSource = AUDIO_MIC;
      int32_t audioEncodingBitRate = sampleRate;
      VideoSourceType source = VIDEO_SOURCE_SURFACE_ES;
      int32_t frameRate = 30;
      float fps = 30;
      int32_t rate = 4096;
      int32_t sourceId = 0;
      int32_t audioSourceId = 0;
      int32_t width = 1920;
      int32_t height = 1080;
      VideoCodecFormat encoder = H264;
      recorder->SetVideoSource(source, sourceId); // Set the video source and obtain the sourceId.
      recorder->SetVideoEncoder(sourceId, encoder); // Set the video encoding format.
      recorder->SetVideoSize(sourceId, width, height); // Set the video width and height.
      recorder->SetVideoFrameRate(sourceId, frameRate); // Set the video frame rate.
      recorder->SetVideoEncodingBitRate(sourceId, rate); //: Sets the video encoding bit rate.
      recorder->SetCaptureRate(sourceId, frameRate); //: Sets the frame capture rate of video frames.
      recorder->SetAudioSource(inputSource, audioSourceId); // Set the audio source and obtain audioSourceId.
      recorder->SetAudioEncoder(audioSourceId, audioFormat); // Set the audio encoding format.
      recorder->SetAudioSampleRate(audioSourceId, sampleRate); // Set the audio sampling rate.
      recorder->SetAudioChannels(audioSourceId, channelCount); // Set the number of audio channels.
      recorder->SetAudioEncodingBitRate(audioSourceId, audioEncodingBitRate); // Set the audio encoding bit rate.

3. Prepare for the recording. The Recorder prepares for the recording.

   ::

      recorder->Prepare(); // Prepares for recording.

4. The Recorder starts recording based on the configured audio and video
   sources.

   ::

      recorder->Start(); // Start recording.

5. Stop recording and release resources.

   ::

      recorder->Stop(); // Stop recording.
      recorder->Release(); // Release recording resources.
