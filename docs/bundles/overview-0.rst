.. _overview-0:

Overview
========

This document describes how to develop OpenHarmony bundles and
distributions, and how to create, develop, and build code, as well as
burn and debug devices by using a command line tool.

-  A bundle usually maps onto a code repository, which is a code archive
   with the **bundle.json**, **README**, and **LICENSE** files.
-  A distribution consists of multiple bundles. Each distribution
   integrates various bundles of a comprehensive system, such as the
   driver, kernel, framework, and applications. These bundles can be
   used for device burning.

**Table 1** Differences between a bundle and a distribution

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row17288183614415">

.. raw:: html

   <th class="cellrowborder" valign="top" width="16.24162416241624%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p528818361545">

Aspect

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="33.31333133313331%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p1288836247">

Bundle

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50.44504450445044%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p112885362418">

Distribution

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

   <tr id="row1728813361848">

.. raw:: html

   <td class="cellrowborder" valign="top" width="16.24162416241624%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2010613564815">

Application scenario

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.31333133313331%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1910555184818">

Feature-oriented

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.44504450445044%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p13871955484">

System-oriented

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row676745614472">

.. raw:: html

   <td class="cellrowborder" valign="top" width="16.24162416241624%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1028816365414">

Content

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.31333133313331%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p428812361042">

Codes or a binary library for implementing features

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.44504450445044%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p328817366417">

List of dependent bundles as well as their compiling and building
scripts

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row95114356">

.. raw:: html

   <td class="cellrowborder" valign="top" width="16.24162416241624%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p184894513517">

Integrity

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.31333133313331%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1951741155">

A part of the operating system

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.44504450445044%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p20521542512">

An entire operating system

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row13581419518">

.. raw:: html

   <td class="cellrowborder" valign="top" width="16.24162416241624%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p859171059">

Compilation result

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.31333133313331%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p259201355">

Bundles

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.44504450445044%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p459414519">

System image

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

**Figure 1** Composition of bundles and distributions

|image1|

.. |image1| image:: figures/en-us_image_0000001054663940.png
