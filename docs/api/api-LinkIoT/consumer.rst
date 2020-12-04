Consumer
========

**Overview**\ 
--------------

**Related Modules:**

`Broadcast <broadcast.md>`__

**Description:**

Defines the topic consumer used to receive events and push data. You
need to implement this struct for your application.

**Summary**\ 
-------------

Data Fields
-----------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1177098769191858">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1510694763191858">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p359040708191858">

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

   <tr id="row541337055191858">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p664636100191858">

identity

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p788137349191858">

const Identity \*

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1891627096191858">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p830646910191858">

Notify )(Consumer *consumer, const Topic*\ topic, const Request
\*origin)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1596993159191858">

void(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p711307819191858">

Defines how the consumer will process the events or data of a released
topic.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row551589053191858">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p381665072191858">

Equal )(const Consumer *current, const Consumer*\ other)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1685313723191858">

BOOL(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p886417998191858">

Checks whether two consumers are equal.

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

Equal
-----

::

   BOOL(* Consumer::Equal) (const [Consumer](consumer.md) *current, const [Consumer](consumer.md) *other)

**Description:**

Checks whether two consumers are equal.

You need to implement this function to prevent repeated topic
subscription.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row900903701191858">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1944786767191858">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1202034969191858">

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

   <tr id="row486662959191858">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

current

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the current consumer.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1035514191191858">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

other

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the target consumer to compare.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **TRUE** if the two consumers are equal; returns **FALSE**
otherwise.

identity
--------

::

   const [Identity](identity.md)* Consumer::identity

**Description:**

`Consumer <consumer.md>`__ ID

Notify
------

::

   void(* Consumer::Notify) ([Consumer](consumer.md) *consumer, const [Topic](broadcast.md#gaf03f5bc94cad32ab628a6cdee09b0542) *topic, const [Request](request.md) *origin)

**Description:**

Defines how the consumer will process the events or data of a released
topic.

You can implement this function for consumers to process topics
associated with the them. Note that the passed topic must have been
subscribed by the consumer. Otherwise, the function does nothing.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row549325055191858">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1507178705191858">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2034406603191858">

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

   <tr id="row358410277191858">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

consumer

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates this pointer of the consumer.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1998990578191858">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

topic

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the topic to be processed.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2068793086191858">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

origin

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the data to be processed.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>
