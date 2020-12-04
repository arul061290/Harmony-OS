OHOS::UIScrollView::OnScrollListener
====================================

**Overview**\ 
--------------

**Related Modules:**

`Graphic <graphic.md>`__

**Description:**

Represents a listener that contains a callback to be invoked upon scroll
state changes. The state can either be **SCROLL_STATE_STOP** or
**SCROLL_STATE_MOVE**.

**Since:**

1.0

**Version:**

1.0

**Summary**\ 
-------------

Public Member Functions
-----------------------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row732285466093534">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p637744680093534">

Public Member Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p4438132093534">

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

   <tr id="row1030275338093534">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1813387675093534">

OnScrollListener ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p925778424093534">

.. raw:: html

   </p>

.. raw:: html

   <p id="p1974057277093534">

A constructor used to create an OnScrollListener instance with the
default scroll state SCROLL_STATE_STOP.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row310155202093534">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p402601820093534">

~OnScrollListener ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1394584269093534">

virtual

.. raw:: html

   </p>

.. raw:: html

   <p id="p799999362093534">

A destructor used to delete the OnScrollListener instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1037079787093534">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1320919184093534">

OnScrollStart ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p692421806093534">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1881544119093534">

Called when a scroll starts.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1637565398093534">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p278352355093534">

OnScrollEnd ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1059250463093534">

virtual void

.. raw:: html

   </p>

.. raw:: html

   <p id="p173972467093534">

Called when a scroll ends.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2019926486093534">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p998400031093534">

GetScrollState () const

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p785207086093534">

uint8_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p711135678093534">

Obtains the scroll state of this view.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row437894882093534">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p938346530093534">

operator new (size_t size)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p187166280093534">

void \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1418607459093534">

Overrides the new function.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row630873310093534">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p426946833093534">

operator delete (void \*p)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1971679501093534">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1480736647093534">

Overrides the delete function.

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
