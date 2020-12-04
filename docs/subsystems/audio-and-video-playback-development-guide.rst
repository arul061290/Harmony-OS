Audio and Video Playback Development Guide
==========================================

When to Use
-----------

Audio and video playback is a process in which audio and video files or
audio and video stream data is decoded and played by using an output
device, and a playback task is managed.

Available APIs
--------------

The audio and video playback APIs are described as follows. For details
about the APIs, see the API reference document.

**Table 1** Audio and Video Playback APIs

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row85501040111310">

.. raw:: html

   <th class="cellrowborder" valign="top" width="15.959999999999999%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p755044051316">

API

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="47.77%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p1755024018131">

Function

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="36.27%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p8550134015131">

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

   <tr id="row17550440151310">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p6550440111312">

Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p65504403132">

static Player \*CreatePlayer();

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p115501540191319">

Creates a Player instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row14550164011132">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p55505406135">

Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p15550240191312">

int32_t SetSource(const Source &source);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p125502402132">

Set playback source

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row155044001318">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p255064021310">

Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p10550104014132">

int32_t Prepare();

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p155503406138">

Prepares the playback environment and buffers media data.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row165502040141313">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p3550174081313">

Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p9550144011310">

int32_t Play();

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p255094041314">

Starts playback.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row855064010130">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p3550840151318">

Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p195501409137">

bool IsPlaying()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p255114020137">

Determines whether the playback is in progress.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1555111402135">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p05511840151313">

Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p16551340151314">

int32_t Pause();

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p14551164021311">

Pauses playback.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row155511740111315">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p185515403139">

Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p19551184031318">

int32_t Stop();

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p555154041312">

Stops playback.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1255118400138">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p6551114081317">

Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p8551154015135">

int32_t Rewind(int_64 mSeconds, int32_t mode);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1255184019138">

Change the playback position.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row195511640141312">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1455164061314">

Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p5551340151313">

int32_t SetVolume(float leftVolume, float rightVolume);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p19551940181320">

Sets the volume of the audio-left and audio-right channels.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row19551144015130">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2055113408131">

Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1055124011314">

int32_t SetVideoSurface(Surface \*surface)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1355104041311">

Setting the Playback Window

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1355174010135">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p85511140161313">

Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p155114401137">

int32_t EnableSingleLooping(bool loop)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p05513403130">

Single-song repeat

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row185511040151319">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p3552124010139">

Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p6552144021318">

bool IsSingleLooping();

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p555220403134">

Determines whether to play the video cyclically.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row24941622111618">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1555214041314">

Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1655294011317">

int32_t GetCurrentTime(int64_t &time) const;

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p255234031315">

Obtains the current playback duration.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row655224015139">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p165520406137">

Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p7552164071320">

int32_t GetDuration(int64_t &duration) const;

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p17552640141312">

Obtains the total playback duration.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row11552194019131">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p955214013132">

Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p655234018131">

int32_t GetVideoWidth(int32_t &videoWidth);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p12552174081314">

Obtains the width of a video source.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row8552164013134">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p125525404136">

Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p13552114011316">

int32_t GetVideoHeight(int32_t &videoHeight);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p14552134011138">

Obtains the height of a video source.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row6552340181312">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1155244017138">

Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1955374031313">

int32_t Reset();

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1553124061317">

Restores the player to the initial state.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row6553134021311">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1655314021316">

Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p13553194018132">

int32_t Release();

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p455354018139">

Releasing Player Resources

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row25531940151318">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p95531440191318">

Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1955317400131">

void SetPlayerCallback(const std::shared_ptr<PlayerCallback> &cb);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p135530402139">

Sets the playback callback function.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row26841936205916">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p155531940171317">

Source

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1955314012137">

Source(const std::string& uri);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p755314031315">

Creating a Source Instance Based on the URI

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1839749195917">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p13553040181316">

Source

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p125538401138">

Source(const std::string &uri, const std::map<std::string, std::string>
&header);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p35533406130">

Creating a Source Instance Based on the URI and URI Header

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row16713165319598">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p195531740141316">

Source

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p655310403132">

Source(const std::shared_ptr<StreamSource> &stream, const Format
&formats);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p05536401138">

Creating a Source Instance Based on Flows

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row39004563590">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p15531340191312">

Source

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p13553174091318">

SourceType GetSourceType() const;

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1455354016136">

Obtains the source type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row15429101008">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1655434018139">

Source

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p7554154013137">

const std::string &GetSourceUri() const;

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1855414071310">

Obtains the audio and video URIs.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row12357142103">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1554124015132">

Source

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p12554134016134">

const std::map<std::string, std::string> &GetSourceHeader() const;

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p3554124091318">

Obtains the audio and video URI headers.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row17477411011">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p105540409134">

Source

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1355434014138">

const std::shared_ptr<StreamSource> &GetSourceStream() const;

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p455415408132">

Obtaining Audio and Video Streams

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row19135971706">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p257064871110">

Source

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p151191016151214">

const Format &GetSourceStreamFormat() const;

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p14257126131210">

Obtains the audio and video stream formats.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1543179104">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p255412409135">

Format

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p655454001314">

bool PutIntValue(const std::string &key, int32_t value);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p205661711619">

Sets the metadata of the integer type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row695314111204">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p655454019138">

Format

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1554840111319">

bool PutLongValue(const std::string &key, int64_t value);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p230317337163">

Sets the metadata of the long integer type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row3518133213019">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1855434031312">

Format

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1555484014139">

bool PutFloatValue(const std::string &key, float value);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p12391147111614">

Sets the metadata of the single-precision floating-point type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row176434351308">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p655534031317">

Format

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p5555640111320">

bool PutDoubleValue(const std::string &key, double value);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p185881525191711">

Sets the metadata of the double-precision floating-point type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row9476163810013">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p3555154017133">

Format

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p3555124015133">

bool PutStringValue(const std::string &key, const std::string &value);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p16021743131719">

Sets the metadata of the character string type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row879515406015">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p15551540181313">

Format

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p19555164041313">

bool GetIntValue(const std::string &key, int32_t &value) const;

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p435725714171">

Obtains the metadata value of the integer type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row462919431104">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1655544021318">

Format

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p0555194031314">

bool GetLongValue(const std::string &key, int64_t &value) const;

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p7330132141811">

Obtains the metadata value of the long integer type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1797513451904">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1655624011319">

Format

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p155567401134">

bool GetFloatValue(const std::string &key, float &value) const;

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p080203817189">

Obtains the metadata value of the single-precision floating-point type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row012319491603">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p855694013132">

Format

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p10556124015132">

bool GetDoubleValue(const std::string &key, double &value) const;

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p116117558189">

Obtains the metadata value of the double-precision floating-point type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row22531651901">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1855604081314">

Format

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p9556840171310">

bool GetStringValue(const std::string &key, std::string &value) const;

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p6495161451914">

Obtains the metadata value of the character string type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row552743019">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p165563405133">

Format

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p4556134061315">

const std::map<std::string, FormatData \*> &GetFormatMap() const;

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p3379195115711">

Obtain the Map table of the format.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row127651251115">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p16556240111315">

Format

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p195561240111317">

bool CopyFrom(const Format &format);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p185953195717">

Copies all content from a format instance.

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

When the input source is an audio or video stream, the playback progress
cannot be controlled and the file duration cannot be obtained.

How to Develop
--------------

1. Implement the PlayerCallback callback function for event processing.

   ::

      class TestPlayerCallback : public PlayerCallback{ 
          void OnPlayBackComplete() override 
          { 
      // The implementation code is used to process the event that the file playback is complete.
          } 
          void OnError(int32_t errorType, int32_t errorCode) override 
          { 
      // Implement the code processing error event.
          } 
          void OnInfo(int type, int extra) override 
          { 
      //Implement the code to process common events.
          } 
          void OnRewindToComplete() override 
          { 
      //Implement the event that the code processing progress control is complete.
          } 
      };

2. Create a player instance, set the playback source, and start
   playback.

   ::

      Player *player = Player::CreatePlayer(); 
      std::shared_ptr<PlayerCallback> callback = std::make_shared<TestPlayerCallback>(); 
      player->SetPlayerCallback(callback);// Set player callback.
      std::string uri(filePath);// filePath is the local file path.
      Source source(uri);//Save the URI to the source instance.
      player->SetSource(source);//Set the source to the player.
      player->SetVideoSurface(surface);//Set the playback window.
      player->Prepare(); // Prepare for the playback.
      player->Play(); //Starts playback.

3. Perform playback control based on the scenario.

   ::

      player->SetVolume(lvolume, rvolume);//Set the left and right sound channels.
      player->EnableSingleLooping(true);// Set cyclic playback.
      player->Pause(); //Pause.
      player->Play(); //Continue the playback.

4. Release resources after the playback task is complete.

   ::

      player->Stop(); //Stop the playback.
      player->Release(); // Release resources.
