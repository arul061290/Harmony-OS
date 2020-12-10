Distributed Scheduler
=====================

Overview
--------

The Distributed Scheduler is used for cross-device component management.
It allows the local device to access or control remote components, and
enables application collaboration in distributed scenarios. The
following figure shows the modules in the Distributed Scheduler.

|image1|

Directory Structure
-------------------

The following table describes the directory structure of the Distributed
Scheduler.

**Table 1** Directory structure of the major source code

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row20416556201718">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p10416456121716">

Directory

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1841645631717">

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

   <tr id="row64161056151718">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p9416656181720">

dtbschedmgr_lite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p541645611177">

Implementation of the Distributed Scheduler

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row104169564177">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p17416125614179">

safwk_lite

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p04163569170">

Implementation of the foundation process

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

The source code directory structure of the Distributed Scheduler is as
follows:

::

   ├── BUILD.gn
   ├── include
   │  ├── distributed_schedule_service.h        # Header file for the open APIs provided by the Distributed Scheduler
   │  ├── dmslite_check_remote_permission.h     # Header file for the permission management module of the Distributed Scheduler
   │  ├── dmslite_famgr.h                       # Header file for the FA management module of the Distributed Scheduler
   │  ├── dmslite_inner_common.h                # Internal common file for the Distributed Scheduler
   │  ├── dmslite.h                             # Header file for the implementation of the Distributed Scheduler Service
   │  ├── dmslite_log.h                         # Header file for the log module
   │  ├── dmslite_msg_parser.h                  # Header file for the distributed message parsing module
   │  ├── dmslite_tlv_common.h                  # Header file for the TLV data parsing module
   │  └── dmslite_session.h                     # Header file for the inter-device communication module
   ├── readme.rst
   ├── LICENSE
   ├── source
       ├── distributed_schedule_service.c
       ├── dmslite.c
       ├── dmslite_check_remote_permission.c
       ├── dmslite_famgr.c
       ├── dmslite_msg_parser.c
       ├── dmslite_tlv_common.c
       └── dmslite_session.c

Constraints
-----------

**Language**: C or C++

**Networking environment**: The primary and secondary devices must be on
the same LAN and can ping each other.

**Operating system**: OpenHarmony

**Limitations and constraints on remote startup**:

-  Only FAs can be started remotely. Remote startup is unavailable to
   abilities using the Service template.
-  Before the remote startup, ensure that the distributed networking
   between the primary and secondary devices is successful. Otherwise,
   the remote startup fails.

Usage
-----

-  **Compiling the Distributed Scheduler**

The code of the Distributed Scheduler is stored in the following
directory:

::

   foundation/distributedschedule/services/dtbschedmgr_lite

When compiling the code for a specific platform, you need to specify the
target platform. The following code snippet uses code compilation for
the Hi3516DV300 platform as an example:

::

   python build.py ipcamera -p hi3516dv300_liteos_a

-  **Primary device development** (taking FA startup as an example)

Create a **Want** instance to set the remote device ID, bundle name, and
ability class name of the target FA and set the
**Want.FLAG_ABILITYSLICE_MULTI_DEVICE** flag to enable distributed
startup.

::

   import ohos.aafwk.ability.Ability;
   import ohos.aafwk.content.Want;
   import ohos.bundle.ElementName;

   // Create a Want instance that will be passed to the startAbility method.
   Want want = new Want();
   ElementName name = new ElementName(remote_device_id, "com.huawei.remote_bundle_name", "remote_ability_name"); 
   want.setElement(name); // Add information about the target FA for startup to the Want instance.
   want.setFlags(Want.FLAG_ABILITYSLICE_MULTI_DEVICE); // Set the multi-device startup flag. If this flag is not set, remote FA startup will be unavailable.

   // Start the remote FA on the secondary device.
   startAbility(want); // Start the specified FA based on the want parameter. If the name and type of the want parameter are different from those used in the IDE, use the parameter name and type in the IDE.

-  **Prerequisites**

The target FA with the specified bundle name must have been installed on
the secondary device.

-  **Execution** (taking FA startup as an example)

Call the **startAbility** method on the primary device to start the
target FA on the secondary device.

Repositories Involved
---------------------

distributedschedule_interfaces_kits_samgr_lite

distributedschedule_services_dtbschedmgr_lite

distributedschedule_services_safwk_lite

.. |image1| image:: figures/en-us_image_0000001055103250.png
