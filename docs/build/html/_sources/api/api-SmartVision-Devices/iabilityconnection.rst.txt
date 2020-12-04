IAbilityConnection
==================

**Overview**\ 
--------------

**Related Modules:**

`AbilityKit <abilitykit.md>`__

**Description:**

Provides callbacks to be invoked when a remote `Service <service.md>`__
ability is connected or disconnected.

**Summary**\ 
-------------

Data Fields
-----------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1519684370093531">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p447945243093531">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p69779550093531">

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

   <tr id="row1852392276093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1636655364093531">

OnAbilityConnectDone )(ElementName *elementName,
SvcIdentity*\ serviceSid, int resultCode, void \*data)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p384130105093531">

void(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p998948282093531">

Called when a client is connected to a Service ability.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1262690490093531">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1055921306093531">

OnAbilityDisconnectDone )(ElementName *elementName, int resultCode,
void*\ data)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p594567871093531">

void(\*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1012132056093531">

Called after all connections to a Service ability are disconnected.

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
