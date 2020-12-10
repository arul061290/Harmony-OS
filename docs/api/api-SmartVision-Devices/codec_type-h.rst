codec_type.h
============

**Overview**\ 
--------------

**Related Modules:**

`Codec <codec.rst>`__

**Description:**

Declares custom data types used in API declarations for the Codec
module, including the codec types, audio and video parameters, input and
output data, and callbacks.

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

   <tr id="row1960046574084828">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2016152428084828">

Data Structure Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p320254296084828">

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

   <tr id="row1507323575084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p959172643084828">

Param

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2135408201084828">

Describes the dynamic parameter structure, which is mainly used by
CodecCreate and CodecSetParameter.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1575246798084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2037143404084828">

BufferHandle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1223091105084828">

Defines the buffer handle type. The virtual address of a handle maps to
its physical address.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row529450492084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1668235956084828">

CodecBufferInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p815791496084828">

Describes buffer information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row492461023084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p416751397084828">

InputInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1030849217084828">

Describes input information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row734818250084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2068273710084828">

OutputInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p576393773084828">

Describes output information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1044254700084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1117144018084828">

ResizableArray

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1946005268084828">

Defines a variable-length queue.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1156818827084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1994543800084828">

Alginment

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p478497806084828">

Defines the alignment.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1962880116084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p256269643084828">

Rect

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p623223572084828">

Defines a rectangle.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row540426967084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p273022189084828">

Capbility

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1482088597084828">

Defines the codec capability.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1557846678084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p172338824084828">

CodecCallback

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1116375387084828">

Defines callbacks and their parameters.

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

Macros
------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row197878477084828">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p638249996084828">

Macro Name and Value

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p314751089084828">

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

   <tr id="row1565602250084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1933748438084828">

ELEMENT_MAX_LEN 50

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1086700054084828">

Indicates the maximum number of reserved parameters in the array.

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

Typedefs
--------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row341673077084828">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1026937632084828">

Typedef Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p565447302084828">

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

   <tr id="row2029720066084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p275951800084828">

CODEC_HANDLETYPE

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p844129728084828">

typedef void \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1234196025084828">

Defines the pointer to the codec handle, which is the context
information for function calls.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1492830448084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1140046084084828">

ValueType

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p348147151084828">

typedef void \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p88834049084828">

Defines the pointer to the type of the dynamic parameter value.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1979929749084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1638176761084828">

BufferHandle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2080957391084828">

typedef struct BufferHandle

.. raw:: html

   </p>

.. raw:: html

   <p id="p1134054336084828">

Defines the buffer handle type. The virtual address of a handle maps to
its physical address.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row136474467084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1465066640084828">

BufferType

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1643176806084828">

typedef enum BufferType

.. raw:: html

   </p>

.. raw:: html

   <p id="p383458095084828">

Enumerates buffer types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1619920573084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1125196664084828">

OutputInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1147926780084828">

typedef struct OutputInfo

.. raw:: html

   </p>

.. raw:: html

   <p id="p931230207084828">

Describes output information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row613779929084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1746544163084828">

AllocateBufferMode

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p134804684084828">

typedef enum AllocateBufferMode

.. raw:: html

   </p>

.. raw:: html

   <p id="p2105226579084828">

Enumerates allocation modes of input and output buffers.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row88912696084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p512745999084828">

CapsMask

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p661530515084828">

typedef enum CapsMask

.. raw:: html

   </p>

.. raw:: html

   <p id="p641914122084828">

Enumerates playback capabilities.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1795589246084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1784177652084828">

CodecCapbility

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1623346095084828">

typedef struct Capbility

.. raw:: html

   </p>

.. raw:: html

   <p id="p246137123084828">

Defines the codec capability.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row282520749084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p647005390084828">

UINTPTR

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p519963950084828">

typedef uintptr_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p405786549084828">

Redefines the unsigned pointer type, which is used for pointer
conversion.

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

   <tr id="row1723425185084828">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1364626928084828">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p247993325084828">

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

   <tr id="row140371928084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p212602410084828">

CodecType { VIDEO_DECODER, VIDEO_ENCODER, AUDIO_DECODER, AUDIO_ENCODER,
INVALID_TYPE }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p175896515084828">

Enumerates codec types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1605822419084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p280070827084828">

ParamKey { KEY_MIMETYPE = 0x01, KEY_BUFFERSIZE, KEY_LEFT_STREAM_FRAMES,
KEY_CODEC_TYPE, KEY_DIRECTION_TYPE, KEY_BITRATE = 0x500, KEY_WIDTH =
0x1000, KEY_HEIGHT, KEY_STRIDE, KEY_VIDEO_FIELD, KEY_PIXEL_FORMAT,
KEY_VIDEO_RC_MODE, KEY_VIDEO_GOP_MODE, KEY_VIDEO_PIC_SIZE,
KEY_VIDEO_PROFILE, KEY_VIDEO_FRAME_RATE, KEY_SAMPLE_RATE = 0x1500,
KEY_AUDIO_PROFILE, KEY_CHANNEL_COUNT, KEY_BITWITH, KEY_SOUND_MODE,
KEY_POINT_NUM_PER_FRAME, KEY_DEVICE_ID }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2078294378084828">

Enumerates indexes of parameter types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row180755901084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1237903691084828">

VenCodeRcMode { VENCOD_RC_CBR = 0, VENCOD_RC_VBR, VENCOD_RC_AVBR,
VENCOD_RC_QVBR, VENCOD_RC_CVBR, VENCOD_RC_QPMAP, VENCOD_RC_FIXQP }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p937983449084828">

Enumerates control modes of the channel encoding rate.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1570166870084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p625185968084828">

PicSize { Resolution_CIF, Resolution_360P, Resolution_D1_PAL,
Resolution_D1_NTSC, Resolution_720P, Resolution_1080P,
Resolution_INVALID }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1772718533084828">

Enumerates resolutions.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1767642137084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p404857669084828">

VenCodeGopMode { VENCOD_GOPMODE_NORMALP = 0, VENCOD_GOPMODE_DUALP = 1,
VENCOD_GOPMODE_SMARTP = 2, VENCOD_GOPMODE_ADVSMARTP = 3,
VENCOD_GOPMODE_BIPREDB = 4, VENCOD_GOPMODE_LOWDELAYB = 5,
VENCOD_GOPMODE_INVALID }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p897799670084828">

Enumerates types of group of pictures (GOP).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row548895589084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1051765026084828">

VideoField { VID_FIELD_TOP = 0x1, VID_FIELD_BOTTOM = 0x2,
VID_FIELD_INTERLACED = 0x3, VID_FIELD_FRAME = 0x4, VID_FIELD_INVALID }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1082574900084828">

Enumerates video frame fields.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1514169514084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p357738938084828">

PixelFormat { YVU_SEMIPLANAR_420 = 0, YVU_SEMIPLANAR_420_TILE,
PIX_FORMAT_INVALID }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p733135871084828">

Enumerates pixel formats.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1208501526084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p924100610084828">

AudioSoundMode { AUD_SOUND_MODE_MONO = 0, AUD_SOUND_MODE_STEREO = 1,
AUD_SOUND_MODE_INVALID }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1224989200084828">

Enumerates audio channel modes.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1086290988084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p973405699084828">

AudioSampleRate { AUD_SAMPLE_RATE_8000 = 8000, AUD_SAMPLE_RATE_12000 =
12000, AUD_SAMPLE_RATE_11025 = 11025, AUD_SAMPLE_RATE_16000 = 16000,
AUD_SAMPLE_RATE_22050 = 22050, AUD_SAMPLE_RATE_24000 = 24000,
AUD_SAMPLE_RATE_32000 = 32000, AUD_SAMPLE_RATE_44100 = 44100,
AUD_SAMPLE_RATE_48000 = 48000, AUD_SAMPLE_RATE_64000 = 64000,
AUD_SAMPLE_RATE_96000 = 96000, AUD_SAMPLE_RATE_INVALID }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p846866403084828">

Enumerates audio sampling rates.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row354208705084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1127681718084828">

AudioBitRate { AUD_AAC_BPS_8K = 8000, AUD_AAC_BPS_16K = 16000,
AUD_AAC_BPS_22K = 22000, AUD_AAC_BPS_24K = 24000, AUD_AAC_BPS_32K =
32000, AUD_AAC_BPS_48K = 48000, AUD_AAC_BPS_64K = 64000, AUD_AAC_BPS_96K
= 96000, AUD_AAC_BPS_128K = 128000, AUD_AAC_BPS_256K = 256000,
AUD_AAC_BPS_320K = 320000 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1563716701084828">

Enumerates audio bit rates.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1577287092084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1683029431084828">

StreamFlagType { STREAM_FLAG_KEYFRAME = 1,
STREAM_FLAG_CODEC_SPECIFIC_INF = 2, STREAM_FLAG_EOS = 4,
STREAM_FLAG_PART_OF_FRAME = 8, STREAM_FLAG_END_OF_FRAME = 16 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p340411416084828">

Enumerates stream flags.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1919450765084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p842862263084828">

BufferType { BUFFER_TYPE_VIRTUAL = 0, BUFFER_TYPE_FD, BUFFER_TYPE_HANDLE
}

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1514920033084828">

Enumerates buffer types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1169831936084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p233498868084828">

AvCodecMime { MEDIA_MIMETYPE_IMAGE_JPEG = 0, MEDIA_MIMETYPE_VIDEO_AVC,
MEDIA_MIMETYPE_VIDEO_HEVC, MEDIA_MIMETYPE_AUDIO_AAC,
MEDIA_MIMETYPE_INVALID }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1953687794084828">

Enumerates MIME types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1579357354084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p860864683084828">

Profile { INVALID_PROFILE = 0, AAC_LC_PROFILE = 0x1000,
AAC_MAIN_PROFILE, AAC_HE_V1_PROFILE, AAC_HE_V2_PROFILE, AAC_LD_PROFILE,
AAC_ELD_PROFILE, AVC_BASELINE_PROFILE = 0x2000, AVC_MAIN_PROFILE,
AVC_HIGH_PROFILE, HEVC_MAIN_PROFILE = 0x3000, HEVC_MAIN_10_PROFILE }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1872553901084828">

Enumerates codec profiles.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row753920041084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p197613531084828">

Level { INVALID_LEVEL = 0, AVC_LEVEL_1 = 0x1000, HEVC_LEVEL_MAIN_1 =
0x2000, HEVC_LEVEL_MAIN_2 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1225904752084828">

Enumerates codec levels.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row366970145084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2078544098084828">

AllocateBufferMode { ALLOCATE_INPUT_BUFFER_CODEC = 0x1,
ALLOCATE_INPUT_BUFFER_USER = 0x2, ALLOCATE_OUTPUT_BUFFER_CODEC = 0x4,
ALLOCATE_OUTPUT_BUFFER_USER = 0x8 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1436062262084828">

Enumerates allocation modes of input and output buffers.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2029179647084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1575698171084828">

CapsMask { ADAPTIVE_PLAYBACK = 0x1, SECURE_PLAYBACK = 0x2 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p635958155084828">

Enumerates playback capabilities.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1309274616084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1976349612084828">

EventType { EventError, EventFlushCompelte, EventStopCompelte,
EventOutFormatChanged, EventMax = 0x1FFFFFFF }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p315226659084828">

Enumerates event types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1292577953084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p834540765084828">

DirectionType { INPUT_TYPE, OUTPUT_TYPE, ALL_TYPE }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p361460391084828">

Enumerates input and output types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1591436891084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2074968568084828">

BufferMode { INTERNAL, EXTERNAL }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p947308506084828">

Enumerates allocation types.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1002400018084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p366437149084828">

{ CODEC_ERR_STREAM_BUF_FULL = 100, CODEC_ERR_FRAME_BUF_EMPTY,
CODEC_RECEIVE_EOS, CODEC_ERR_INVALID_OP }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1419488241084828">

Enumerates codec error types.

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
