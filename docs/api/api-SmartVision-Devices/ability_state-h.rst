ability_state.h
===============

**Overview**\ 
--------------

**Related Modules:**

`AbilityKit <abilitykit.rst>`__

**Description:**

Declares ability-related functions, including ability lifecycle
callbacks and functions for connecting to or disconnecting from Particle
Abilities. As the fundamental unit of OpenHarmony applications,
abilities are classified into `Feature <feature.rst>`__ Abilities and
Particle Abilities. `Feature <feature.rst>`__ Abilities support the Page
template, and Particle Abilities support the `Service <service.rst>`__
template. An ability using the Page template is called a Page ability
for short and that using the `Service <service.rst>`__ template is called
a `Service <service.rst>`__ ability.

**Since:**

1.0

**Version:**

1.0

**Summary**\ 
-------------

Enumerations
------------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row628547594084828">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1732612963084828">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1581004586084828">

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

   <tr id="row557122420084828">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1076909722084828">

State { STATE_UNINITIALIZED, STATE_INITIAL, STATE_INACTIVE,
STATE_ACTIVE, STATE_BACKGROUND }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p733131520084828">

Enumerates all lifecycle states that an ability will go through over the
course of its lifetime.

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
