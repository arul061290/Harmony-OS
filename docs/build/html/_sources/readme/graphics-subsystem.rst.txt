Graphics Subsystem
==================

Overview
--------

The graphics subsystem mainly includes user interface (UI) components,
layout, animator, font, input event, window management, rendering and
drawing modules. It builds an application framework based on the LiteOS
to develop applications on Internet of Things (IoT) devices with small
hardware resources.

Module description:

-  Components: provides application components, including the UIView,
   UIViewGoup, UIButton, UILabel, UILabelButton, UIList, and UISlider.
-  Layout: lays out components, including Flexlayout, GridLayout, and
   ListLayout.
-  Animator: defines functions for customizing animators.
-  Fonts: defines functions related to fonts.
-  Event: processes basic events, including click, press, drag, and long
   press.
-  Tasks: manages tasks.
-  Input: processes input events.
-  Display: processes display events.
-  Render: renders and draws components.
-  Draw2d: draws lines, rectangles, circles, arcs, images, and texts,
   and interconnects with software rendering and hardware acceleration.
-  Surface: applies for and releases shared memory.
-  Window: manages windows, including creating, showing, hiding a
   window, and combining windows.
-  Adapter: interconnects with underlying interfaces of the adaptation
   layer.

Directory Structure
-------------------

**Table 1** Directory structure of source code for the graphics
subsystem

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row7977610131417">

.. raw:: html

   <th class="cellrowborder" valign="top" width="17.7%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p18792459121314">

Directory

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="82.3%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p77921459191317">

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

   <tr id="row17977171010144">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.7%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p2793159171311">

config

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="82.3%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p879375920132">

Configuration files

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row6978161091412">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.7%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p37931659101311">

frameworks/surface

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="82.3%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p6793059171318">

Shared memory

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row6978201031415">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.7%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p117935599130">

frameworks/ui

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="82.3%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p0793185971316">

UI module, which defines functions related to UI components, animators
and fonts.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1897841071415">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.7%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p16793185961315">

hals

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="82.3%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p14793959161317">

Hardware abstraction layer (HAL) logic

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1420633124613">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.7%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p16207133194613">

interfaces/ui

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="82.3%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p182076317465">

Header files of open APIs related to the UI module

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1679114715461">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.7%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1079120477466">

interfaces/utils

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="82.3%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1279144754611">

Header files of utils for the graphics subsystem

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1534591617478">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.7%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p43456161472">

services/ims

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="82.3%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p23451616124717">

Input event management, including processing and distributing input
events such as click and press.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1044522874716">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.7%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p644516283476">

services/wms

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="82.3%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p194451528144716">

Window management, including creating, managing, and combining windows.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row48471930154713">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.7%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p4847830134713">

utils

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="82.3%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p8847193074715">

Public library of the graphics subsystem

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

Constraints
-----------

-  Language version

   -  C++ 11 or later

-  The specifications of the application framework vary depending on the
   System-on-a-Chip (SoC) and underlying OS capabilities.

   -  Cortex-M RAM and ROM:

      -  RAM: greater than 100 KB (recommended)
      -  ROM: greater than 300 KB

   -  Cortex-A RAM/ROM:

      -  RAM: greater than 1 MB (recommended)
      -  ROM: greater than 1 MB

Adding a UI Component
---------------------

All components inherit from the base class UIView and share common
attributes and styles. UI components are classified into common and
container ones. You can add child components for a container component,
but not for a common component.

Store new header files in the **interfaces/ui/components** directory and
.cpp files in the **frameworks/ui/src/components** directory. Override
**OnDraw** function to draw this UI component. Add the new file to the
**frameworks/ui/BUILD.gn** directory and it will be compiled to
**libui.so** during building.

Repositories Involved
---------------------

graphic_lite
