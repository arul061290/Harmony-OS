Driver Subsystem
================

Overview
--------

The OpenHarmony driver subsystem is constructed using the C
object-oriented programming (OOP). It provides a unified driver platform
through platform decoupling, kernel decoupling, and compatible kernels.
This unified driver architecture platform is designed to provide a more
precise and efficient development environment, where you develop a
driver that can be deployed on different systems supporting HDF.

The OpenHarmony driver subsystem provides the following key features and
capabilities to shorten the driver development period and make
third-party device driver integration much easier:

-  Flexible framework capabilities

   Based on the traditional driver framework, the OpenHarmony driver
   subsystem builds flexible framework capabilities to deploy terminal
   products with the capacity ranging from hundreds KB to hundreds MB of
   memory.

-  Standardized driver APIs

   The OpenHarmony driver subsystem provides you with abundant and
   stable driver APIs, which are compatible with those of future-proof
   smartphones, tablets, smart TVs.

-  Component-based driver models

   The OpenHarmony driver subsystem supports component-based driver
   models. It provides more refined driver management to dismantle
   components, enabling you to focus on the interaction between the
   hardware and driver.

   The subsystem also presets some template-based driver model
   components, such as the network device models.

-  Normalized configuration GUIs

   The OpenHarmony driver subsystem provides a unified configuration GUI
   and a cross-platform tool for configuration conversion and generation
   to implement seamless switchover across platforms.

You can use DevEco to manage driver projects, generate driver templates,
and manage settings to make the development of OpenHarmony drivers
easier.

Architecture
------------

The OpenHarmony driver framework adopts the primary/secondary mode and
is developed based on the framework, model, competence library, and
tool.

**Figure 1** Interaction between the driver and framework

|image1|

-  Driver framework stored in the **frameworks/core** directory

   -  Loads and starts drivers.
   -  Deploys and expands the driver framework flexibly through the
      object manager.

-  Driver models stored in the **frameworks/model** directory

   -  Provides model-based driving capabilities, such as network device
      models.

-  Driver capability library stored in the **frameworks/ability**
   directory

   -  Provides basic driver models, such as the I/O communication model.

-  Driver tools stored in the **frameworks\tools** directory

   -  Provides tools for HDI API conversion, and driver configuration
      and driver compilation.

-  Driver APIs stored in the **lite\hdi** directory

   -  Provides normalized driver APIs.

-  Support stored in the **frameworks/support** directory

   -  Provides platform driver APIs and system APIs with normalized
      abstraction capabilities.

Directory Structures
--------------------

**Table 1** Directory structure of the OpenHarmony driver framework

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row7977610131417">

.. raw:: html

   <th class="cellrowborder" valign="top" width="30.34%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p18792459121314">

Directory

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="69.66%" id="mcps1.2.3.1.2">

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

   <tr id="row17666001869">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p4667601064">

hdf

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p154741318610">

Indicates the OpenHarmony driver framework.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row17977171010144">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p2793159171311">

hdf/frameworks

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p879375920132">

Provides the source code to develop the driver frameworks, driver
models, and capability model libraries.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row258624313915">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p858718432912">

hdf/frameworks/ability

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1866016071012">

Provides functional capabilities for the driver development, such as the
message model libraries.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row6978161091412">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p37931659101311">

hdf/frameworks/core

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p6793059171318">

Provides the core code to implement the OpenHarmony driver framework.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row6978201031415">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p117935599130">

hdf/frameworks/core/host

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p53051522133">

Provides functions of the driver host environment framework, including:

.. raw:: html

   </p>

.. raw:: html

   <p id="p168291956191214">

1. Loading and starting a driver, and dispatching device nodes.

.. raw:: html

   </p>

.. raw:: html

   <p id="p945834131310">

2. Dispatching events.

.. raw:: html

   </p>

.. raw:: html

   <p id="p1365513245138">

3. Managing the internal power status.

.. raw:: html

   </p>

.. raw:: html

   <p id="p113814121414">

4. Managing the common driver resource configurations.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row138241821218">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1138321861211">

hdf/frameworks/core/manager

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p103831518181211">

Provides the management modules of the driver framework, including:

.. raw:: html

   </p>

.. raw:: html

   <p id="p1125114971315">

1. Driver API management module.

.. raw:: html

   </p>

.. raw:: html

   <p id="p419655510136">

2. Driver configuration management module.

.. raw:: html

   </p>

.. raw:: html

   <p id="p95776361144">

3. Device node management module.

.. raw:: html

   </p>

.. raw:: html

   <p id="p75789456140">

4. Security management module.

.. raw:: html

   </p>

.. raw:: html

   <p id="p183476761517">

5. Fault management module.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row116251627171512">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p76251275152">

hdf/frameworks/core/shared

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p56256278150">

Provides shared code for the host and manager.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2306123015162">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p10306143019164">

hdf/frameworks/model

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1030713021612">

Provides a universal framework model for drivers.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2021312310176">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p421315312177">

hdf/frameworks/model/network

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p421313113179">

Provides network device models for drivers.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2167642189">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p21683416181">

hdf/frameworks/support

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p71681548183">

Provides drivers with system APIs and hardware, such as GPIO, I2C, and
SPI capabilities.

.. raw:: html

   </p>

.. raw:: html

   <p id="p19848191416195">

Some interfaces can be migrated across platforms.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row116634294203">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1866392919204">

hdf/frameworks/support/platform

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p5663329202017">

Provides APIs that support the common hardware of platforms, such as
GPIO, I2C, and SPI capabilities.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row193157275210">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1331513279211">

hdf/frameworks/tools

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p131542762113">

Provides the driver capability libraries, such as the tool that
configures and compiles the HCS (HDF Configuration Source).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row66349163223">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p2634161611224">

hdf/frameworks/utils

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p26341516202215">

Provides basic data structures and algorithms.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1897841071415">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p16793185961315">

hdf/lite/adapter

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p14793959161317">

Adapts to kernel operation APIs and provides abstract APIs.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row16448173512518">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p644893514514">

hdf/lite/include

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1744933517511">

Provides driver APIs for lightweight devices.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row192731625216">

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.34%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p10281116185217">

hdf/lite/hdi

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p7286165524">

Provides APIs of the OpenHarmony driver.

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

None

Use
---

**Figure 2** Interaction between the driver and framework

|image2|

Driver loading is mostly done by the driver framework, and you only need
to register and configure required APIs. The driver framework will load
and initialize the driver based on the parsing content.

Driver development based on the HDF consists of the following three
parts:

1. Driver: develop the functions.

2. Information configuration: present the loading information of the
   driver.

3. Resource configuration: configure the hardware information of the
   driver.

The driver mainly aims to develop the functions.

The first part that catches your eyes is the driver entry, which is
described through **DriverEntry**.

Three APIs are available, namely **bind**, **init**, and **release**.

::

   struct HdfDriverEntry g_deviceSample = {
       .moduleVersion = 1,
       .moduleName = "sample_driver", 
       .Bind = SampleDriverBind,
       .Init = SampleDriverInit,
       .Release = SampleDriverRelease,
   };

**Bind**: This API is used to bind driver devices and its functions.

::

   int32_t SampleDriverBind(struct HdfDeviceObject *deviceObject)
   {
       // TODO: Bind device service to device object.
       // And you can also initialize device resources here.
       return HDF_SUCCESS;
   }

Description of Init: When devices are successfully bound, the framework
calls Init to initialize the driver. After initialization is complete,
the driver framework will determine whether to create external service
interfaces based on the configuration file. If the driver fails to be
initialized, the driver framework will automatically release the created
device interface.

::

   int32_t SampleDriverInit(struct HdfDeviceObject *deviceObject)
   {
       // TODO: Init hardware or other resources here.
       return HDF_SUCCESS;
   }

**Release**: When you need to uninstall a driver, the drive framework
calls this function to release the driver resources. Then, other
internal resources will be released.

::

   void SampleDriverRelease(struct HdfDeviceObject *deviceObject)
   {
       // Release all resources.
       return;
   }

Installation
------------

The OpenHarmony driver is mainly deployed in the kernel space using the
static link mode. It is compiled and packed with the kernel subsystem
and system image.

**Figure 3** OpenHarmony driver installation

|image3|

Repositories Involved
---------------------

`drivers_hdf_frameworks <https://openharmony.gitee.com/openharmony/drivers_hdf_frameworks>`__

`drivers_hdf_lite <https://openharmony.gitee.com/openharmony/drivers_hdf_lite>`__

.. |image1| image:: figures/en-us_image_0000001053805078.png
.. |image2| image:: figures/en-us_image_0000001052764349.png
.. |image3| image:: figures/en-us_image_0000001053044331.png
