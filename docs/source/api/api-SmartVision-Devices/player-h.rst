player.h
========

**Overview**\ 
--------------

**Related Modules:**

`MultiMedia_Player <multimedia_player.md>`__

**Description:**

Declares the **Player** class, which is used to implement player-related
operations.

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

   <tr id="row970159725093527">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2032343646093527">

Data Structure Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1856801493093527">

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

   <tr id="row1042868543093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1600804126093527">

OHOS::Media::PlayerCallback

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p827629751093527">

Provides listeners for events and exception notifications that occur
during media playback.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row189239062093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2113895889093527">

OHOS::Media::Player

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p570749034093527">

Provides functions for playing online movies, offline movies, and
streams, for example, playing local movies and advanced audio coding
(AAC) streams.

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

   <tr id="row548624964093527">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p849654474093527">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p653107091093527">

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

   <tr id="row1408165417093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1783960043093527">

OHOS::Media::PlayerSeekMode : int32_t {
OHOS::Media::PLAYER_SEEK_PREVIOUS_SYNC = 0,
OHOS::Media::PLAYER_SEEK_NEXT_SYNC,
OHOS::Media::PLAYER_SEEK_CLOSEST_SYNC, OHOS::Media::PLAYER_SEEK_CLOSEST,
OHOS::Media::PLAYER_SEEK_FRAME_INDEX }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1222646729093527">

Enumerates player seek modes. You can move the current playback position
of the media to a given time position using the specified mode.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row529816840093527">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p595758775093527">

OHOS::Media::PlayerStates : uint32_t { OHOS::Media::PLAYER_STATE_ERROR =
0, OHOS::Media::PLAYER_IDLE = 1 << 0, OHOS::Media::PLAYER_INITIALIZED =
1 << 1, OHOS::Media::PLAYER_PREPARING = 1 << 2,
OHOS::Media::PLAYER_PREPARED = 1 << 3, OHOS::Media::PLAYER_STARTED = 1
<< 4, OHOS::Media::PLAYER_PAUSED = 1 << 5, OHOS::Media::PLAYER_STOPPED =
1 << 6, OHOS::Media::PLAYER_PLAYBACK_COMPLETE = 1 << 7 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1684662132093527">

Enumerates player states.

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
