format_interface.h
==================

**Overview**\ 
--------------

**Related Modules:**

`Format <format.md>`__

**Description:**

Declares format-related APIs.

For example, you use the functions provided in this file to define
custom data types and to initialize, create, destroy the muxer and
demuxer, and set their parameters. Also, you can read demuxer data
frames, select demuxer tracks, add muxer tracks, and write data frames
into a container.

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

   <tr id="row1538455717093525">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1242387238093525">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1045218669093525">

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

   <tr id="row263925225093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p135038706093525">

FormatInit (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p801704731093525">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1311348807093525">

Initializes the format.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row136008339093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p406548937093525">

FormatDeInit (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2025731462093525">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1744658667093525">

Deinitializes the format.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1139696505093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1484244721093525">

FormatDemuxerCreate (const FormatSource \*source, void \**handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2131066849093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p894103992093525">

Creates a demuxer component and returns its context handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1340019463093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1332230191093525">

FormatDemuxerSetParameter (const void *handle, int32_t trackId, const
ParameterItem*\ metaData, int32_t metaDataCnt)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p669796469093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p630887961093525">

Sets demuxer attributes.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1041317145093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1496463729093525">

FormatDemuxerGetParameter (const void *handle, int32_t trackId,
ParameterItem*\ metaData)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1631422337093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1784435051093525">

Obtains demuxer attributes.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1333595594093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1789398042093525">

FormatDemuxerSetCallBack (void *handle, const FormatCallback*\ callBack)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1242005970093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2099380810093525">

Sets a callback for the demuxer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1968765507093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1390730323093525">

FormatDemuxerSetBufferConfig (void *handle, const
FormatBufferSetting*\ setting)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1298977598093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p310316681093525">

Sets buffer information for the demuxer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row686836975093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p224933785093525">

FormatDemuxerGetBufferConfig (const void *handle,
FormatBufferSetting*\ setting)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2054962615093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1037553586093525">

Obtains the buffer information of the demuxer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row783075667093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p435615739093525">

FormatDemuxerPrepare (void \*handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1811188556093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p808165404093525">

Makes preparations for the demuxer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2044150739093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p578784752093525">

FormatDemuxerGetFileInfo (void *handle, FileInfo*\ info)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p67685368093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1429334524093525">

Obtains the attributes of a media file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row846509491093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1013272868093525">

FormatDemuxerSelectTrack (const void \*handle, int32_t programId,
int32_t trackId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1716686996093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2130643253093525">

Selects a specified media track.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2106581450093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p636204752093525">

FormatDemuxerUnselectTrack (const void \*handle, int32_t programId,
int32_t trackId)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p459149720093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p12979640093525">

Unselects a specified media track from which the demuxer reads data
frames.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1442754661093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p160821416093525">

FormatDemuxerStart (void \*handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2075535456093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1434346919093525">

Starts the demuxer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1469784849093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1248365814093525">

FormatDemuxerGetSelectedTrack (const void *handle, int32_t*\ programId,
int32_t trackId[], int32_t \*nums)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1250513482093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1118682269093525">

Obtains the ID of the media track selected by the demuxer for output.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row282486069093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1948155308093525">

FormatDemuxerReadFrame (const void *handle, FormatFrame*\ frame, int32_t
timeOutMs)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1364772757093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1949527375093525">

Reads data frames.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row216778346093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1775033422093525">

FormatDemuxerFreeFrame (void *handle, FormatFrame*\ frame)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p942919539093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1237371044093525">

Frees data frames.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1327297166093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2086028677093525">

FormatDemuxerSeek (const void \*handle, int32_t streamIndex, int64_t
timeStampUs, FormatSeekMode mode)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1891025701093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p870706021093525">

Seeks for a specified position for the demuxer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1959908101093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1498624057093525">

FormatDemuxerStop (void \*handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2128677001093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p167453307093525">

Stops the demuxer from working.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row446141999093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p775663381093525">

FormatDemuxerDestory (void \*handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p707157808093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1501171793093525">

Destroys demuxer resources.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row503605676093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1441820349093525">

FormatMuxerCreate (void \**handle, FormatOutputConfig \*outputConfig)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p641496722093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p520862712093525">

Creates a muxer and returns its context handle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1283754400093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p749722125093525">

FormatMuxerDestory (const void \*handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p653976905093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1974355959093525">

Destroys a muxer and release its resources created by calling
FormatMuxerCreate.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row942239204093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p544008354093525">

FormatMuxerAddTrack (void *handle, const TrackSource*\ trackSource)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2080637403093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2064277535093525">

Adds a media track source for the muxer. For details about track
sources, see TrackSource.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2021749016093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1100523117093525">

FormatMuxerSetCallBack (void *handle, const FormatCallback*\ callBack)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p102646293093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p648745064093525">

Sets a callback for the muxer. For details about the callback, see
FormatCallback.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1173189058093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p539694840093525">

FormatMuxerSetOrientation (void \*handle, int degrees)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1552017061093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1991023384093525">

Sets the orientation of the video track for the muxer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1563625249093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p379115392093525">

FormatMuxerSetLocation (const void \*handle, int latitude, int
longitude)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1244292331093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1077359986093525">

Sets the geographical information for the output file of the muxer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row236020162093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p410001718093525">

FormatMuxerSetMaxFileSize (void \*handle, int64_t bytes)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p730765350093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p858959435093525">

Sets the maximum size (in bytes) for the output file of the muxer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1736560375093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2067206325093525">

FormatMuxerSetMaxFileDuration (void \*handle, int64_t durationUs)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1580650549093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1782647218093525">

Sets the maximum duration (in seconds) for the output file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row107240351093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1416329148093525">

FormatMuxerSetFileSplitDuration (const void \*handle, ManualSplitType
type, int64_t timestampUs, uint32_t durationUs)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1442376136093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p859237519093525">

Manually splits a file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1531743155093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1018559465093525">

FormatMuxerStart (void \*handle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1979208818093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2140955923093525">

Starts the muxer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row429198830093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p914879852093525">

FormatMuxerWriteFrame (const void *handle, const
FormatFrame*\ frameData)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1925850954093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2112153899093525">

Writes data frames into the muxer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2130525149093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1882564330093525">

FormatMuxerSetNextOutputFile (const void \*handle, int32_t fd)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1021835675093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p622054733093525">

Sets the descriptor for the next output file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1019192794093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1310665170093525">

FormatMuxerStop (const void \*handle, bool block)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p508182387093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1527667267093525">

Stops the muxer that was started by calling FormatMuxerStart.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row339413666093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1875493085093525">

FormatMuxerSetParameter (void *handle, int32_t trackId, const
ParameterItem*\ item, int32_t itemNum)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1025648227093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1500975867093525">

Sets muxer attributes.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1474673960093525">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1027363824093525">

FormatMuxerGetParameter (void *handle, int32_t trackId,
ParameterItem*\ item, int32_t itemNum)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1628994625093525">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p682568633093525">

Obtains muxer attributes.

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
