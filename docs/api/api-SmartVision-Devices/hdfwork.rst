HdfWork
=======

**Overview**\ 
--------------

**Related Modules:**

`DriverUtils <driverutils.rst>`__

**Description:**

Describes a work item and a delayed work item. This structure defines
the work and delayed work items, and then calls the initialization
function
`HdfWorkInit <driverutils.rst#gad171adc8eda320fd01049a2b87ea62fb>`__ or
`HdfDelayedWorkInit <driverutils.rst#ga55bf669dc6740c65e4d45a4f641db2f1>`__
to perform initialization. The
`HdfAddWork() <driverutils.rst#ga82cc68d656aa17317634b07d49dae160>`__
function is to add a work item to a work queue immediately, and the
`HdfAddDelayedWork() <driverutils.rst#gaef781ccc1579db3070745088da47b2c5>`__
function is to add a work item to a work queue after the configured
delayed time.

**Summary**\ 
-------------

Data Fields
-----------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row540227682093530">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p601732280093530">

Variable Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2113177913093530">

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

   <tr id="row1156814672093530">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p983577245093530">

realWork

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p834767806093530">

void \*

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

realWork
--------

::

   void* HdfWork::realWork

**Description:**

Pointer to a work item and a delayed work item
