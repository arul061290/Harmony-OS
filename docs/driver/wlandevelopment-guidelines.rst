WLAN Development Guidelines
===========================

The WLAN driver is developed based on the HDF and PAL. It provides a
unified driver model for WLAN modules of different vendors regardless of
the operating system (OS) and system on a chip (SoC).

Limitations and Constraints
---------------------------

None

How to Develop
--------------

1. Configure hardware parameters such as **module** (different features)
   and **chip** in the **wifi_config.hcs** file.
2. Parse the **wifi_config.hcs** file and generate a structure with the
   configured parameters.
3. Initialize and create a module.
4. Mount and initialize the chip.
5. Initialize the bus.
6. Mount the upper-layer WPA service.

..

   |image1| **NOTE:** Some of the above adaptation steps have been
   provided. For details, see the third part **Development Example**.
   The steps waiting to be performed by developers include modifying
   configuration parameters based on hardware parameters, adapting and
   mounting a module, and performing tests and verification.

.. |image1| image:: public_sys-resources/icon-note.gif
