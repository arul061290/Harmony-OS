.. _environmentvariables:

Environment Variables
=====================

During bundle compilation, system-provided environment variables are
required to define the output and link the required binary files. These
variables are injected into the context for executing scripts based on
service requirements. Therefore, their values can be directly obtained
from the scripts. Currently, there are global and fixed environment
variables in the system.

Global variables are defined by the*\* envs*\* attribute in
**bundle.json**. All dependent bundles can obtain the values of global
variables.

::

   {
       "envs": {
           "compileEnv": "arm"
       }
   }

Different parameters can be passed to bundles when introducing
dependencies so that the compilation of dependent bundles can meet the
requirements of the current bundle. The parameters defined in the
dependencies can be obtained from the context for executing the
corresponding scripts.

::

   {
       "dependencies": {
           "my-bundle": {
               "version": "1.0.0",
               "mode": "debug"
           }
       }
   }

When linking to a binary file, the bundle needs to know the file path
regarding the dependencies. Therefore, the path (as an environment
variable) is passed to the bundle for compiling.

The passed environment variable is in **DEP\_\ BundleName** format,
where **BundleName** indicates the name of the dependent bundle, for
example, **DEP_first-bundle**.

Tags can be defined to group dependent bundles. You can obtain the path
of a group of dependent bundles based on their tag. A tag starts with a
number sign (#) and is defined as follows:

::

   {
       "dependencies": {
           "#tool": {
               "first-bundle": "1.0.0",
               "second-bundle": "1.0.0"
           },
           "#drivers": {
               "xx-bundle": "1.0.0",
               "yy-bundle": "1.0.0"
           }
       }
   }

There are two fixed environment variables:

-  **DEP_OHOS_BUNDLES**: path of the **ohos_bundles** folder
-  **DEP_BUNDLE_BASE**: path of the outermost bundle
