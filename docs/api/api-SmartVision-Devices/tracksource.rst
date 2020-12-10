TrackSource
===========

**Overview**\ 
--------------

**Related Modules:**

`Format <format.rst>`__

**Description:**

Defines information about the muxer source.

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

   <tr id="row1709016909084842">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1339020229084842">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1190343295084842">

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

   <tr id="row241190412084842">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p975374521084842">

trackSourceType

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p844334696084842">

TrackSourceType

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1510191155084842">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2099702031084842">

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p367802265084842">

union {

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row903277367084842">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

  

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p982151517084842">

VideoTrackSourceInfo videoInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2120553217084842">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

  

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1035570793084842">

AudioTrackSourceInfo audioInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row965636496084842">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

  

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1003010887084842">

DataTrackSourceInfo dataInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1952682130084842">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1401404177084842">

trackSourceInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p389095578084842">

}

.. raw:: html

   </p>

.. raw:: html

   <p id="p16172861084842">

Defines detailed information about different types of stream sources.

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

audioInfo
---------

::

   [AudioTrackSourceInfo](audiotracksourceinfo.rst) TrackSource::audioInfo

**Description:**

Audio stream. For details, see
`AudioTrackSourceInfo <audiotracksourceinfo.rst>`__.

dataInfo
--------

::

   [DataTrackSourceInfo](datatracksourceinfo.rst) TrackSource::dataInfo

**Description:**

Data stream. For details, see
`DataTrackSourceInfo <datatracksourceinfo.rst>`__

trackSourceType
---------------

::

   [TrackSourceType](format.rst#ga953bc46f95d7b2d8866838d792f8f6aa) TrackSource::trackSourceType

**Description:**

Stream source type. For details, see
`TrackSourceType <format.rst#ga953bc46f95d7b2d8866838d792f8f6aa>`__

videoInfo
---------

::

   [VideoTrackSourceInfo](videotracksourceinfo.rst) TrackSource::videoInfo

**Description:**

Video stream. For details, see
`VideoTrackSourceInfo <videotracksourceinfo.rst>`__.
