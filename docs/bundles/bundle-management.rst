.. _compose1:

Bundle Management
=================

Dependency
----------

A basic **bundle.json** file needs to be enriched by bundle dependencies
to implement more complex features. Bundle names and version numbers
should be defined in the **dependencies** field of **bundle.json**.

::

   {
       "name": "my-bundle",
       "version": "1.0.0",
       "dependencies": {
           "net": "1.0.0"
       }
   }

In this example, **my-bundle** depends on **net 1.0.0**. After you
globally install the hpm-cli tool, run the following command to obtain
bundle dependencies from the remote repository:

::

   hpm install 

Bundle dependencies are then stored in the **ohos_bundles** folder in
the root directory of the current bundle. A tree structure illustrating
the bundle and its dependencies will be generated. You need to run the
following command in the root directory of the bundle:

::

   username@server MINGW64 /f/showcase/demo/demo
   $ hpm list
   +--demo@1.0.0
   | +--@huawei/media@1.0.2
   | +--@demo/sport_hi3518ev300_liteos_a@1.0.0
   | | +--@demo/app@4.0.1
   | | | +--@demo/build@4.0.1
   | | | +--@demo/arm_harmonyeabi_gcc@4.0.0   
   | | +--@demo/liteos_a@4.0.0
   | | | +--@demo/third_party_fatfs@4.0.0     
   | | | +--@demo/arm_harmonyeabi_gcc@4.0.0   
   | | +--@demo/init@4.0.0
   | | +--@demo/dist_tools@4.0.0

Alternatively, you can view the dependencies of the current bundle in a
graph by running the following command:

::

   hpm dependencies

A **deps_visual** folder is generated in the current directory. The
folder contains the **deps.html** and **deps-data.js** files. After you
open the **deps.html** file via a browser, you can view bundle
dependencies illustrated by a graph, as shown in the following figure.

Each dependency type is indicated by a different color at the
corresponding node. You can move the mouse pointer to a node to view the
implied information.

| **Figure 1** Bundle dependencies
| |image1|

HPM Command Reference
---------------------

You can use the hpm-cli tool to manage the lifecycle of a bundle. The
following table describes available HPM commands. (You can run the **hpm
-h** command to get the command details).

**Table 1** HPM commands

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row125101745103718">

.. raw:: html

   <th class="cellrowborder" valign="top" width="20.95209520952095%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p1451014454371">

Function

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="30.623062306230626%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p17510144553716">

Command

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="48.42484248424842%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p65102452371">

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

   <tr id="row25106453375">

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.95209520952095%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p151044514378">

Querying version information

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.623062306230626%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1653795113472">

hpm -V or hpm –version

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="48.42484248424842%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p399295684713">

Queries the hpm-cli version number.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row651017455374">

.. raw:: html

   <td class="cellrowborder" rowspan="2" align="left" valign="top" width="20.95209520952095%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p551054516372">

Querying help information

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.623062306230626%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p18648167124812">

hpm -h or hpm –version

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="48.42484248424842%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1464811794817">

Queries the command list and help information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1751016452379">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p16778111111487">

hpm -h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1877811154818">

Queries command reference.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2511945123715">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="20.95209520952095%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p3955174864810">

Creating a project

.. raw:: html

   </p>

.. raw:: html

   <p id="p14511184518374">

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.623062306230626%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2046811558481">

hpm init bundle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="48.42484248424842%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1646818557481">

Creates a bundle project.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row351184593713">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p18991313496">

hpm init -t template

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p109912104911">

Creates a scaffolding project based on the template.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1751164511374">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="20.95209520952095%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1351111454374">

Installing bundles

.. raw:: html

   </p>

.. raw:: html

   <p id="p251144513715">

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.623062306230626%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p8896182914913">

hpm install or hpm i

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="48.42484248424842%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1289692919493">

Installs dependent bundles in the bundle.json file.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row15511194563712">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p17917436134911">

hpm install bundle@version

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1891723611494">

Installs bundles of a specified version.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row21051110155011">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="20.95209520952095%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1630384435010">

Uninstalling bundles

.. raw:: html

   </p>

.. raw:: html

   <p id="p83417161509">

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.623062306230626%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p288195017502">

hpm uninstall bundle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="48.42484248424842%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2088450165014">

Removes dependent bundles.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row73341617507">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p934161613508">

hpm remove or hpm rm bundlename

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p234111685016">

Removes dependent bundles.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row166449214501">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="20.95209520952095%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p8645421125016">

Viewing information

.. raw:: html

   </p>

.. raw:: html

   <p id="p12645202115014">

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.623062306230626%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p679412535211">

hpm list or hpm ls

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="48.42484248424842%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p07941451526">

Displays the bundle tree of available bundles and distributions.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1764552105017">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p035818131525">

hpm dependencies

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p19358413135217">

Generates the dependency diagram (in HTML format) of available bundles
and distributions.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1553428145020">

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.95209520952095%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p353202845014">

Searching for bundles

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.623062306230626%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1423903005211">

hpm search name

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="48.42484248424842%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p17239163018524">

Searches for bundles. –json is used to specify the search result in JSON
format, and -type is used to set the target type, which can be bundle,
distribution, or code-segment.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row135482855018">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="20.95209520952095%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p38201311174016">

Setting HPM configuration items

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.623062306230626%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p279915013522">

hpm config set key value

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="48.42484248424842%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p157991450205211">

Sets configuration items, such as the server address and network proxy.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row454172810509">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p111125615215">

hpm config delete key

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p171156105215">

Deletes configurations.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row3925233115011">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="20.95209520952095%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1250314020555">

Updating bundle versions

.. raw:: html

   </p>

.. raw:: html

   <p id="p59251633105018">

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.623062306230626%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1127981305516">

hpm update

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="48.42484248424842%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p427971311555">

Updates the versions of dependent bundles.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row692503385015">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p627961317557">

hpm check-update

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p3279121315557">

Checks whether version updates are available to dependent bundles.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1925173385019">

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="20.95209520952095%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2925133305014">

Building

.. raw:: html

   </p>

.. raw:: html

   <p id="p692515335501">

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.623062306230626%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2058919655611">

hpm build

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="48.42484248424842%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1958920625619">

Builds a bundle or distribution.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row18925233115016">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1958912618563">

hpm dist

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2058936115611">

Packs a distribution, depending on the dist script in scripts of
bundle.json.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row59261233155013">

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.95209520952095%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p3926123305011">

Packing

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.623062306230626%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1785810219574">

hpm pack

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="48.42484248424842%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1485872165714">

Packs dependencies of local bundles.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1592653305016">

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.95209520952095%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p84251810125716">

Burning

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.623062306230626%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p7973616175716">

hpm run flash

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="48.42484248424842%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p20973111612575">

Burns the firmware, depending on the flash script in scripts of
bundle.json.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row992615339504">

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.95209520952095%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1225172310576">

Publishing

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.623062306230626%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p198081455105712">

hpm publish

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="48.42484248424842%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p880885516574">

Publishes a bundle, which must be unique in the repository and has a
unique version. (An account is required for login.)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row5926333135014">

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.95209520952095%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p39267336504">

Running extended commands

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.623062306230626%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p9933172588">

hpm run

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="48.42484248424842%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p18933476584">

Runs the commands in scripts defined in bundle.json. Multiple commands
can be executed in batches by using &&.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row122864915206">

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.95209520952095%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1529124912207">

Generating a key

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.623062306230626%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p9291492204">

hpm gen-keys

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="48.42484248424842%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p429249182012">

Generates a public-private key pair and configures the public key on the
hpm server, achieving password-free hpm-cli login for bundle publishing.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row3556450102011">

.. raw:: html

   <td class="cellrowborder" valign="top" width="20.95209520952095%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p35561850172015">

Generating third-party open source notice

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="30.623062306230626%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1155625018209">

hpm gen-notice

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="48.42484248424842%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p11557175015205">

Generates a joint file describing the notice on third-party open source
based on the description of each bundle.

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

.. |image1| image:: figures/bundle-dependencies.png
