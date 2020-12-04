OHOS::DragEvent
===============

**Overview**\ 
--------------

**Related Modules:**

`Graphic <graphic.md>`__

**Description:**

Defines a drag event, which indicates a certain movement (more than 10
pixels) after a view is pressed.

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

   <tr id="row1749356511093535">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1791354777093535">

Public Member Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1118526305093535">

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

   <tr id="row420118413093535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p979562917093535">

DragEvent (const Point &newPos, const Point &lastPos, const Point
&totalLen)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p472832500093535">

.. raw:: html

   </p>

.. raw:: html

   <p id="p1110172948093535">

A constructor used to create a DragEvent instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2060032513093535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p358336541093535">

~DragEvent ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p763444014093535">

virtual

.. raw:: html

   </p>

.. raw:: html

   <p id="p11648280093535">

A destructor used to delete the DragEvent instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row703305271093535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p97536297093535">

GetLastPoint () const

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p103989620093535">

const Point &

.. raw:: html

   </p>

.. raw:: html

   <p id="p920257711093535">

Obtains the coordinates of the last position in the drag event.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1599633837093535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1900763694093535">

GetStartPoint () const

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1630901005093535">

const Point &

.. raw:: html

   </p>

.. raw:: html

   <p id="p507052005093535">

Obtains the start coordinates in the drag event.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row728213705093535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p993314566093535">

SetPreLastPoint (const Point &preLastPos)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p319866975093535">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1159771053093535">

Sets the coordinates of the stay position before the last position in
the drag event.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1559667377093535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2102779832093535">

GetPreLastPoint () const

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p590482368093535">

const Point &

.. raw:: html

   </p>

.. raw:: html

   <p id="p1448883756093535">

Obtains the coordinates of the stay position before the last position in
the drag event.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row599354748093535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p240305858093535">

GetDragDirection () const

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p525103650093535">

uint8_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1457964967093535">

Obtains the direction in the drag event.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1845488858093535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1755301367093535">

GetDeltaX () const

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1430399560093535">

int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p172114056093535">

Obtains the difference between the current position and the last
position of the view in the x-axis.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row191109740093535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p420430065093535">

GetDeltaY () const

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p889648627093535">

int16_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1797700697093535">

Obtains the difference between the current position and the last
position of the view in the y-axis.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1724128163093535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p428300760093535">

Event ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p908651811093535">

.. raw:: html

   </p>

.. raw:: html

   <p id="p1882226633093535">

A default constructor used to create an Event instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row122274591093535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p463944550093535">

Event (const Point &curPos)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1410213984093535">

.. raw:: html

   </p>

.. raw:: html

   <p id="p1609553664093535">

A constructor used to create an Event instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1351168419093535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1174105924093535">

~Event ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1883693774093535">

virtual

.. raw:: html

   </p>

.. raw:: html

   <p id="p1812392750093535">

A destructor used to delete the Event instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row475153781093535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1630548778093535">

GetCurrentPos () const

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1032244522093535">

const Point &

.. raw:: html

   </p>

.. raw:: html

   <p id="p242100536093535">

Obtains the position where an event occurs.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row9636156093535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p70110628093535">

GetTimeStamp () const

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1364767409093535">

const TimeType &

.. raw:: html

   </p>

.. raw:: html

   <p id="p2015892218093535">

Obtains the timestamp when an event occurs.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1543475498093535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p11359895093535">

SetTimeStamp (const TimeType &timeStamp)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1839883773093535">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p366250085093535">

Sets the timestamp when an event occurs.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row19153108093535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1628612281093535">

operator new (size_t size)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p909969992093535">

void \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p531446792093535">

Overrides the new function.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row66974360093535">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p214435319093535">

operator delete (void \*p)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1143726140093535">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p235781896093535">

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
