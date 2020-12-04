WLAN
====

**Overview**\ 
--------------

Defines a WLAN module that supports cross-OS migration, component
adaptation, and modular assembly and compilation. Driver developers of
WLAN vendors can adapt their driver code based on the unified APIs
provided by the WLAN module.

**Since:**

1.0

**Version:**

1.0

**Summary**\ 
-------------

Files
-----

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1064036438093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p233322258093521">

File Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2061445838093521">

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

   <tr id="row499289373093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p909299226093521">

hdf_netbuf.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2110586225093521">

Declares network data buffers and provides APIs for operating buffer
queues.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1787544166093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1491486594093521">

hdf_wifi_event.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1403426801093521">

Declares WLAN driver events.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row69089035093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1779954528093521">

hdf_wifi_product.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1201369947093521">

Declares the data structure of the WLAN module.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row743253160093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p845428352093521">

net_device.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p747529589093521">

Defines WLAN network device interfaces.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row24149158093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p221586967093521">

wifi_inc.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1402142807093521">

Describes the data structure of WLAN features and bus.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1865050497093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1200132844093521">

wifi_mac80211_ops.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1277351824093521">

Declares Media Access Control (MAC) APIs and functions related to
control flows.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row549534787093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1142832213093521">

wifi_module.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2112715077093521">

Provides features of the WLAN module and functions to create and delete
modules.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row76372038093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2050284379093521">

wifi_module_config.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p139806621093521">

Declares the WLAN module configuration.

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

Data Structures
---------------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row141832523093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p690439747093521">

Data Structure Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p113170810093521">

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

   <tr id="row9502491093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p560538330093521">

NetBuf

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p208496977093521">

Records and saves a network data buffer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1907959935093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p636951808093521">

NetBufQueue

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p63475621093521">

Indicates the queues for storing network data.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row707548388093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p657289311093521">

RateInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2032024884093521">

Defines the rate information received or sent over WLAN.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row772840274093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2066581875093521">

StaBssParameters

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p695958226093521">

Defines parameters related to the WLAN module that works in station
mode.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row88950975093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p430266786093521">

StaFlagUpdate

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p344375364093521">

Defines the update of the Sta flag.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1536415972093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1859095551093521">

StationInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1508572422093521">

Defines station information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row299797011093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p336510059093521">

Auth

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p274043438093521">

Defines authentication information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row704263805093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p675952599093521">

Deauth

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1960550470093521">

Defines deauthentication information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row5412792093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p303706183093521">

AssocReq

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1728956553093521">

Defines station association request.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row782248963093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p826441534093521">

AssocResp

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1756512650093521">

Defines station association response.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row954526108093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1408860254093521">

ReassocReq

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p665464737093521">

Defines station reassociation request.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row89405871093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1047167247093521">

ReassocResp

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1469584027093521">

Defines station reassociation response.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row488827737093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p870754954093521">

Disassoc

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p647336979093521">

Defines station disconnection.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1052897316093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p447925989093521">

Beacon

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p819531317093521">

Defines the update of the Sta flag.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row825076606093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1255864321093521">

ProbeResp

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p557928960093521">

Defines scanning response.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row751801313093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p243391371093521">

Ieee80211Mgmt

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p486048034093521">

Defines management frame information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1254535416093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p605665799093521">

ScannedBssInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1880328342093521">

Represents the scanned BSS information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2117316923093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p364745918093521">

ConnetResult

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1432798966093521">

Defines association results.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2022269171093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p173039805093521">

HdfWifiProductData

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p414049965093521">

Defines the WLAN module.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1084299556093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p795519276093521">

EtherHeader

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p586633190093521">

Defines the Ethernet header information of a data frame, including the
destination address, source address, and Ethernet type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1752235291093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1569967924093521">

IpHeader

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p242695456093521">

Defines the IP header information of a data frame, including the version
number, service type, and total length.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1556444783093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1401201422093521">

UdpHeader

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1677372613093521">

Defines the UDP header information of a data frame, including the source
port number and destination port number.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row522892402093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p999264873093521">

TcpHeader

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p98102869093521">

Defines the TCP header information of a data frame, including the source
port number and destination port number.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1376776968093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1262125782093521">

IpV4Addr

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1457006741093521">

Defines an IPv4 address.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row717574912093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p768541574093521">

NetDevNotify

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2078885395093521">

Defines a network device notification, including an IP address and the
notification type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row320498075093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1909844898093521">

IfType

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p293847371093521">

Defines the network port type, for example, the WLAN network port.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1719376714093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p194340438093521">

IfReq

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p986239889093521">

Defines ioctrl data.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1540956459093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1079215788093521">

NetDevice

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p784919871093521">

Defines a network device, including the network interface category and
name, and network port type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row700946450093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p554033289093521">

NetDeviceInterFace

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1956786398093521">

Defines interfaces that need to be implemented externally by network
devices, including initializing, opening, and closing a network device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1895853320093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p47174955093521">

KeyParams

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p995458499093521">

Describes a key.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row468034304093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p818855732093521">

Ieee80211Channel

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p538029337093521">

Describes a communication channel.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1285287811093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p404335282093521">

Ieee80211Rate

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1752743204093521">

Describes the IEEE 802.11 rate.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1531580267093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1162135800093521">

Ieee80211McsInfo

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p860318930093521">

Describes IEEE 802.11 Modulation and Coding Scheme (MCS) information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1809913208093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p141383385093521">

Ieee80211StaHtCap

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2117465245093521">

Describes the IEEE 802.11 high-throughput (HT) capability.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1368755724093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2033350800093521">

Ieee80211SupportedBand

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1928665424093521">

Describes IEEE 802.11 band information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1330985831093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1160307636093521">

Wiphy

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p56590973093521">

Describes a wiphy device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row569162458093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p408163815093521">

WifiSsid

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1176427191093521">

Describes an SSID.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1891071806093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1452949300093521">

ChannelDef

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1472161073093521">

Describes a communication channel.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row815864284093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p273723267093521">

WirelessDev

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1408450980093521">

Describes a wireless device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1459981912093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p242929991093521">

WifiScanRequest

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p972549077093521">

Describes scan request parameters.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row597561842093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p990034844093521">

CryptoSettings

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p578763183093521">

Describes cryptography settings.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1701935831093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1326027287093521">

MacAddress

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1518318710093521">

Describes the device MAC address.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2132506794093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p697801893093521">

WifiConnectParams

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1158693485093521">

Describes parameters for a connection request.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row917854081093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p488241447093521">

VifParams

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1242828987093521">

Describes virtual API parameters.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2092009008093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1046918371093521">

StationDelParameters

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1540478746093521">

Describes parameters for canceling a connection.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row796876317093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2002204772093521">

MacConfigParam

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1564741660093521">

Describes MAC configuration parameters.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1500094117093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1129963181093521">

Mac80211DisconnectParam

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p738034650093521">

Describes disconnection parameters.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2003993255093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1923142583093521">

Mac80211Ssids

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1245718994093521">

Describes SSIDs.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row253925597093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p836628046093521">

Mac80211beaconParam

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1585464212093521">

Describes beacon parameters.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row966673384093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1849093146093521">

WifiMac80211Ops

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1373590705093521">

Describes MAC-layer control APIs that need to be implemented by the
driver.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1322833189093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1823218086093521">

WifiModuleIface

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1392948878093521">

Defines WLAN module APIs.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row396426309093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1898994044093521">

WifiModule

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p486339791093521">

Defines the WLAN module.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row416761624093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p697776248093521">

WifiFeature

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p547607750093521">

Defines a WLAN feature.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1771337728093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1546757029093521">

WifiFeatureList

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2106027039093521">

Defines the WLAN feature list.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1175948098093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2059654807093521">

HdfWifiChipData

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p965149221093521">

Defines a WLAN chip.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2102196107093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p28418855093521">

WifiModuleConfig

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p743877572093521">

Defines the WLAN module configuration.

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

Macros
------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1083713481093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1346718542093521">

Macro Name and Value

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p951259079093521">

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

   <tr id="row2103363263093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p779294698093521">

MAX_NETBUF_RESEVER_SIZE 68

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p406793757093521">

Defines the reserved field of a network data buffer used to store
private information.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row493248793093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p862934328093521">

MAC_ADDR_SIZE 6

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1730329062093521">

Indicates a 6-byte MAC address.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1328257539093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2082748639093521">

NET_DEVICE_IFF_RUNNING IFF_RUNNING

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p255693589093521">

Indicates that the network port is working.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1599878630093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2072317962093521">

ETHER_TYPE_RARP 0x8035

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p461488478093521">

Indicates Reverse Address Resolution Protocol (RARP).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1255670732093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p722331097093521">

ETHER_TYPE_PAE 0x888e

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1679615755093521">

Indicates Port Access Entity (PAE).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row186423003093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2001759119093521">

ETHER_TYPE_IP 0x0800

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1655603975093521">

Indicates Internet Protocol (IP).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row582868543093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p379286788093521">

ETHER_TYPE_AARP 0x80f3

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p92715721093521">

Indicates AppleTalk Address Resolution Protocol (AARP).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1254511343093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1962727669093521">

ETHER_TYPE_IPX 0x8137

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1445058775093521">

Indicates Internetwork Packet Exchange (IPX).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1702815546093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1024964039093521">

ETHER_TYPE_ARP 0x0806

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2141605739093521">

Indicates Address Resolution Protocol (ARP).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1183050640093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p263089245093521">

ETHER_TYPE_IPV6 0x86dd

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1380443883093521">

Indicates Internet Protocol version 6 (IPv6).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1045096616093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1089263405093521">

ETHER_TYPE_TDLS 0x890d

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p631111844093521">

Indicates Tunneled Direct Link Setup (TDLS).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2035521497093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1087253694093521">

ETHER_TYPE_VLAN 0x8100

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2146715715093521">

Indicates Virtual Local Area Network (VLAN).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1609740261093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1040138656093521">

ETHER_TYPE_WAI 0x88b4

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1497425893093521">

Indicates WLAN Authentication and Privacy Infrastructure (WAPI).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row725048837093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1105802477093521">

ETHER_LLTD_TYPE 0x88D9

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1983055545093521">

Indicates Link Layer Topology Discovery (LLTD).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1392396236093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1785402777093521">

ETHER_ONE_X_TYPE 0x888E

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1651545026093521">

Indicates 802.1x network port authentication.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1172446772093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1594873548093521">

ETHER_TUNNEL_TYPE 0x88bd

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1985428530093521">

Indicates a tunnel protocol.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row370903690093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2001610321093521">

ETHER_TYPE_PPP_DISC 0x8863

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p348416886093521">

Indicates the point-to-point discovery type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1926515533093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p578533525093521">

ETHER_TYPE_PPP_SES 0x8864

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p898005225093521">

Indicates the point-to-point session discovery type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row268838351093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1779077701093521">

ETHER_TYPE_6LO 0xa0ed

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p586284251093521">

Indicates IPv6 over Low Power Wireless Personal Area Networks
(6LoWPANs).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1208017563093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1193431732093521">

TCP_PROTOCAL 6

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1383076103093521">

Indicates the Transmission Control Protocol (TCP).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1143568423093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p60899522093521">

UDP_PROTOCAL 17

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1236389479093521">

Indicates the User Datagram Protocol (UDP).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2078644254093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p97102557093521">

IP_PRI_SHIFT 5

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p319058705093521">

Indicates the shift in the priority for an IP address.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1450368585093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p551835797093521">

DHCP_UDP_SRC_PORT 68

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p669729591093521">

Indicates the source port number of DHCP.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1743326274093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1937355145093521">

DHCP_UDP_DES_PORT 67

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p734714617093521">

Indicates the destination port number of DHCP.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row543065721093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1183168208093521">

MAX_WIFI_COMPONENT_NAME_LEN 10

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p698244150093521">

Indicates the length of the name of a WLAN module or feature.

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

Typedefs
--------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row465687364093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p419452486093521">

Typedef Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p654243286093521">

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

   <tr id="row1568214738093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p142774837093521">

NetDevice

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1039364600093521">

typedef struct NetDevice

.. raw:: html

   </p>

.. raw:: html

   <p id="p1537080684093521">

Defines a network device, including the network interface category and
name, and network port type.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1409654497093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p918392231093521">

WifiConnectParams

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p402750575093521">

typedef struct WifiConnectParams

.. raw:: html

   </p>

.. raw:: html

   <p id="p1852609873093521">

Describes parameters for a connection request.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row923041594093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1212697672093521">

Mac80211SetMacParam

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1987976822093521">

typedef struct MacConfigParam

.. raw:: html

   </p>

.. raw:: html

   <p id="p100148495093521">

Describes MAC configuration parameters.

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

Enumerations
------------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row47266118093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1471132972093521">

Enumeration Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1036952344093521">

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

   <tr id="row470408944093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1355484535093521">

{ E_HEAD_BUF, E_DATA_BUF, E_TAIL_BUF, MAX_BUF_NUM }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1657547095093521">

Enumerates the segments of a network data buffer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row29426973093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p663259643093521">

WifiHmacMgmtStatus { WIFI_HMAC_MGMT_SUCCESS = 0, WIFI_HMAC_MGMT_INVALID
= 1, WIFI_HMAC_MGMT_TIMEOUT = 2, WIFI_HMAC_MGMT_REFUSED = 3,
WIFI_HMAC_MGMT_TOMANY_REQ = 4, WIFI_HMAC_MGMT_ALREADY_BSS = 5 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1450413484093521">

Enumerates MLME management statuses, indicating whether a device is
successfully associated or fails to be associated.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1793707740093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2056402117093521">

NetIfCategory { LITE_OS, RICH_OS }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1935038812093521">

Enumerates network interface categories, including lightweight OS and
rich OS.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1213033164093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p918633897093521">

NetIfStatus { NETIF_DOWN, NETIF_UP }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p177656823093521">

Enumerates network interface states, including online and offline.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1760765565093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p767032602093521">

NetIfLinkStatus { NETIF_LINK_DOWN, NETIF_LINK_UP }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1058070066093521">

Enumerates network link layer states, including online and offline.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1908472106093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p421851969093521">

NetLinkType { ETHERNET_LINK = 1, WIFI_LINK = 801 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p151112515093521">

Enumerates data link types, including Ethernet and WLAN.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1207564794093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p169819401093521">

ProcessingResult { PROCESSING_CONTINUE, PROCESSING_COMPLETE,
PROCESSING_ERROR }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p996800055093521">

Enumerates data processing results, including continuing processing,
processing completed, and error.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1812503175093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1604297107093521">

NetDevTxResult { NETDEV_TX_OK = 0x00, NETDEV_TX_BUSY = 0x10,
NETDEV_TX_LOCKED = 0x20 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1003253902093521">

Enumerates data sending results, including sending succeeded, other data
being sent at the link layer, and data link layer being locked.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1265653315093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1563657357093521">

Protocol80211IfType { PROTOCOL_80211_IFTYPE_UNSPECIFIED,
PROTOCOL_80211_IFTYPE_ADHOC, PROTOCOL_80211_IFTYPE_STATION,
PROTOCOL_80211_IFTYPE_AP, PROTOCOL_80211_IFTYPE_AP_VLAN,
PROTOCOL_80211_IFTYPE_WDS, PROTOCOL_80211_IFTYPE_MONITOR,
PROTOCOL_80211_IFTYPE_MESH_POINT, PROTOCOL_80211_IFTYPE_P2P_CLIENT,
PROTOCOL_80211_IFTYPE_P2P_GO, PROTOCOL_80211_IFTYPE_P2P_DEVICE,
PROTOCOL_80211_IFTYPE_NUM, PROTOCOL_80211_IFTYPE_MAX =
PROTOCOL_80211_IFTYPE_NUM - 1 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p685018131093521">

Enumerates 802.11 network port types, including AP, STA, and P2P.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row821747608093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2026579277093521">

NetdeviceError { COMMON_ERROR = 1, ADD_LWIP_ERROR }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p33618155093521">

Enumerates network device errors, including common errors and errors in
adding network devices to LwIP.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1057432701093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p668185454093521">

WifiMainFeatureType { HDF_WIFI_FEATURE_BASE, HDF_WIFI_FEATURE_AP,
HDF_WIFI_FEATURE_STA, HDF_WIFI_FEATURE_P2P, HDF_WIFI_FEATURE_NAN,
HDF_WIFI_FEATURE_RTT, HDF_WIFI_FEATURE_NUM = 10 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2077284605093521">

Enumerates feature types of a WLAN module.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row941154127093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1603169460093521">

WifiBusType { BUS_SDIO, BUS_USB }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1007764691093521">

Enumerates bus types of a WLAN module.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1693309025093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p846911455093521">

MacSetType { MAC_BEACON_SET = 0, MAC_BEACON_ADD = 1 }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p864374947093521">

Enumerates setting types of MAC addresses.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row270298377093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p725404467093521">

Ieee80211Band { IEEE80211_BAND_2GHZ, IEEE80211_BAND_5GHZ,
IEEE80211_NUM_BANDS }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2127843697093521">

Enumerates frequency bands.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row719955940093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1044425748093521">

WifiChannelType { WIFI_CHAN_NO_HT, WIFI_CHAN_HT20, WIFI_CHAN_HT40MINUS,
WIFI_CHAN_HT40PLUS }

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2030739365093521">

Enumerates channel types.

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

Functions
---------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1228311346093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1990506584093521">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2016714892093521">

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

   <tr id="row1172179934093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1041829220093521">

NetBufQueueInit (struct NetBufQueue \*q)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1761467274093521">

static void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1727663347093521">

Initializes a network data buffer queue.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1757746216093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p578429419093521">

NetBufQueueSize (const struct NetBufQueue \*q)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1442318469093521">

static uint32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p519611596093521">

Obtains the size of a network data buffer queue.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1099568589093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p587840895093521">

NetBufQueueIsEmpty (const struct NetBufQueue \*q)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p971459071093521">

static bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p779681455093521">

Checks whether the network data buffer queue is empty.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row330341976093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1037040794093521">

NetBufQueueEnqueue (struct NetBufQueue *q, struct NetBuf*\ nb)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p127646759093521">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1442133646093521">

Adds a network data buffer to the tail of a queue.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row254440301093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p743317991093521">

NetBufQueueEnqueueHead (struct NetBufQueue *q, struct NetBuf*\ nb)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1302524806093521">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p103867253093521">

Adds a network data buffer to the header of a queue.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row732713374093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1816736128093521">

NetBufQueueDequeue (struct NetBufQueue \*q)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1692661162093521">

struct NetBuf \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1471119861093521">

Obtains a network data buffer from the header of a queue and deletes it
from the queue.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row750969027093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p394812196093521">

NetBufQueueDequeueTail (struct NetBufQueue \*q)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2001083061093521">

struct NetBuf \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1306070199093521">

Obtains a network data buffer from the tail of a queue and deletes it
from the queue.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row605952506093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2072947564093521">

NetBufQueueAtHead (const struct NetBufQueue \*q)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p119075106093521">

static struct NetBuf \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p306454845093521">

Obtains the network data buffer from the header of a queue, without
deleting it from the queue.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row823965366093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2129483619093521">

NetBufQueueAtTail (const struct NetBufQueue \*q)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2078064929093521">

static struct NetBuf \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p818595257093521">

Obtains the network data buffer from the tail of a queue, without
deleting it from the queue.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row524416759093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1323074702093521">

NetBufQueueClear (struct NetBufQueue \*q)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p675081390093521">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p173698392093521">

Clears a network data buffer queue and releases the network data buffer
in the queue.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row627415965093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p679222833093521">

NetBufQueueConcat (struct NetBufQueue *q, struct NetBufQueue*\ add)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1239149124093521">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p1497246071093521">

Moves all network data buffers from one queue to another and clears the
source queue.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row703606385093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p487709848093521">

NetBufAlloc (uint32_t size)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1006391281093521">

struct NetBuf \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1599477929093521">

Applies for a network data buffer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2101944564093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p121274916093521">

NetBufFree (struct NetBuf \*nb)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p63325763093521">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p111485937093521">

Releases a network data buffer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1301363920093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1824349471093521">

NetBufDevAlloc (const struct NetDevice \*dev, uint32_t size)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p883645570093521">

struct NetBuf \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p929807968093521">

Applies for a network data buffer based on the reserved space and
requested size set by a network device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1054490466093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2093576294093521">

NetBufPush (struct NetBuf \*nb, uint32_t id, uint32_t len)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1448422674093521">

void \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1907417353093521">

Performs operations based on the segment ID of a network data buffer.
The function is opposite to that of NetBufPop.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row829462990093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1031076855093521">

NetBufPop (struct NetBuf \*nb, uint32_t id, uint32_t len)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p245156383093521">

void \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p505862275093521">

Performs operations based on the segment ID of a network data buffer.
The function is opposite to that of NetBufPush.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row235553937093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1614004407093521">

NetBufGetAddress (const struct NetBuf \*nb, uint32_t id)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1313014605093521">

static uint8_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p460413966093521">

Obtains the address of a specified buffer segment in a network data
buffer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row50176012093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p885515382093521">

NetBufGetRoom (const struct NetBuf \*nb, uint32_t id)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p126898862093521">

static uint32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1554289260093521">

Obtains the size of a specified buffer segment space in a network data
buffer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1032119191093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1001053966093521">

NetBufGetDataLen (const struct NetBuf \*nb)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p657293862093521">

static uint32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1135016725093521">

Obtains the actual data length of the data segment of a network data
buffer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row990209999093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1090120521093521">

NetBufResizeRoom (struct NetBuf \*nb, uint32_t head, uint32_t tail)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p876015807093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1351053307093521">

Adjusts the size of a network data buffer space.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1851876020093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p292465023093521">

NetBufConcat (struct NetBuf *nb, struct NetBuf*\ cnb)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1250549596093521">

uint32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p879172756093521">

Copies data in a network data buffer to another network data buffer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1959232713093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1261132347093521">

Pbuf2NetBuf (const struct NetDevice *netdev, struct pbuf*\ lwipBuf)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1270730961093521">

struct NetBuf \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1429148077093521">

Converts the pbuf structure of Lightweight TCP/IP Stack (lwIP) to a
network data buffer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row326043789093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1854412346093521">

NetBuf2Pbuf (const struct NetBuf \*nb)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1401274633093521">

struct pbuf \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p897481766093521">

Converts a network data buffer to the pbuf structure of Lightweight
TCP/IP Stack (lwIP).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1574996814093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p512686373093521">

HdfWifiEventNewSta (const struct NetDevice *netdev, const
uint8_t*\ macAddr, uint8_t addrLen, const struct StationInfo \*info)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1046534888093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1917171674093521">

Reports a new STA event.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1645716193093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p799312194093521">

HdfWifiEventDelSta (struct NetDevice *netdev, const uint8_t*\ macAddr,
uint8_t addrLen)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p401214443093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1262505567093521">

Reports a station deletion event.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1933732479093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1236306042093521">

HdfWifiEventInformBssFrame (const struct NetDevice *netdev, struct
Wiphy*\ wiphy, const struct Ieee80211Channel *channel, const struct
ScannedBssInfo*\ bssInfo)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p715230324093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1810299202093521">

Reports a scanned BSS event.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1583428152093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p561617226093521">

HdfWifiEventScanDone (const struct NetDevice \*netdev, WifiScanStatus
status)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p189139132093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p39897097093521">

Reports a scanning completion event.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row282411226093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p118645482093521">

HdfWifiEventConnectResult (const struct NetDevice *netdev, const struct
ConnetResult*\ result)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p719186189093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1949441085093521">

Reports a connection result event.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1095732710093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1840125546093521">

HdfWifiEventDisconnected (const struct NetDevice *netdev, uint16_t
reason, const uint8_t*\ ie, uint32_t len)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1004246645093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1435835938093521">

Reports a disconnection event.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1390029008093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p29436192093521">

HdfWifiEventMgmtTxStatus (const struct NetDevice *netdev, const
uint8_t*\ buf, size_t len, uint8_t ack)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1571325431093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p801868334093521">

Reports a transmission management status event.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1779273510093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1111819439093521">

HdfWifiEventRxMgmt (const struct NetDevice *netdev, int32_t freq,
int32_t sigMbm, const uint8_t*\ buf, size_t len)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1019804505093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2128737331093521">

Reports a receive management status event.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1508932370093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p193707196093521">

HdfWifiEventCsaChannelSwitch (const struct NetDevice \*netdev, int32_t
freq)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p440754013093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p829173394093521">

Reports a CSA channel switching event.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row507555899093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p381556975093521">

HdfWifiEventTimeoutDisconnected (const struct NetDevice \*netdev)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p465658564093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1688316156093521">

Reports a timeout disconnection event.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1310636618093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p199980058093521">

HdfWifiEventEapolRecv (const char *name, void*\ context)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p55093159093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2074704241093521">

Reports the event of receiving the EAPOL frame and notifies WPA to read
the EAPOL frame.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2015049930093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1746488581093521">

HdfWifiGetProduct (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p4003282093521">

struct HdfWifiProductData \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p146848687093521">

Obtains the data structure of the WLAN module.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1589134771093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p994803968093521">

NetDeviceInit (const char \*ifName, uint32_t len, NetIfCategory
ifCategory)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1905855227093521">

struct NetDevice \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1423255259093521">

Initializes a network device to obtain its instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1458181529093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1459660575093521">

NetDeviceDeInit (struct NetDevice \*netDevice)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p901379630093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1427394767093521">

Deletes a network device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1196890058093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1357135570093521">

NetDeviceAdd (struct NetDevice \*netDevice, Protocol80211IfType ifType)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p187829460093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p816907797093521">

Adds a network device to a protocol stack.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1850795038093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p237821364093521">

NetDeviceDelete (struct NetDevice \*netDevice)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p481525306093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p489335232093521">

Deletes a network device from a protocol stack.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row709922679093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p405789169093521">

NetDeviceGetInstByName (const char \*name)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1892435453093521">

struct NetDevice \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p777356534093521">

Obtains the initialized network device instance by a specified device
name.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row747642188093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p297609515093521">

NetDeviceIsAnyInstRunning (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p250349330093521">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p943633783093521">

Checks whether there are working devices among the added network
devices.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row814780554093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p251528639093521">

NetDeviceIsInstRunning (const struct NetDevice \*netDevice)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p508584472093521">

bool

.. raw:: html

   </p>

.. raw:: html

   <p id="p511484107093521">

Checks whether a specified network device is working.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row877989583093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p309926306093521">

NetDevGetRegisterCount (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1206029696093521">

uint32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1863343755093521">

Obtains the number of added network devices.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row223403520093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1993915959093521">

NetDeviceGetCap (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p884517227093521">

uint32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1386817111093521">

Obtains the maximum number of network devices that can be registered
with this system at the same time.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row742954852093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p911964370093521">

NetDeviceGetInstByIndex (uint32_t index)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p282054325093521">

struct NetDevice \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1112135311093521">

Obtains a network device instance based on the index number.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1423922963093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p180078122093521">

NetIfSetAddr (const struct NetDevice *netDevice, const
IpV4Addr*\ ipAddr, const IpV4Addr *netMask, const IpV4Addr*\ gw)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p88184170093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p75554033093521">

Sets an IP address, mask, and gateway.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row26028279093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1735012287093521">

NetIfSetStatus (const struct NetDevice \*netDevice, NetIfStatus status)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1864847115093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1857294969093521">

Notifies the network layer of the network port state.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row352133590093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1315213453093521">

NetIfSetLinkStatus (const struct NetDevice \*netDevice, NetIfLinkStatus
status)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p195744094093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1130398578093521">

Notifies the network layer of the data link layer status.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1441290863093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1618638868093521">

NetIfRx (const struct NetDevice *netDevice, struct NetBuf*\ buff)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1449528246093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p82879894093521">

Transfers the input data packets from the network side to a protocol
stack.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row609822992093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1437767928093521">

NetIfRxNi (const struct NetDevice *netDevice, struct NetBuf*\ buff)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1635739556093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1156377006093521">

Transfers data packets from the network side to a protocol stack in an
interrupt processing thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1099706215093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1077345427093521">

NetIfDhcpsStart (const struct NetDevice *netDevice, char*\ ip, u16_t
ipNum)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1840521348093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1628306813093521">

Starts the DHCP server.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2016377745093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p421145935093521">

NetIfDhcpsStop (const struct NetDevice \*netDevice)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1933141720093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1040106776093521">

Stops the DHCP server.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1197075281093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p23140220093521">

NetIfDhcpStart (const struct NetDevice \*netDevice)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1650396600093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1469739850093521">

Starts the DHCP client of a specified network device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1337981515093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1642046503093521">

NetIfDhcpStop (const struct NetDevice \*netDevice)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1213604150093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p185775338093521">

Stops the DHCP client of a specified network device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row17027514093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1022695846093521">

NetIfDhcpIsBound (const struct NetDevice \*netDevice)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1345346172093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p387834428093521">

Obtains the DHCP negotiation status of a specified network device.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1725271986093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p711535678093521">

Mac80211RegisterOps (struct WifiMac80211Ops \*ops)
**attribute**\ ((weak))

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1215674827093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p504765107093521">

Registers a WifiMac80211Ops object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1122515026093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2064211195093521">

Mac80211GetOps (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p706185208093521">

struct WifiMac80211Ops \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p106672644093521">

Obtains the WifiMac80211Ops object that the driver needs to implement.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1464347599093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2022805102093521">

WifiModuleCreate (const struct HdfConfigWifiModuleConfig \*config)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1104057225093521">

struct WifiModule \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1664093975093521">

Creates a WifiModule object based on a specified configuration generated
by the HCS.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row251125321093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1692598161093521">

WifiModuleDelete (struct WifiModule \*module)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1650155998093521">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p683862233093521">

Deletes a specified WifiModule object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2128838059093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1144490919093521">

DelFeature (struct WifiModule \*module, uint16_t featureType)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p914309682093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2097257917093521">

Deletes a specified feature from a specified module.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row891044029093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p255562441093521">

AddFeature (struct WifiModule *module, uint16_t featureType, struct
WifiFeature*\ featureData)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1077873769093521">

int32_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p315613239093521">

Adds a specified feature to a specified module.

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

**Macro Definition Documentation**\ 
------------------------------------

MAX_NETBUF_RESEVER_SIZE
-----------------------

::

   #define MAX_NETBUF_RESEVER_SIZE   68

**Description:**

Defines the reserved field of a network data buffer used to store
private information.

The length of the reserved field is **68** bytes.

MAX_WIFI_COMPONENT_NAME_LEN
---------------------------

::

   #define MAX_WIFI_COMPONENT_NAME_LEN   10

**Description:**

Indicates the length of the name of a WLAN module or feature.

The name of a WLAN module or feature cannot contain more than 10
characters; otherwise, the name will be truncated and cannot be
identified.

**Typedef Documentation**\ 
---------------------------

Mac80211SetMacParam
-------------------

::

   typedef struct [MacConfigParam](macconfigparam.md) [Mac80211SetMacParam](wlan.md#ga7566bdca5b1746ade791cd7f863f259b)

**Description:**

Describes MAC configuration parameters.

NetDevice
---------

::

   typedef struct [NetDevice](netdevice.md) [NetDevice](netdevice.md)

**Description:**

Defines a network device, including the network interface category and
name, and network port type.

WifiConnectParams
-----------------

::

   typedef struct [WifiConnectParams](wificonnectparams.md) [WifiConnectParams](wificonnectparams.md)

**Description:**

Describes parameters for a connection request.

**Enumeration Type Documentation**\ 
------------------------------------

anonymous enum
--------------

::

   anonymous enum

**Description:**

Enumerates the segments of a network data buffer.

The entire network data buffer is divided into three segments: a header,
data, and a tail. The header and tail are used to extend both ends of
the data segment.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1806646344093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p903721083093521">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p331630330093521">

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

   <tr id="row542284840093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

E_HEAD_BUF

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1451425088093521">

Header buffer segment

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1648146501093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

E_DATA_BUF

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2086742335093521">

Data segment

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1744176404093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

E_TAIL_BUF

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1217194313093521">

Tail buffer segment

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row657945902093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

MAX_BUF_NUM

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p582757883093521">

Maximum number of buffer segments

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

Ieee80211Band
-------------

::

   enum [Ieee80211Band](wlan.md#ga9882f415202cf9acb0f4cdfbc456a88d)

**Description:**

Enumerates frequency bands.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row154181429093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p150350491093521">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2143062267093521">

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

   <tr id="row1816291132093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

IEEE80211_BAND_2GHZ

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p38747768093521">

2.4 GHz

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1685190181093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

IEEE80211_BAND_5GHZ

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p342570824093521">

5 GHz

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row629812677093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

IEEE80211_NUM_BANDS

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p865169517093521">

Reserved

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

MacSetType
----------

::

   enum [MacSetType](wlan.md#ga75cba3dc6ab4c5dc5653b037433b3abf)

**Description:**

Enumerates setting types of MAC addresses.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row762617112093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p679397358093521">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p234655586093521">

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

   <tr id="row1962412968093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

MAC_BEACON_SET

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p914870305093521">

Setting a beacon MAC address

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row320839631093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

MAC_BEACON_ADD

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p649273566093521">

Adding a beacon MAC address

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

NetdeviceError
--------------

::

   enum [NetdeviceError](wlan.md#ga9023c5dc1cc43758cbb468d78af41c2d)

**Description:**

Enumerates network device errors, including common errors and errors in
adding network devices to LwIP.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row339601340093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1905455754093521">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1119760703093521">

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

   <tr id="row131239671093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

COMMON_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1482068923093521">

Common errors

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row220737829093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ADD_LWIP_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1978991193093521">

Errors in adding network devices to LwIP

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

NetDevTxResult
--------------

::

   enum [NetDevTxResult](wlan.md#ga9fb4e578a15db1b0087d7b3831591ced)

**Description:**

Enumerates data sending results, including sending succeeded, other data
being sent at the link layer, and data link layer being locked.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row244395215093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1203260932093521">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p825510408093521">

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

   <tr id="row920638271093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

NETDEV_TX_OK

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1238869494093521">

Sending succeeded

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1786579093093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

NETDEV_TX_BUSY

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p710233763093521">

Other data being sent at the link layer

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1454764626093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

NETDEV_TX_LOCKED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p564892211093521">

Data link layer being locked

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

NetIfCategory
-------------

::

   enum [NetIfCategory](wlan.md#ga530241881cd17e03f8ae254ef1d9755e)

**Description:**

Enumerates network interface categories, including lightweight OS and
rich OS.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row458106973093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p278169805093521">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1093888475093521">

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

   <tr id="row698391390093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

LITE_OS

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p99631684093521">

Lightweight OS

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row576248235093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

RICH_OS

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1116809833093521">

Rich OS

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

NetIfLinkStatus
---------------

::

   enum [NetIfLinkStatus](wlan.md#ga7b1187d116fb065d7927ad9f77edd842)

**Description:**

Enumerates network link layer states, including online and offline.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1805456246093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p331247549093521">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p312900299093521">

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

   <tr id="row1547021336093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

NETIF_LINK_DOWN

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p386752832093521">

Data link offline

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row427585432093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

NETIF_LINK_UP

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p82975331093521">

Data link online

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

NetIfStatus
-----------

::

   enum [NetIfStatus](wlan.md#ga0fb482694e5eac3f48c75de1749c8baf)

**Description:**

Enumerates network interface states, including online and offline.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1867225283093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1711428941093521">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p584263779093521">

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

   <tr id="row360261732093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

NETIF_DOWN

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1805429628093521">

Network interface offline

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1720369704093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

NETIF_UP

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1834971342093521">

Network interface online

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

NetLinkType
-----------

::

   enum [NetLinkType](wlan.md#gad3175955d2e6ef3c4f52da9b509d5b4a)

**Description:**

Enumerates data link types, including Ethernet and WLAN.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row615447602093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p79266673093521">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p668667416093521">

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

   <tr id="row1562107078093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ETHERNET_LINK

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p243757955093521">

Ethernet

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row982930038093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

WIFI_LINK

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1068227787093521">

WLAN

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

ProcessingResult
----------------

::

   enum [ProcessingResult](wlan.md#ga9c1d6e7df4468671742cb76f72b67af1)

**Description:**

Enumerates data processing results, including continuing processing,
processing completed, and error.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1824838084093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1066192366093521">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1609971427093521">

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

   <tr id="row1227467935093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PROCESSING_CONTINUE

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p96774376093521">

Continuing processing

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row656023324093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PROCESSING_COMPLETE

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1692358555093521">

Processing completed

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row810391378093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PROCESSING_ERROR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1579057167093521">

Error

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

Protocol80211IfType
-------------------

::

   enum [Protocol80211IfType](wlan.md#gac69954f56fcc99fc8aac68aa157831c7)

**Description:**

Enumerates 802.11 network port types, including AP, STA, and P2P.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1573445406093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2077197447093521">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1228497481093521">

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

   <tr id="row226219292093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PROTOCOL_80211_IFTYPE_UNSPECIFIED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1948374194093521">

Unspecified

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1530670496093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PROTOCOL_80211_IFTYPE_ADHOC

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p519375832093521">

Ad hoc network

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1470321168093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PROTOCOL_80211_IFTYPE_STATION

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p376041540093521">

Workstation

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1395376328093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PROTOCOL_80211_IFTYPE_AP

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p431800521093521">

Access point

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1955354528093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PROTOCOL_80211_IFTYPE_AP_VLAN

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p504549818093521">

Virtual access point

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row928613527093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PROTOCOL_80211_IFTYPE_WDS

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2011324635093521">

Wireless distributed system

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1119611424093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PROTOCOL_80211_IFTYPE_MONITOR

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1810112351093521">

Listening

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1694656626093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PROTOCOL_80211_IFTYPE_MESH_POINT

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p276218238093521">

Mesh network

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row378670998093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PROTOCOL_80211_IFTYPE_P2P_CLIENT

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1057673507093521">

P2P client

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row817395857093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PROTOCOL_80211_IFTYPE_P2P_GO

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2019891554093521">

P2P group owner

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1677267100093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PROTOCOL_80211_IFTYPE_P2P_DEVICE

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p376066847093521">

P2P device

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1392039713093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PROTOCOL_80211_IFTYPE_NUM

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1825873220093521">

Number of network ports

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row186381935093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

PROTOCOL_80211_IFTYPE_MAX

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1374689110093521">

Maximum number of 802.11 network port types

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

WifiBusType
-----------

::

   enum [WifiBusType](wlan.md#ga1c5537e64f05b5e91b951ddeb66d4261)

**Description:**

Enumerates bus types of a WLAN module.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row236613177093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p791065869093521">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1829950319093521">

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

   <tr id="row472481021093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

BUS_SDIO

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1815612852093521">

Secure Digital Input and Output (SDIO)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1675389345093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

BUS_USB

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p562561643093521">

Universal Serial Bus (USB)

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

WifiChannelType
---------------

::

   enum [WifiChannelType](wlan.md#ga9d902b330de99c24b2a8c3ba7120af21)

**Description:**

Enumerates channel types.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1525883792093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p512336604093521">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p353928045093521">

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

   <tr id="row1732701847093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

WIFI_CHAN_NO_HT

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1195354648093521">

non-HT channel

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1705715326093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

WIFI_CHAN_HT20

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p241215968093521">

20 MHz HT channel

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row196783670093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

WIFI_CHAN_HT40MINUS

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p829591569093521">

40 MHz minus HT channel (The channel is formed by two 20 MHz HT
channels, one as the main channel and the other as the auxiliary
channel. The center frequency of the main channel is lower than that of
the auxiliary channel.)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1958896954093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

WIFI_CHAN_HT40PLUS

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2045909819093521">

40 MHz plus HT channel (The channel is formed by two 20 MHz HT channels,
one as the main channel and the other as the auxiliary channel. The
center frequency of the main channel is higher than that of the
auxiliary channel.)

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

WifiHmacMgmtStatus
------------------

::

   enum [WifiHmacMgmtStatus](wlan.md#gaf3e873b51f0cfa077aca9d33ed7a0960)

**Description:**

Enumerates MLME management statuses, indicating whether a device is
successfully associated or fails to be associated.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row400515872093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p914555485093521">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2080354147093521">

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

   <tr id="row1817205183093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

WIFI_HMAC_MGMT_SUCCESS

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p504183547093521">

Association succeeds

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row864176620093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

WIFI_HMAC_MGMT_INVALID

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1942525087093521">

Association fails

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1133680492093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

WIFI_HMAC_MGMT_TIMEOUT

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1066537876093521">

Association timeout

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1079293262093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

WIFI_HMAC_MGMT_REFUSED

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p100557891093521">

Association refused

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row962386272093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

WIFI_HMAC_MGMT_TOMANY_REQ

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p975416148093521">

Repeated association request

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1841820047093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

WIFI_HMAC_MGMT_ALREADY_BSS

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p233776757093521">

Associated with the BSS

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

WifiMainFeatureType
-------------------

::

   enum [WifiMainFeatureType](wlan.md#gaec03ba36d71cc2d5f3209bc24aa6ee10)

**Description:**

Enumerates feature types of a WLAN module.

You can query and register a feature or bind a feature to a WLAN module
based on the feature type.

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row860898724093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p957982135093521">

Enumerator

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p598983309093521">

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

   <tr id="row107611194093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

HDF_WIFI_FEATURE_BASE

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p936358479093521">

Base feature

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1971364312093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

HDF_WIFI_FEATURE_AP

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p259379632093521">

AP

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1446469009093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

HDF_WIFI_FEATURE_STA

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1317588320093521">

Station

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row176301300093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

HDF_WIFI_FEATURE_P2P

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p809617792093521">

Peer-to-peer (P2P)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row567573730093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

HDF_WIFI_FEATURE_NAN

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p64385124093521">

Neighbor Awareness Networking (NAN)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1964508410093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

HDF_WIFI_FEATURE_RTT

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1681634762093521">

Round Trip Time (RTT)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1481462785093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

HDF_WIFI_FEATURE_NUM

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2118167948093521">

Maximum number of features

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

**Function Documentation**\ 
----------------------------

AddFeature()
------------

::

   int32_t AddFeature (struct [WifiModule](wifimodule.md) * module, uint16_t featureType, struct [WifiFeature](wififeature.md) * featureData )

**Description:**

Adds a specified feature to a specified module.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1808298923093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1348652969093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p852194851093521">

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

   <tr id="row928235947093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

module

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the module.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row90262712093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

featureType

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the type of the feature to add.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row628353818093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

featureData

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the feature to add.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the feature is added successfully; returns a negative
value otherwise.

DelFeature()
------------

::

   int32_t DelFeature (struct [WifiModule](wifimodule.md) * module, uint16_t featureType )

**Description:**

Deletes a specified feature from a specified module.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row740219164093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1261015331093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p191973933093521">

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

   <tr id="row829395008093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

module

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the module.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row560063897093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

featureType

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the type of the feature to delete.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the feature is deleted successfully; returns **-1**
otherwise.

HdfWifiEventConnectResult()
---------------------------

::

   int32_t HdfWifiEventConnectResult (const struct [NetDevice](netdevice.md) * netdev, const struct [ConnetResult](connetresult.md) * result )

**Description:**

Reports a connection result event.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row726428029093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1384116436093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p537520660093521">

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

   <tr id="row961151239093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netdev

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device. This parameter cannot be
null.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row365937211093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

result

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the connection result. This parameter cannot be
null.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the event is reported successfully; returns **-1**
otherwise.

HdfWifiEventCsaChannelSwitch()
------------------------------

::

   int32_t HdfWifiEventCsaChannelSwitch (const struct [NetDevice](netdevice.md) * netdev, int32_t freq )

**Description:**

Reports a CSA channel switching event.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row217858320093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1937590248093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1702908022093521">

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

   <tr id="row1130882045093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netdev

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device. This parameter cannot be
null.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1440862386093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

freq

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the frequency of the channel.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the event is reported successfully; returns **-1**
otherwise.

HdfWifiEventDelSta()
--------------------

::

   int32_t HdfWifiEventDelSta (struct [NetDevice](netdevice.md) * netdev, const uint8_t * macAddr, uint8_t addrLen )

**Description:**

Reports a station deletion event.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1599435850093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p215254924093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1902793618093521">

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

   <tr id="row863080887093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netdev

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device. This parameter cannot be
null.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1317007890093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

macAddr

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the MAC address of the station. This parameter
cannot be null.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1498278728093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

addrLen

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the length of the MAC address of the station. The length is
fixed to six bytes.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the event is reported successfully; returns **-1**
otherwise.

HdfWifiEventDisconnected()
--------------------------

::

   int32_t HdfWifiEventDisconnected (const struct [NetDevice](netdevice.md) * netdev, uint16_t reason, const uint8_t * ie, uint32_t len )

**Description:**

Reports a disconnection event.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1902493221093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1753070416093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p832651700093521">

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

   <tr id="row675255926093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netdev

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device. This parameter cannot be
null.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row528779845093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

reason

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the reason for disconnection.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1516504320093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ie

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the deauth/disassoc frame IE.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row639349531093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ieLen

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the length of the deauth/disassoc IE.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the event is reported successfully; returns **-1**
otherwise.

HdfWifiEventEapolRecv()
-----------------------

::

   int32_t HdfWifiEventEapolRecv (const char * name, void * context )

**Description:**

Reports the event of receiving the EAPOL frame and notifies WPA to read
the EAPOL frame.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row56375458093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2062060520093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p270602851093521">

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

   <tr id="row297016750093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

name

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network port name, for example, wlan0.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row959628190093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

context

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the context. This parameter is reserved.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns **-1** otherwise.

HdfWifiEventInformBssFrame()
----------------------------

::

   int32_t HdfWifiEventInformBssFrame (const struct [NetDevice](netdevice.md) * netdev, struct [Wiphy](wiphy.md) * wiphy, const struct [Ieee80211Channel](ieee80211channel.md) * channel, const struct [ScannedBssInfo](scannedbssinfo.md) * bssInfo )

**Description:**

Reports a scanned BSS event.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row135939546093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1908723012093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1377333254093521">

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

   <tr id="row719238104093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netdev

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device. This parameter cannot be
null.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row742208024093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

wiphy

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the physical layer of the wireless network.
This parameter cannot be null.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2020726605093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

channel

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the channel information. This parameter cannot
be null.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row265629573093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

bssInfo

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the BSS information. This parameter cannot be
null.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the event is reported successfully; returns **-1**
otherwise.

HdfWifiEventMgmtTxStatus()
--------------------------

::

   int32_t HdfWifiEventMgmtTxStatus (const struct [NetDevice](netdevice.md) * netdev, const uint8_t * buf, size_t len, uint8_t ack )

**Description:**

Reports a transmission management status event.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1526043558093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2117355258093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p548251802093521">

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

   <tr id="row2092149100093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netdev

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device. This parameter cannot be
null.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row314892892093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

buf

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the transmission management frame. This
parameter cannot be null.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1412628230093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

len

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the length of the transmission management frame.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row489215205093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ack

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates whether the transmission management frame is acknowledged.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the event is reported successfully; returns **-1**
otherwise.

HdfWifiEventNewSta()
--------------------

::

   int32_t HdfWifiEventNewSta (const struct [NetDevice](netdevice.md) * netdev, const uint8_t * macAddr, uint8_t addrLen, const struct [StationInfo](stationinfo.md) * info )

**Description:**

Reports a new STA event.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1272346781093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p773405791093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1186669938093521">

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

   <tr id="row230465345093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netdev

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device. This parameter cannot be
null.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1625045131093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

macAddr

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the MAC address of the station. This parameter
cannot be null.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row956991956093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

addrLen

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the length of the MAC address of the station. The length is
fixed to six bytes.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1748005194093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

info

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the station information.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the event is reported successfully; returns **-1**
otherwise.

HdfWifiEventRxMgmt()
--------------------

::

   int32_t HdfWifiEventRxMgmt (const struct [NetDevice](netdevice.md) * netdev, int32_t freq, int32_t sigMbm, const uint8_t * buf, size_t len )

**Description:**

Reports a receive management status event.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row626997831093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p958228739093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1864952029093521">

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

   <tr id="row1843099401093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netdev

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device. This parameter cannot be
null.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1148133840093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

freq

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the frequency of receiving management frame.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2046470346093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

sigMbm

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the signal strength (in dBm).

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2099328349093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

buf

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the receive management frame. This parameter
cannot be null.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1407153518093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

len

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the length of the receive management frame.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the event is reported successfully; returns **-1**
otherwise.

HdfWifiEventScanDone()
----------------------

::

   int32_t HdfWifiEventScanDone (const struct [NetDevice](netdevice.md) * netdev, WifiScanStatus status )

**Description:**

Reports a scanning completion event.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1259321871093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p895049930093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1651525782093521">

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

   <tr id="row1660831962093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netdev

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device. This parameter cannot be
null.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row253325533093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

status

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the scanning completion status. Value 0 indicates that the
scanning is successful, and other values indicate that the scanning
fails.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the event is reported successfully; returns **-1**
otherwise.

HdfWifiEventTimeoutDisconnected()
---------------------------------

::

   int32_t HdfWifiEventTimeoutDisconnected (const struct [NetDevice](netdevice.md) * netdev)

**Description:**

Reports a timeout disconnection event.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row526270040093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p258112072093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p326955896093521">

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

   <tr id="row1930365578093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netdev

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device. This parameter cannot be
null.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the event is reported successfully; returns **-1**
otherwise.

HdfWifiGetProduct()
-------------------

::

   struct [HdfWifiProductData](hdfwifiproductdata.md)* HdfWifiGetProduct (void )

**Description:**

Obtains the data structure of the WLAN module.

**Returns:**

Returns the pointer to the data structure of the WLAN module. For
details, see `HdfWifiProductData <hdfwifiproductdata.md>`__.

Mac80211GetOps()
----------------

::

   struct [WifiMac80211Ops](wifimac80211ops.md)* Mac80211GetOps (void )

**Description:**

Obtains the `WifiMac80211Ops <wifimac80211ops.md>`__ object that the
driver needs to implement.

**Returns:**

Returns the pointer to the `WifiMac80211Ops <wifimac80211ops.md>`__
object.

Mac80211RegisterOps()
---------------------

::

   int32_t Mac80211RegisterOps (struct [WifiMac80211Ops](wifimac80211ops.md) * ops)

**Description:**

Registers a `WifiMac80211Ops <wifimac80211ops.md>`__ object.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1720582211093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1540205708093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p552405628093521">

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

   <tr id="row1410454519093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ops

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the WifiMac80211Ops object to register.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the `WifiMac80211Ops <wifimac80211ops.md>`__ object is
registered successfully; returns a non-zero value otherwise.

NetBuf2Pbuf()
-------------

::

   struct pbuf* NetBuf2Pbuf (const struct [NetBuf](netbuf.md) * nb)

**Description:**

Converts a network data buffer to the **pbuf** structure of Lightweight
TCP/IP Stack (lwIP).

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row726041384093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1120064323093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p362130203093521">

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

   <tr id="row1513903190093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

nb

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the pointer to the **pbuf** structure if the operation is
successful; returns **NULL** otherwise.

NetBufAlloc()
-------------

::

   struct [NetBuf](netbuf.md)* NetBufAlloc (uint32_t size)

**Description:**

Applies for a network data buffer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row742747106093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p151554905093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1081697090093521">

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

   <tr id="row1635135197093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

size

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the size of the network data buffer.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the pointer to the network data buffer if the operation is
successful; returns **NULL** otherwise.

NetBufConcat()
--------------

::

   uint32_t NetBufConcat (struct [NetBuf](netbuf.md) * nb, struct [NetBuf](netbuf.md) * cnb )

**Description:**

Copies data in a network data buffer to another network data buffer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1761795278093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2124668964093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1873952332093521">

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

   <tr id="row727072715093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

nb

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row225865543093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

cnb

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the target network data buffer.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a non-zero value
otherwise.

NetBufDevAlloc()
----------------

::

   struct [NetBuf](netbuf.md)* NetBufDevAlloc (const struct [NetDevice](netdevice.md) * dev, uint32_t size )

**Description:**

Applies for a network data buffer based on the reserved space and
requested size set by a network device.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1707543862093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p692893534093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1185569342093521">

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

   <tr id="row1338449080093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

dev

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row911260291093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

size

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the size of the network data buffer applied.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the pointer to the network data buffer if the operation is
successful; returns **NULL** otherwise.

NetBufFree()
------------

::

   void NetBufFree (struct [NetBuf](netbuf.md) * nb)

**Description:**

Releases a network data buffer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2082237640093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p841679657093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p493381138093521">

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

   <tr id="row1112433826093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

nb

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

NetBufGetAddress()
------------------

::

   static uint8_t* NetBufGetAddress (const struct [NetBuf](netbuf.md) * nb, uint32_t id )

**Description:**

Obtains the address of a specified buffer segment in a network data
buffer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row821974717093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p974844088093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2137978139093521">

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

   <tr id="row536547635093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

nb

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row783404718093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

id

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the buffer segment ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the address of the specified buffer segment if the operation is
successful; returns **NULL** if the buffer segment ID is invalid.

NetBufGetDataLen()
------------------

::

   static uint32_t NetBufGetDataLen (const struct [NetBuf](netbuf.md) * nb)

**Description:**

Obtains the actual data length of the data segment of a network data
buffer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row34591743093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p594461061093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p730956515093521">

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

   <tr id="row1730839066093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

nb

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the actual data length of the data segment.

NetBufGetRoom()
---------------

::

   static uint32_t NetBufGetRoom (const struct [NetBuf](netbuf.md) * nb, uint32_t id )

**Description:**

Obtains the size of a specified buffer segment space in a network data
buffer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row93095495093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2134701935093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1651006067093521">

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

   <tr id="row1663208519093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

nb

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row620915336093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

id

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the buffer segment ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the size of the specified buffer segment space if the operation
is successful; returns **NULL** if the buffer segment ID is invalid.

NetBufPop()
-----------

::

   void* NetBufPop (struct [NetBuf](netbuf.md) * nb, uint32_t id, uint32_t len )

**Description:**

Performs operations based on the segment ID of a network data buffer.
The function is opposite to that of
`NetBufPush <wlan.md#gac4ec1cedef616e61038dcb6dbf67d204>`__.

Description:

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1441774830093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1714769449093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1705337010093521">

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

   <tr id="row128738774093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

nb

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1321462384093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

id

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the buffer segment ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row114417652093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

len

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the operation length.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the start address of the data segment if the operation is
successful; returns **NULL** if the operation length exceeds the space
of a specified buffer segment.

NetBufPush()
------------

::

   void* NetBufPush (struct [NetBuf](netbuf.md) * nb, uint32_t id, uint32_t len )

**Description:**

Performs operations based on the segment ID of a network data buffer.
The function is opposite to that of
`NetBufPop <wlan.md#ga81f298aebc5b7772f173e2f6fadc004f>`__.

Description:

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row72155362093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p210244346093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1275489117093521">

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

   <tr id="row1581023756093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

nb

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1642011461093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

id

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the buffer segment ID.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row69060145093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

len

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the operation length.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the start address of the data segment if the operation is
successful; returns **NULL** if the operation length exceeds the space
of a specified buffer segment.

NetBufQueueAtHead()
-------------------

::

   static struct [NetBuf](netbuf.md)* NetBufQueueAtHead (const struct [NetBufQueue](netbufqueue.md) * q)

**Description:**

Obtains the network data buffer from the header of a queue, without
deleting it from the queue.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2131735472093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p106146710093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p801377777093521">

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

   <tr id="row858849298093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

q

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer queue.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the pointer to the first network data buffer if the queue is not
empty; returns **NULL** otherwise.

NetBufQueueAtTail()
-------------------

::

   static struct [NetBuf](netbuf.md)* NetBufQueueAtTail (const struct [NetBufQueue](netbufqueue.md) * q)

**Description:**

Obtains the network data buffer from the tail of a queue, without
deleting it from the queue.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1835459915093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p827637128093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2045578645093521">

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

   <tr id="row15290992093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

q

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer queue.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the pointer to the last network data buffer if the queue is not
empty; returns **NULL** otherwise.

NetBufQueueClear()
------------------

::

   void NetBufQueueClear (struct [NetBufQueue](netbufqueue.md) * q)

**Description:**

Clears a network data buffer queue and releases the network data buffer
in the queue.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row953253645093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1005269646093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p340696312093521">

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

   <tr id="row340238216093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

q

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer queue.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

NetBufQueueConcat()
-------------------

::

   void NetBufQueueConcat (struct [NetBufQueue](netbufqueue.md) * q, struct [NetBufQueue](netbufqueue.md) * add )

**Description:**

Moves all network data buffers from one queue to another and clears the
source queue.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row892886884093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1539723635093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p474996512093521">

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

   <tr id="row667002347093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

q

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the target network data buffer queue.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row196527782093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

add

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the source network data buffer queue.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

NetBufQueueDequeue()
--------------------

::

   struct [NetBuf](netbuf.md)* NetBufQueueDequeue (struct [NetBufQueue](netbufqueue.md) * q)

**Description:**

Obtains a network data buffer from the header of a queue and deletes it
from the queue.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1928529976093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p453620783093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2054298666093521">

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

   <tr id="row84965692093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

q

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer queue.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the pointer to the first network data buffer if the queue is not
empty; returns **NULL** otherwise.

NetBufQueueDequeueTail()
------------------------

::

   struct [NetBuf](netbuf.md)* NetBufQueueDequeueTail (struct [NetBufQueue](netbufqueue.md) * q)

**Description:**

Obtains a network data buffer from the tail of a queue and deletes it
from the queue.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1887194617093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p822004722093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1543135580093521">

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

   <tr id="row60839575093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

q

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer queue.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the pointer to the last network data buffer if the queue is not
empty; returns **NULL** otherwise.

NetBufQueueEnqueue()
--------------------

::

   void NetBufQueueEnqueue (struct [NetBufQueue](netbufqueue.md) * q, struct [NetBuf](netbuf.md) * nb )

**Description:**

Adds a network data buffer to the tail of a queue.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row19599441093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p857254513093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1529597228093521">

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

   <tr id="row1964075557093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

q

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer queue.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row358406769093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

nb

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

NetBufQueueEnqueueHead()
------------------------

::

   void NetBufQueueEnqueueHead (struct [NetBufQueue](netbufqueue.md) * q, struct [NetBuf](netbuf.md) * nb )

**Description:**

Adds a network data buffer to the header of a queue.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1371148718093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1677388202093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2124265792093521">

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

   <tr id="row2046416334093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

q

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer queue.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1489244859093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

nb

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

NetBufQueueInit()
-----------------

::

   static void NetBufQueueInit (struct [NetBufQueue](netbufqueue.md) * q)

**Description:**

Initializes a network data buffer queue.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1598144029093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1844798838093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1003076310093521">

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

   <tr id="row812398807093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

q

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer queue.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

NetBufQueueIsEmpty()
--------------------

::

   static bool NetBufQueueIsEmpty (const struct [NetBufQueue](netbufqueue.md) * q)

**Description:**

Checks whether the network data buffer queue is empty.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row160420265093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p993299936093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p910539175093521">

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

   <tr id="row1926396307093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

q

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer queue.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **true** if the queue is empty; returns **false** otherwise.

NetBufQueueSize()
-----------------

::

   static uint32_t NetBufQueueSize (const struct [NetBufQueue](netbufqueue.md) * q)

**Description:**

Obtains the size of a network data buffer queue.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row64326175093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p14331711093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1484642522093521">

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

   <tr id="row1978850085093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

q

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer queue.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the size of the network data buffer queue.

NetBufResizeRoom()
------------------

::

   int32_t NetBufResizeRoom (struct [NetBuf](netbuf.md) * nb, uint32_t head, uint32_t tail )

**Description:**

Adjusts the size of a network data buffer space.

This function is used to apply for a new network data buffer based on
the configured reserved space and the size of the source network data
buffer, and copy the actual data to the new network data buffer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row8767134093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p820811494093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p592093392093521">

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

   <tr id="row636158212093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

nb

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network data buffer.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1984418021093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

head

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the size of the header buffer segment reserved.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row311643500093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

tail

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the size of the tail buffer segment reserved.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a non-zero value
otherwise.

NetDevGetRegisterCount()
------------------------

::

   uint32_t NetDevGetRegisterCount (void )

**Description:**

Obtains the number of added network devices.

**Returns:**

Returns the number of added network devices.

NetDeviceAdd()
--------------

::

   int32_t NetDeviceAdd (struct [NetDevice](netdevice.md) * netDevice, [Protocol80211IfType](wlan.md#gac69954f56fcc99fc8aac68aa157831c7) ifType )

**Description:**

Adds a network device to a protocol stack.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1481112438093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p655009756093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p559679453093521">

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

   <tr id="row1780148088093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netDevice

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device structure obtained during
initialization.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1308410093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netDevice

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the network port type, as enumerated in Protocol80211IfType.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a negative value
representing
`HDF_STATUS <driverutils.md#ga7e01536ecbe9b17563dd3fe256202a67>`__ if
the operation fails.

NetDeviceDeInit()
-----------------

::

   int32_t NetDeviceDeInit (struct [NetDevice](netdevice.md) * netDevice)

**Description:**

Deletes a network device.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1083853850093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p758493702093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p597937244093521">

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

   <tr id="row1923173339093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netDevice

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device structure obtained during
initialization.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a negative value
representing
`HDF_STATUS <driverutils.md#ga7e01536ecbe9b17563dd3fe256202a67>`__ if
the operation fails.

NetDeviceDelete()
-----------------

::

   int32_t NetDeviceDelete (struct [NetDevice](netdevice.md) * netDevice)

**Description:**

Deletes a network device from a protocol stack.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2133108483093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1534497032093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p816684734093521">

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

   <tr id="row806259658093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netDevice

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device structure netDevice obtained
during initialization.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a negative value
representing
`HDF_STATUS <driverutils.md#ga7e01536ecbe9b17563dd3fe256202a67>`__ if
the operation fails.

NetDeviceGetCap()
-----------------

::

   uint32_t NetDeviceGetCap (void )

**Description:**

Obtains the maximum number of network devices that can be registered
with this system at the same time.

**Returns:**

Returns the maximum number of network devices.

NetDeviceGetInstByIndex()
-------------------------

::

   struct [NetDevice](netdevice.md)* NetDeviceGetInstByIndex (uint32_t index)

**Description:**

Obtains a network device instance based on the index number.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row237321191093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p487117502093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p918246240093521">

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

   <tr id="row630219805093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

index

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the index number.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the network device structure `NetDevice <netdevice.md>`__ if the
operation is successful; returns **NULL** if the operation fails.

NetDeviceGetInstByName()
------------------------

::

   struct [NetDevice](netdevice.md)* NetDeviceGetInstByName (const char * name)

**Description:**

Obtains the initialized network device instance by a specified device
name.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1866397527093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p836286458093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2080687492093521">

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

   <tr id="row1993983449093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

name

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device name.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the network device structure `NetDevice <netdevice.md>`__
matching the network device name if the operation is successful; returns
**NULL** if the operation fails.

NetDeviceInit()
---------------

::

   struct [NetDevice](netdevice.md)* NetDeviceInit (const char * ifName, uint32_t len, [NetIfCategory](wlan.md#ga530241881cd17e03f8ae254ef1d9755e) ifCategory )

**Description:**

Initializes a network device to obtain its instance.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1213640191093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1957483122093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p227993611093521">

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

   <tr id="row1091681158093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ifName

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device name.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row762596038093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

len

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the length of the network device name.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row155215940093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ifCategory

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the network port category.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the structure `NetDevice <netdevice.md>`__ for the initialized
network device if the operation is successful; returns **NULL** if the
operation fails.

NetDeviceIsAnyInstRunning()
---------------------------

::

   bool NetDeviceIsAnyInstRunning (void )

**Description:**

Checks whether there are working devices among the added network
devices.

**Returns:**

Returns **true** if the added network devices are working; returns
**false** if none of the added network devices is working.

NetDeviceIsInstRunning()
------------------------

::

   bool NetDeviceIsInstRunning (const struct [NetDevice](netdevice.md) * netDevice)

**Description:**

Checks whether a specified network device is working.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row2022725453093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1743031031093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p844750009093521">

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

   <tr id="row195243230093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netDevice

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device structure netDevice obtained
during initialization.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **true** if the specified network device is working; returns
**false** otherwise.

NetIfDhcpIsBound()
------------------

::

   int32_t NetIfDhcpIsBound (const struct [NetDevice](netdevice.md) * netDevice)

**Description:**

Obtains the DHCP negotiation status of a specified network device.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row223618272093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1757745514093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p734574890093521">

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

   <tr id="row1025456312093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netDevice

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device obtained during
initialization.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a non-zero value
otherwise.

NetIfDhcpsStart()
-----------------

::

   int32_t NetIfDhcpsStart (const struct [NetDevice](netdevice.md) * netDevice, char * ip, u16_t ipNum )

**Description:**

Starts the DHCP server.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1677480965093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p2027133084093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2028013646093521">

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

   <tr id="row1953782322093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netDevice

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device structure netDevice obtained
during initialization.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1298809018093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

beginIp

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the IP address to start.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row701812950093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ipNum

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the number of IP addresses.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a non-zero value
otherwise.

NetIfDhcpsStop()
----------------

::

   int32_t NetIfDhcpsStop (const struct [NetDevice](netdevice.md) * netDevice)

**Description:**

Stops the DHCP server.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row109800661093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1626757661093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p2066211210093521">

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

   <tr id="row1963891565093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netDevice

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device structure netDevice obtained
during initialization.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a non-zero value
otherwise.

NetIfDhcpStart()
----------------

::

   int32_t NetIfDhcpStart (const struct [NetDevice](netdevice.md) * netDevice)

**Description:**

Starts the DHCP client of a specified network device.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1998857457093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1363158844093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1464067773093521">

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

   <tr id="row2085020222093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netDevice

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device obtained during
initialization.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a non-zero value
otherwise.

NetIfDhcpStop()
---------------

::

   int32_t NetIfDhcpStop (const struct [NetDevice](netdevice.md) * netDevice)

**Description:**

Stops the DHCP client of a specified network device.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1615944210093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1086851553093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p258238860093521">

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

   <tr id="row1061377202093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netDevice

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device obtained during
initialization.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a non-zero value
otherwise.

NetIfRx()
---------

::

   int32_t NetIfRx (const struct [NetDevice](netdevice.md) * netDevice, struct [NetBuf](netbuf.md) * buff )

**Description:**

Transfers the input data packets from the network side to a protocol
stack.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1848229838093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p291786268093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1613668342093521">

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

   <tr id="row1355488815093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

buff

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the network-side data, in Ether format.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a non-zero value
otherwise.

NetIfRxNi()
-----------

::

   int32_t NetIfRxNi (const struct [NetDevice](netdevice.md) * netDevice, struct [NetBuf](netbuf.md) * buff )

**Description:**

Transfers data packets from the network side to a protocol stack in an
interrupt processing thread.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1060030159093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1963477406093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1611303308093521">

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

   <tr id="row328754100093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

buff

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the network-side data, in Ether format.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a non-zero value
`HDF_STATUS <driverutils.md#ga7e01536ecbe9b17563dd3fe256202a67>`__ if
the operation fails.

NetIfSetAddr()
--------------

::

   int32_t NetIfSetAddr (const struct [NetDevice](netdevice.md) * netDevice, const [IpV4Addr](ipv4addr.md) * ipAddr, const [IpV4Addr](ipv4addr.md) * netMask, const [IpV4Addr](ipv4addr.md) * gw )

**Description:**

Sets an IP address, mask, and gateway.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1792111782093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1585623463093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1003840552093521">

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

   <tr id="row950365072093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netDevice

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device structure netDevice obtained
during initialization.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row570275478093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

ipAddr

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the IP address to set.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2141001342093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netMask

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the mask to set.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row851631466093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

gw

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the gateway to set.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a non-zero value
otherwise.

NetIfSetLinkStatus()
--------------------

::

   int32_t NetIfSetLinkStatus (const struct [NetDevice](netdevice.md) * netDevice, [NetIfLinkStatus](wlan.md#ga7b1187d116fb065d7927ad9f77edd842) status )

**Description:**

Notifies the network layer of the data link layer status.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row544002814093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1520902052093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1035686736093521">

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

   <tr id="row2011198588093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netDevice

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device obtained during
initialization.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1699887119093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

status

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

status Indicates the data link layer status, as enumerated in
NetIfLinkSatus.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a non-zero value
otherwise.

NetIfSetStatus()
----------------

::

   int32_t NetIfSetStatus (const struct [NetDevice](netdevice.md) * netDevice, [NetIfStatus](wlan.md#ga0fb482694e5eac3f48c75de1749c8baf) status )

**Description:**

Notifies the network layer of the network port state.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1133671958093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1580359940093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p105933788093521">

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

   <tr id="row203621547093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netDevice

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device obtained during
initialization. Indicates the network port state, as enumerated in
NetIfSatus.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns **0** if the operation is successful; returns a non-zero value
otherwise.

Pbuf2NetBuf()
-------------

::

   struct [NetBuf](netbuf.md)* Pbuf2NetBuf (const struct [NetDevice](netdevice.md) * netdev, struct pbuf * lwipBuf )

**Description:**

Converts the **pbuf** structure of Lightweight TCP/IP Stack (lwIP) to a
network data buffer.

When a network device is specified, the reserved space of the network
device will be added to the size of the converted network data buffer.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1137920635093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1570741157093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p622720862093521">

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

   <tr id="row361783790093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

netdev

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the network device.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1615625954093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

lwip_buf

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the data buffer of lwIP.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the pointer to the network data buffer if the operation is
successful; returns **NULL** otherwise.

WifiModuleCreate()
------------------

::

   struct [WifiModule](wifimodule.md)* WifiModuleCreate (const struct HdfConfigWifiModuleConfig * config)

**Description:**

Creates a `WifiModule <wifimodule.md>`__ object based on a specified
configuration generated by the HCS.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row667665349093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p371081459093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1081741494093521">

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

   <tr id="row1020275194093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

config

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the configuration generated by the HCS.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Returns:**

Returns the created `WifiModule <wifimodule.md>`__ object.

WifiModuleDelete()
------------------

::

   void WifiModuleDelete (struct [WifiModule](wifimodule.md) * module)

**Description:**

Deletes a specified `WifiModule <wifimodule.md>`__ object.

**Parameters:**

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row519625817093521">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1038233092093521">

Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1616339784093521">

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

   <tr id="row80665771093521">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

module

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

Indicates the pointer to the WifiModule object to delete.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Variable Documentation**\ 
----------------------------

aborted
-------

::

   uint8_t WifiScanRequest::aborted

**Description:**

Whether to abort the scan

abortScan
---------

::

   int32_t(* WifiMac80211Ops::abortScan) ([NetDevice](netdevice.md) *netDev)

**Description:**

Stopping a scan

ackNum
------

::

   uint32_t TcpHeader::ackNum

**Description:**

Acknowledgement number

.. _addfeature-1:

addFeature
----------

::

   int32_t(* WifiModuleIface::addFeature) (struct [WifiModule](wifimodule.md) *module, uint16_t featureType, struct [WifiFeature](wififeature.md) *featureData)

**Description:**

Adding a feature

addKey
------

::

   int32_t(* WifiMac80211Ops::addKey) (struct [NetDevice](netdevice.md) *netdev, uint8_t keyIndex, bool pairwise, const uint8_t *macAddr, struct [KeyParams](keyparams.md) *params)

**Description:**

Adding a key with specified parameters

addr [1/2]
----------

::

   uint8_t MacAddress::addr[ETH_ADDR_LEN]

**Description:**

Device MAC address

addr [2/2]
----------

::

   uint32_t IpV4Addr::addr

**Description:**

IPv4 address

addrLen
-------

::

   uint8_t NetDevice::addrLen

**Description:**

MAC address length

addrMask
--------

::

   uint8_t Wiphy::addrMask[WLAN_MAC_ADDR_LEN]

**Description:**

MAC address mask of the wiphy device. If the device supports multiple
virtual MAC addresses, the bit whose value is **1** in the mask
represents a variable part of the MAC address.

aid [1/2]
---------

::

   uint16_t AssocResp::aid

**Description:**

Authentication ID

aid [2/2]
---------

::

   uint16_t ReassocResp::aid

**Description:**

Authentication ID

akmSuites
---------

::

   uint32_t CryptoSettings::akmSuites[NL80211_MAX_NR_AKM_SUITES]

**Description:**

AKM suite data. For details, see **NL80211_MAX_NR_AKM_SUITES**.

ampduDensity
------------

::

   uint8_t Ieee80211StaHtCap::ampduDensity

**Description:**

Minimum MPDU start spacing

ampduFactor
-----------

::

   uint8_t Ieee80211StaHtCap::ampduFactor

**Description:**

Maximum length of an aggregated MAC Protocol Data Unit (A-MPDU)

arry
----

::

   uint8_t ScannedBssInfo::arry[2]

**Description:**

Reserved

assocReq [1/2]
--------------

::

   struct [AssocReq](assocreq.md) Ieee80211Mgmt::assocReq

**Description:**

Association request

assocReq [2/2]
--------------

::

   struct { ... } ::assocReq

**Description:**

Association request

assocReqIes
-----------

::

   const uint8_t* StationInfo::assocReqIes

**Description:**

Information Elements (IEs) in Association `Request <request.md>`__

assocReqIesLen
--------------

::

   uint32_t StationInfo::assocReqIesLen

**Description:**

IE length in Association `Request <request.md>`__

assocResp [1/2]
---------------

::

   struct [AssocResp](assocresp.md) Ieee80211Mgmt::assocResp

**Description:**

Association response

assocResp [2/2]
---------------

::

   struct { ... } ::assocResp

**Description:**

Association response

aucArry
-------

::

   uint8_t Mac80211Ssids::aucArry[MAC80211_SSIDS_AUC_SIZE]

**Description:**

AuC data array

aucResv
-------

::

   uint8_t WifiConnectParams::aucResv[WIFI_CONNECT_PARM_RESV_SIZE]

**Description:**

Reserved field

aucRsv [1/2]
------------

::

   uint8_t Ieee80211StaHtCap::aucRsv[IEEE80211_STAHTCAP_RESV]

**Description:**

Reserved field

aucRsv [2/2]
------------

::

   uint8_t Wiphy::aucRsv[WIPHY_RSV_SIZE]

**Description:**

Manual alignment of data structures

aucSsid
-------

::

   uint8_t Mac80211Ssids::aucSsid[OAL_IEEE80211_MAX_SSID_LEN]

**Description:**

SSID array

auth [1/2]
----------

::

   struct { ... } ::auth

**Description:**

Authentication Information

auth [2/2]
----------

::

   struct [Auth](auth.md) Ieee80211Mgmt::auth

**Description:**

Authentication Information

authAlg
-------

::

   uint16_t Auth::authAlg

**Description:**

Authentication algorithm

authTransaction
---------------

::

   uint16_t Auth::authTransaction

**Description:**

Authentication transaction

authType
--------

::

   uint8_t WifiConnectParams::authType

**Description:**

Authorization type

band [1/2]
----------

::

   enum [Ieee80211Band](wlan.md#ga9882f415202cf9acb0f4cdfbc456a88d) Ieee80211Channel::band

**Description:**

Frequency band, either 2.4 GHz or 5 GHz

band [2/2]
----------

::

   enum [Ieee80211Band](wlan.md#ga9882f415202cf9acb0f4cdfbc456a88d) Ieee80211SupportedBand::band

**Description:**

Band matching this data structure description

bands
-----

::

   struct [Ieee80211SupportedBand](ieee80211supportedband.md)* Wiphy::bands[[IEEE80211_NUM_BANDS](wlan.md#gga9882f415202cf9acb0f4cdfbc456a88da703cf67d516a80d6dae1b1995017b9a4)]

**Description:**

Supported bands

beacon [1/2]
------------

::

   struct [Beacon](beacon.md) Ieee80211Mgmt::beacon

**Description:**

`Beacon <beacon.md>`__ frame

beacon [2/2]
------------

::

   struct { ... } ::beacon

**Description:**

`Beacon <beacon.md>`__ frame

beaconData
----------

::

   WifiBeaconData* Mac80211beaconParam::beaconData

**Description:**

`Beacon <beacon.md>`__ frame data

beaconFound
-----------

::

   int8_t Ieee80211Channel::beaconFound

**Description:**

When a beacon frame is found in this channel

beaconInt [1/2]
---------------

::

   uint16_t Beacon::beaconInt

**Description:**

`Beacon <beacon.md>`__ interval

beaconInt [2/2]
---------------

::

   uint16_t ProbeResp::beaconInt

**Description:**

`Beacon <beacon.md>`__ interval

beaconInterval
--------------

::

   uint16_t StaBssParameters::beaconInterval

**Description:**

`Beacon <beacon.md>`__ interval

beaconLossCount
---------------

::

   uint32_t StationInfo::beaconLossCount

**Description:**

Number of beacon loss events triggered

bitrate
-------

::

   uint16_t Ieee80211Rate::bitrate

**Description:**

Bit rate, in 100 kbit/s

bitrates
--------

::

   struct [Ieee80211Rate](ieee80211rate.md)* Ieee80211SupportedBand::bitrates

**Description:**

An array of supported bit rates

bssid [1/3]
-----------

::

   uint8_t Ieee80211Mgmt::bssid[6]

**Description:**

BSS ID

bssid [2/3]
-----------

::

   uint8_t ConnetResult::bssid[ETH_ADDR_LEN]

**Description:**

MAC address of the AP associated with the station

bssid [3/3]
-----------

::

   uint8_t* WifiConnectParams::bssid

**Description:**

AP basic service set identifier (BSSID). If this parameter is not
specified, the AP BSSID is automatically obtained from the scan result.

bssParam
--------

::

   struct [StaBssParameters](stabssparameters.md) StationInfo::bssParam

**Description:**

Current BSS parameters

bufs
----

::

   struct BufField NetBuf::bufs[[MAX_BUF_NUM](wlan.md#gga68c01102755fc7d1c810bb0b0635fa90aeef2a730ef9f722cfbac0b24998f8e19)]

**Description:**

Defines buffer segments used to record the offset address (based on the
memory buffer address) and length of each buffer segment, including the
header buffer segment, data segment, and tail buffer segment. For
details, see
`MAX_BUF_NUM <wlan.md#gga68c01102755fc7d1c810bb0b0635fa90aeef2a730ef9f722cfbac0b24998f8e19>`__.

cap
---

::

   uint16_t Ieee80211StaHtCap::cap

**Description:**

HT capability table provided in 802.11n

capabInfo [1/6]
---------------

::

   uint16_t AssocReq::capabInfo

**Description:**

WLAN capability information

capabInfo [2/6]
---------------

::

   uint16_t AssocResp::capabInfo

**Description:**

WLAN capability information

capabInfo [3/6]
---------------

::

   uint16_t ReassocReq::capabInfo

**Description:**

WLAN capability information

capabInfo [4/6]
---------------

::

   uint16_t ReassocResp::capabInfo

**Description:**

WLAN capability information

capabInfo [5/6]
---------------

::

   uint16_t Beacon::capabInfo

**Description:**

WLAN capability information

capabInfo [6/6]
---------------

::

   uint16_t ProbeResp::capabInfo

**Description:**

WLAN capability information

centerFreq
----------

::

   uint16_t Ieee80211Channel::centerFreq

**Description:**

Center frequency

centerFreq1
-----------

::

   int32_t ChannelDef::centerFreq1

**Description:**

Center frequency 1

centerFreq2
-----------

::

   int32_t ChannelDef::centerFreq2

**Description:**

Center frequency 2

chan
----

::

   struct [Ieee80211Channel](ieee80211channel.md)* ChannelDef::chan

**Description:**

Channel information

changeBeacon
------------

::

   int32_t(* WifiMac80211Ops::changeBeacon) ([NetDevice](netdevice.md) *netDev, [Mac80211beaconParam](mac80211beaconparam.md) *param)

**Description:**

Setting the beacon frame based on specified parameters

changeMtu
---------

::

   int32_t(* NetDeviceInterFace::changeMtu) (struct [NetDevice](netdevice.md) *netDev, int32_t newMtu)

**Description:**

Changes the maximum number of transmission units.

changeVirtualIntf
-----------------

::

   int32_t(* WifiMac80211Ops::changeVirtualIntf) ([NetDevice](netdevice.md) *netDev, uint8_t iftype, uint32_t *flags, struct [VifParams](vifparams.md) *params)

**Description:**

Changing virtual APIs

channel
-------

::

   struct [Ieee80211Channel](ieee80211channel.md)* WifiConnectParams::channel

**Description:**

Connection channel. If this parameter is not specified, the connection
channel is automatically obtained from the scan result.

channels [1/2]
--------------

::

   struct [Ieee80211Channel](ieee80211channel.md)* Ieee80211SupportedBand::channels

**Description:**

An array of supported channels

channels [2/2]
--------------

::

   struct [Ieee80211Channel](ieee80211channel.md)* WifiScanRequest::channels[MAX_SCAN_CHANNELS]

**Description:**

Channels to scan for. For details, see **MAX_SCAN_CHANNELS**.

check [1/3]
-----------

::

   uint16_t IpHeader::check

**Description:**

Header check

check [2/3]
-----------

::

   uint16_t UdpHeader::check

**Description:**

Header check

check [3/3]
-----------

::

   uint16_t TcpHeader::check

**Description:**

Checksum

chip
----

::

   struct [HdfWifiChipData](hdfwifichipdata.md)* WifiFeature::chip

**Description:**

Chip

cipher
------

::

   uint32_t KeyParams::cipher

**Description:**

Cipher suite

cipherGroup
-----------

::

   uint32_t CryptoSettings::cipherGroup

**Description:**

Cipher group

ciphersPairwise
---------------

::

   uint32_t CryptoSettings::ciphersPairwise[NL80211_MAX_NR_CIPHER_SUITES]

**Description:**

Unicast cipher suite. For details, see **NL80211_MAX_NR_CIPHER_SUITES**.

cipherSuites
------------

::

   const uint32_t* Wiphy::cipherSuites

**Description:**

Supported cipher suites

connect
-------

::

   int32_t(* WifiMac80211Ops::connect) ([NetDevice](netdevice.md) *netDev, [WifiConnectParams](wificonnectparams.md) *param)

**Description:**

Starting a connection based on the specified parameters

connectedTime
-------------

::

   uint32_t StationInfo::connectedTime

**Description:**

Duration (in seconds) since the last station connection

connectStatus
-------------

::

   uint16_t ConnetResult::connectStatus

**Description:**

Connection status

controlPort
-----------

::

   int8_t CryptoSettings::controlPort

**Description:**

Whether the user space control port is authorized. The value **true**
indicates that the user space control port is unauthorized.

controlPortEthertype
--------------------

::

   uint16_t CryptoSettings::controlPortEthertype

**Description:**

Data can be transmitted over an unauthenticated port.

controlPortNoEncrypt
--------------------

::

   int8_t CryptoSettings::controlPortNoEncrypt

**Description:**

Whether to encrypt frames transmitted over the control port. The value
**1** indicates that the frames are not encrypted.

crypto
------

::

   struct [CryptoSettings](cryptosettings.md) WifiConnectParams::crypto

**Description:**

Cryptography information

currentAp
---------

::

   uint8_t ReassocReq::currentAp[6]

**Description:**

Current AP

dAddr
-----

::

   uint32_t IpHeader::dAddr

**Description:**

Destination address

dataLen
-------

::

   uint32_t NetBuf::dataLen

**Description:**

Actual data length of the network data buffer

deauth [1/2]
------------

::

   struct [Deauth](deauth.md) Ieee80211Mgmt::deauth

**Description:**

Deauthentication Information

deauth [2/2]
------------

::

   struct { ... } ::deauth

**Description:**

Deauthentication Information

deInit [1/3]
------------

::

   int32_t(* WifiModuleIface::deInit) (struct [WifiModule](wifimodule.md) *module)

**Description:**

Deinitializing a WLAN module

deInit [2/3]
------------

::

   int32_t(* WifiFeature::deInit) (struct [WifiFeature](wififeature.md) *feature)

**Description:**

Function for deinitializing the feature

deinit
------

::

   int32_t(* HdfWifiChipData::deinit) (struct [HdfWifiChipData](hdfwifichipdata.md) *chipData)

**Description:**

Function for deinitializing the chip

deInit [3/3]
------------

::

   void(* NetDeviceInterFace::deInit) (struct [NetDevice](netdevice.md) *netDev)

**Description:**

Deinitializes a network device to be delete.

.. _delfeature-1:

delFeature
----------

::

   int32_t(* WifiModuleIface::delFeature) (struct [WifiModule](wifimodule.md) *module, uint16_t featureType)

**Description:**

Deleting a feature

delKey
------

::

   int32_t(* WifiMac80211Ops::delKey) (struct [NetDevice](netdevice.md) *netdev, uint8_t keyIndex, bool pairwise, const uint8_t *macAddr)

**Description:**

Deleting a key based on a specified MAC address

delStation
----------

::

   int32_t(* WifiMac80211Ops::delStation) ([NetDevice](netdevice.md) *netDev, const uint8_t *macAddr)

**Description:**

Deleting a station with a specified MAC address

dest
----

::

   uint16_t UdpHeader::dest

**Description:**

Destination port number

dev [1/2]
---------

::

   void* NetBuf::dev

**Description:**

Network device that receives the network data

dev [2/2]
---------

::

   struct [NetDevice](netdevice.md)* WifiScanRequest::dev

**Description:**

A specified network device to scan for

device
------

::

   struct [HdfDeviceObject](hdfdeviceobject.md)* HdfWifiProductData::device

**Description:**

Structure of the Device Object

disassoc [1/2]
--------------

::

   struct { ... } ::disassoc

**Description:**

Disconnected

disassoc [2/2]
--------------

::

   struct [Disassoc](disassoc.md) Ieee80211Mgmt::disassoc

**Description:**

Disconnected

disconnect
----------

::

   int32_t(* WifiMac80211Ops::disconnect) ([NetDevice](netdevice.md) *netDev, uint16_t reasonCode)

**Description:**

Canceling a connection

dlist [1/2]
-----------

::

   struct [DListHead](dlisthead.md) NetBuf::dlist

**Description:**

Doubly linked list. Generally, multiple network data buffers are linked
by using a doubly linked list.

dlist [2/2]
-----------

::

   struct [DListHead](dlisthead.md) NetBufQueue::dlist

**Description:**

Doubly linked list. Generally, multiple network data buffers are linked
by using a doubly linked list.

dPort
-----

::

   uint16_t TcpHeader::dPort

**Description:**

Destination port number

dstAddr
-------

::

   uint8_t Ieee80211Mgmt::dstAddr[6]

**Description:**

Destination MAC address

dtimPeriod [1/2]
----------------

::

   uint8_t StaBssParameters::dtimPeriod

**Description:**

Delivery Traffic Indication Message (DTIM) period of BSS

dtimPeriod [2/2]
----------------

::

   int32_t Mac80211beaconParam::dtimPeriod

**Description:**

Delivery Traffic Indication Message (DTIM) interval

duration
--------

::

   uint16_t Ieee80211Mgmt::duration

**Description:**

Duration

etherDhost
----------

::

   uint8_t EtherHeader::etherDhost[[MAC_ADDR_SIZE](wlan.md#gae01dbae885bc8abecb82bd865515c081)]

**Description:**

Destination address
`MAC_ADDR_SIZE <wlan.md#gae01dbae885bc8abecb82bd865515c081>`__

etherShost
----------

::

   uint8_t EtherHeader::etherShost[[MAC_ADDR_SIZE](wlan.md#gae01dbae885bc8abecb82bd865515c081)]

**Description:**

Source address
`MAC_ADDR_SIZE <wlan.md#gae01dbae885bc8abecb82bd865515c081>`__

etherType
---------

::

   uint16_t EtherHeader::etherType

**Description:**

Ethernet type, such as 0x8035 (RARP), 0x888e (EAPOL), PAE/802.1x, 0x0800
(IP), 0x86dd (IPV6), and 0x0806 (ARP)

fake
----

::

   uint32_t IfReq::fake

**Description:**

magic field

fe
--

::

   struct [WifiFeature](wififeature.md)* WifiFeatureList::fe[[HDF_WIFI_FEATURE_NUM](wlan.md#ggaec03ba36d71cc2d5f3209bc24aa6ee10a28ff5971d579c1754e03a5f79a0c9e6f)]

**Description:**

An array of WLAN features

feList
------

::

   struct [WifiFeatureList](wififeaturelist.md)* WifiModule::feList

**Description:**

WLAN features

filled
------

::

   uint32_t StationInfo::filled

**Description:**

Flag values of relevant structures

flags [1/7]
-----------

::

   uint8_t RateInfo::flags

**Description:**

Flag field, used to indicate a specific rate transmission type of
802.11n

flags [2/7]
-----------

::

   uint8_t StaBssParameters::flags

**Description:**

Flag, used to indicate a specific rate transmission type of 802.11n

flags [3/7]
-----------

::

   uint32_t Ieee80211Channel::flags

**Description:**

WLAN channel flag

flags [4/7]
-----------

::

   uint32_t Ieee80211Rate::flags

**Description:**

Rate flag

flags [5/7]
-----------

::

   uint32_t Wiphy::flags

**Description:**

`Wiphy <wiphy.md>`__ device attributes

flags [6/7]
-----------

::

   uint8_t TcpHeader::flags

**Description:**

Flags

flags [7/7]
-----------

::

   uint32_t NetDevice::flags

**Description:**

Network port status

fragInfo
--------

::

   uint16_t IpHeader::fragInfo

**Description:**

Fragmentation information

fragThreshold
-------------

::

   uint32_t Wiphy::fragThreshold

**Description:**

Fragment threshold

frameControl
------------

::

   uint16_t Ieee80211Mgmt::frameControl

**Description:**

Frame control field

freq [1/2]
----------

::

   int16_t ScannedBssInfo::freq

**Description:**

Center frequency of the channel where the BSS is located

freq [2/2]
----------

::

   uint16_t ConnetResult::freq

**Description:**

Frequency of the AP

funType
-------

::

   [IfType](iftype.md) NetDevice::funType

**Description:**

Network port type

generation
----------

::

   int32_t StationInfo::generation

**Description:**

Generation number

getModule
---------

::

   struct [WifiModule](wifimodule.md)*(* WifiModuleIface::getModule) (void)

**Description:**

Obtaining a WLAN module (to be deleted)

getStats
--------

::

   struct NetDevStats*(* NetDeviceInterFace::getStats) (struct [NetDevice](netdevice.md) *netDev)

**Description:**

Obtains the statistics.

hardHeaderLen
-------------

::

   uint16_t NetDevice::hardHeaderLen

**Description:**

Header length

hiddenSsid
----------

::

   uint8_t Mac80211beaconParam::hiddenSsid

**Description:**

Whether to hide the SSID

hslConfig
---------

::

   const struct HdfConfigWifiModuleConfig* WifiModuleConfig::hslConfig

**Description:**

Configuration of each feature of the WLAN module

htCap
-----

::

   struct [Ieee80211StaHtCap](ieee80211stahtcap.md) Ieee80211SupportedBand::htCap

**Description:**

HT capability

htSupported
-----------

::

   uint8_t Ieee80211StaHtCap::htSupported

**Description:**

Whether the station supports HT

hwValue [1/2]
-------------

::

   uint16_t Ieee80211Channel::hwValue

**Description:**

Hardware information

hwValue [2/2]
-------------

::

   uint16_t Ieee80211Rate::hwValue

**Description:**

Hardware information

hwValueShort
------------

::

   uint16_t Ieee80211Rate::hwValueShort

**Description:**

Hardware information specified when a short preamble is used

id
--

::

   uint16_t IpHeader::id

**Description:**

Each data packet sent by the host

ie [1/2]
--------

::

   uint8_t* WifiScanRequest::ie

**Description:**

IEEE 802.11 buffer

ie [2/2]
--------

::

   uint8_t* WifiConnectParams::ie

**Description:**

IEEE 802.11 information required for the connection

ieee80211Ptr
------------

::

   struct [WirelessDev](wirelessdev.md)* NetDevice::ieee80211Ptr

**Description:**

Pointer to a wireless device

ieLen [1/2]
-----------

::

   uint32_t WifiScanRequest::ieLen

**Description:**

IEEE 802.11 buffer length

ieLen [2/2]
-----------

::

   uint32_t WifiConnectParams::ieLen

**Description:**

IEEE 802.11 length

iface
-----

::

   struct [WifiModuleIface](wifimoduleiface.md)* WifiModule::iface

**Description:**

APIs

ifrData
-------

::

   uint8_t* IfReq::ifrData

**Description:**

Data pointer

iftype
------

::

   uint8_t WirelessDev::iftype

**Description:**

API type

inactiveTime
------------

::

   uint32_t StationInfo::inactiveTime

**Description:**

Duration (in milliseconds) since the last station activity

init [1/4]
----------

::

   int32_t(* WifiModuleIface::init) (struct [WifiModule](wifimodule.md) *module)

**Description:**

Initializing a WLAN module

init [2/4]
----------

::

   int32_t(* WifiFeature::init) (struct [WifiFeature](wififeature.md) *feature)

**Description:**

Function for initializing the feature

init [3/4]
----------

::

   int32_t(* HdfWifiChipData::init) (struct [HdfWifiChipData](hdfwifichipdata.md) *chipData, const struct HdfConfigWifiChip *chipConfig)

**Description:**

Function for initializing the chip

init [4/4]
----------

::

   int32_t(* NetDeviceInterFace::init) (struct [NetDevice](netdevice.md) *netDev)

**Description:**

Initializes a network device to be added.

interfaceModes
--------------

::

   uint16_t Wiphy::interfaceModes

**Description:**

Bitmask of an API type that is valid for the wiphy device

interval
--------

::

   int32_t Mac80211beaconParam::interval

**Description:**

`Beacon <beacon.md>`__ interval

ioctl
-----

::

   int32_t(* NetDeviceInterFace::ioctl) (struct [NetDevice](netdevice.md) *netDev, [IfReq](ifreq.md) *req, int32_t cmd)

**Description:**

Used for the control command word.

ipAddr
------

::

   uint32_t NetDevNotify::ipAddr

**Description:**

IP address

key [1/2]
---------

::

   uint8_t* KeyParams::key

**Description:**

Key content

key [2/2]
---------

::

   const uint8_t* WifiConnectParams::key

**Description:**

Wired Equivalent Privacy (WEP) key used for Shared Key Authentication
(SKA)

keyIdx
------

::

   uint8_t WifiConnectParams::keyIdx

**Description:**

Index of the WEP key used for SKA

keyLen [1/2]
------------

::

   int32_t KeyParams::keyLen

**Description:**

Key length

keyLen [2/2]
------------

::

   uint8_t WifiConnectParams::keyLen

**Description:**

Key length

lastRxTime
----------

::

   uint32_t NetDevice::lastRxTime

**Description:**

Last time when data is received

legacy
------

::

   uint16_t RateInfo::legacy

**Description:**

100 kbit/s bit rate defined in 802.11a/b/g

len [1/2]
---------

::

   uint32_t NetBuf::len

**Description:**

Length of the memory buffer

len [2/2]
---------

::

   uint16_t UdpHeader::len

**Description:**

Length of a data packet

LinkLayerType
-------------

::

   [NetLinkType](wlan.md#gad3175955d2e6ef3c4f52da9b509d5b4a) NetDevice::LinkLayerType

**Description:**

Data link layer type

listenInterval [1/2]
--------------------

::

   uint16_t AssocReq::listenInterval

**Description:**

Scan interval

listenInterval [2/2]
--------------------

::

   uint16_t ReassocReq::listenInterval

**Description:**

Scan interval

llid
----

::

   uint16_t StationInfo::llid

**Description:**

Local mesh ID

lock
----

::

   struct Spinlock NetBufQueue::lock

**Description:**

Queue operation lock

mac [1/2]
---------

::

   const uint8_t* StationDelParameters::mac

**Description:**

MAC address of the station to which the connection is to be canceled

mac [2/2]
---------

::

   uint8_t MacConfigParam::mac[WLAN_MAC_ADDR_LEN]

**Description:**

MAC address. For details about its length, see **WLAN_MAC_ADDR_LEN**.

macAddr [1/3]
-------------

::

   uint8_t* VifParams::macAddr

**Description:**

MAC address

macAddr [2/3]
-------------

::

   char NetDevice::macAddr[[MAC_ADDR_SIZE](wlan.md#gae01dbae885bc8abecb82bd865515c081)]

**Description:**

MAC address
`MAC_ADDR_SIZE <wlan.md#gae01dbae885bc8abecb82bd865515c081>`__

macAddr [3/3]
-------------

::

   uint8_t Mac80211DisconnectParam::macAddr[WLAN_MAC_ADDR_LEN]

**Description:**

Device MAC address

mask
----

::

   uint32_t StaFlagUpdate::mask

**Description:**

Flag mask

maxAntennaGain
--------------

::

   int32_t Ieee80211Channel::maxAntennaGain

**Description:**

Maximum antenna gain, in dBi

maxPower
--------

::

   int32_t Ieee80211Channel::maxPower

**Description:**

Maximum transmit power, in dBm

maxScanIeLen
------------

::

   uint16_t Wiphy::maxScanIeLen

**Description:**

Maximum SSID length

maxScanSsids
------------

::

   uint8_t Wiphy::maxScanSsids

**Description:**

Maximum number of scanned service set identifiers (SSIDs)

mcs [1/2]
---------

::

   uint8_t RateInfo::mcs

**Description:**

Modulation and Coding Scheme (MCS) index of the HT/VHT/HE rate

mcs [2/2]
---------

::

   struct [Ieee80211McsInfo](ieee80211mcsinfo.md) Ieee80211StaHtCap::mcs

**Description:**

MCS rate

mem
---

::

   uint8_t* NetBuf::mem

**Description:**

Memory buffer address

mfp
---

::

   uint8_t WifiConnectParams::mfp

**Description:**

Whether to enable Management Frame Protection (MFP)

mgmt
----

::

   struct [Ieee80211Mgmt](ieee80211mgmt.md)* ScannedBssInfo::mgmt

**Description:**

Start address of the management frame

mgmtLen
-------

::

   uint32_t ScannedBssInfo::mgmtLen

**Description:**

Management frame length

mlPriv
------

::

   void* NetDevice::mlPriv

**Description:**

Private structure for the driver

module
------

::

   struct [WifiModule](wifimodule.md)* HdfWifiProductData::module

**Description:**

Structure of the WLAN module

moduleConfig
------------

::

   struct [WifiModuleConfig](wifimoduleconfig.md) WifiModule::moduleConfig

**Description:**

Module configurations

modulePrivate
-------------

::

   void* WifiModule::modulePrivate

**Description:**

Private data

mtu
---

::

   uint32_t NetDevice::mtu

**Description:**

Maximum transmission unit

n_akmSuites
-----------

::

   int32_t CryptoSettings::n_akmSuites

**Description:**

Number of authentication and key management (AKM) suites

n_ciphersPairwise
-----------------

::

   int32_t CryptoSettings::n_ciphersPairwise

**Description:**

Number of unicast ciphers supported by the access point (AP)

name [1/3]
----------

::

   char WifiFeature::name[[MAX_WIFI_COMPONENT_NAME_LEN](wlan.md#gaf460a45a5e365279ca6bc5b3e8750542)]

**Description:**

`Feature <feature.md>`__ name, which can contain a maximum of 10
characters

name [2/3]
----------

::

   char HdfWifiChipData::name[[MAX_WIFI_COMPONENT_NAME_LEN](wlan.md#gaf460a45a5e365279ca6bc5b3e8750542)]

**Description:**

Chip name

name [3/3]
----------

::

   char NetDevice::name[IFNAMSIZ]

**Description:**

Network device name **IFNAMSIZ**

nBitrates
---------

::

   int32_t Ieee80211SupportedBand::nBitrates

**Description:**

Length of the array of supported bit rates

nChannels [1/2]
---------------

::

   int32_t Ieee80211SupportedBand::nChannels

**Description:**

Length of the array of supported channels

nChannels [2/2]
---------------

::

   uint32_t WifiScanRequest::nChannels

**Description:**

Number of channels to scan for

nCipherSuites
-------------

::

   int32_t Wiphy::nCipherSuites

**Description:**

Number of supported cipher suites

neededHeadRoom
--------------

::

   uint16_t NetDevice::neededHeadRoom

**Description:**

Length reserved for the header in netbuff\ `NetBuf <netbuf.md>`__

neededTailRoom
--------------

::

   uint16_t NetDevice::neededTailRoom

**Description:**

Length reserved for the tail in netbuff\ `NetBuf <netbuf.md>`__

netdev
------

::

   struct [NetDevice](netdevice.md)* WirelessDev::netdev

**Description:**

Network device

netDeviceIf
-----------

::

   struct [NetDeviceInterFace](netdeviceinterface.md)* NetDevice::netDeviceIf

**Description:**

Network device interface

netifCateg
----------

::

   [NetIfCategory](wlan.md#ga530241881cd17e03f8ae254ef1d9755e) NetDevice::netifCateg

**Description:**

Network interface category
`NetIfCategory <wlan.md#ga530241881cd17e03f8ae254ef1d9755e>`__

netifNotify
-----------

::

   uint32_t(* NetDeviceInterFace::netifNotify) (struct [NetDevice](netdevice.md) *netDev, [NetDevNotify](netdevnotify.md) *notify)

**Description:**

Notifies the network port status.

notifyType
----------

::

   uint32_t NetDevNotify::notifyType

**Description:**

Notification type (reserved)

nss
---

::

   uint8_t RateInfo::nss

**Description:**

Number of streams (for VHT and HE only)

nSsids
------

::

   uint32_t WifiScanRequest::nSsids

**Description:**

Number of SSIDs to scan for

offset [1/2]
------------

::

   int64_t StationInfo::offset

**Description:**

Time offset of station

offset [2/2]
------------

::

   uint8_t TcpHeader::offset

**Description:**

Header length

open
----

::

   int32_t(* NetDeviceInterFace::open) (struct [NetDevice](netdevice.md) *netDev)

**Description:**

Opens the data link layer.

operationType
-------------

::

   uint8_t Mac80211beaconParam::operationType

**Description:**

Operation type

ops
---

::

   struct [WifiMac80211Ops](wifimac80211ops.md)* HdfWifiChipData::ops

**Description:**

Chip MAC address

origFlags
---------

::

   uint32_t Ieee80211Channel::origFlags

**Description:**

Channel flags

origMag
-------

::

   int32_t Ieee80211Channel::origMag

**Description:**

Reserved field

origMpwr
--------

::

   int32_t Ieee80211Channel::origMpwr

**Description:**

Reserved field

owner
-----

::

   struct [NetDevice](netdevice.md)* NetDevice::owner

**Description:**

Network device

p2pMode
-------

::

   uint8_t MacConfigParam::p2pMode

**Description:**

Whether the peer-to-peer (P2P) mode is used.

permAddr
--------

::

   uint8_t Wiphy::permAddr[WLAN_MAC_ADDR_LEN]

**Description:**

Permanent MAC address of the wiphy device. For its length, see
**WLAN_MAC_ADDR_LEN**.

plid
----

::

   uint16_t StationInfo::plid

**Description:**

Peer mesh ID

plinkState
----------

::

   uint8_t StationInfo::plinkState

**Description:**

Mesh peer state

prefixSsidScanFlag
------------------

::

   uint8_t WifiScanRequest::prefixSsidScanFlag

**Description:**

Reserved field

presetChandef
-------------

::

   struct [ChannelDef](channeldef.md) WirelessDev::presetChandef

**Description:**

Channel information

priv
----

::

   uint8_t Wiphy::priv[WIPHY_PRIV_SIZE]

**Description:**

Reserved field

privacy
-------

::

   uint8_t WifiConnectParams::privacy

**Description:**

Whether to use a privacy-enabled AP

probeResp [1/2]
---------------

::

   struct { ... } ::probeResp

**Description:**

Probe response frame

probeResp [2/2]
---------------

::

   struct [ProbeResp](proberesp.md) Ieee80211Mgmt::probeResp

**Description:**

Probe response frame

product_name
------------

::

   char HdfWifiProductData::product_name[[MAX_WIFI_COMPONENT_NAME_LEN](wlan.md#gaf460a45a5e365279ca6bc5b3e8750542)]

**Description:**

WLAN module name, which contains a maximum of 10 bytes

protocol
--------

::

   uint8_t IpHeader::protocol

**Description:**

Protocol, such as 1 (ICMP), 2 (IGMP), 6 (TCP), 17 (UDP), and 89 (OSPF)

qmap
----

::

   uint32_t NetBuf::qmap

**Description:**

Queue mappings of the network data buffer

reasonCode [1/4]
----------------

::

   uint16_t Deauth::reasonCode

**Description:**

Deauthentication cause code

reasonCode [2/4]
----------------

::

   uint16_t Disassoc::reasonCode

**Description:**

Cause code

reasonCode [3/4]
----------------

::

   uint16_t StationDelParameters::reasonCode

**Description:**

Cause of the cancellation

reasonCode [4/4]
----------------

::

   uint16_t Mac80211DisconnectParam::reasonCode

**Description:**

Disconnection reason code

reassocReq [1/2]
----------------

::

   struct { ... } ::reassocReq

**Description:**

Re-authentication

reassocReq [2/2]
----------------

::

   struct [ReassocReq](reassocreq.md) Ieee80211Mgmt::reassocReq

**Description:**

Re-authentication

reassocResp [1/2]
-----------------

::

   struct [ReassocResp](reassocresp.md) Ieee80211Mgmt::reassocResp

**Description:**

Re-authentication response

reassocResp [2/2]
-----------------

::

   struct { ... } ::reassocResp

**Description:**

Re-authentication response

reqIe
-----

::

   uint8_t* ConnetResult::reqIe

**Description:**

Association request IE

reqIeLen
--------

::

   uint32_t ConnetResult::reqIeLen

**Description:**

Length of the association request IE

reserved
--------

::

   uint8_t Ieee80211McsInfo::reserved[IEEE80211_MACINFO_RESV]

**Description:**

Reserved field

resv [1/4]
----------

::

   uint8_t RateInfo::resv

**Description:**

Reserved

resv [2/4]
----------

::

   uint8_t Ieee80211Channel::resv[IEEE80211_CHANNEL_RESV]

**Description:**

Reserved field

resv [3/4]
----------

::

   uint8_t WirelessDev::resv[WIRELESS_DEV_RESV_SIZE]

**Description:**

Reserved field

resv [4/4]
----------

::

   uint8_t WifiScanRequest::resv[SCAN_REQUEST_RESV_SIZE]

**Description:**

Reserved field

resv1
-----

::

   uint8_t StationInfo::resv1

**Description:**

Reserved

rspIe
-----

::

   uint8_t* ConnetResult::rspIe

**Description:**

Association response IE

rspIeLen
--------

::

   uint32_t ConnetResult::rspIeLen

**Description:**

Length of the association response IE

rsv [1/2]
---------

::

   uint8_t NetBuf::rsv[[MAX_NETBUF_RESEVER_SIZE](wlan.md#ga794c035a19a38acc000146a8f9a4ec80)]

**Description:**

Reserved field. For details, see
`MAX_NETBUF_RESEVER_SIZE <wlan.md#ga794c035a19a38acc000146a8f9a4ec80>`__.

rsv [2/2]
---------

::

   uint8_t Ieee80211Rate::rsv[IEEE80211_RATE_RESV]

**Description:**

Reserved field

rtsThreshold
------------

::

   uint32_t Wiphy::rtsThreshold

**Description:**

`Request <request.md>`__ To Send (RTS) threshold

rxBytes [1/2]
-------------

::

   uint64_t StationInfo::rxBytes

**Description:**

Received bytes

rxBytes [2/2]
-------------

::

   uint32_t NetDevStats::rxBytes

**Description:**

Total number of received bits

rxDropped
---------

::

   uint32_t NetDevStats::rxDropped

**Description:**

Packets that are dropped after being received

rxDroppedMisc
-------------

::

   uint32_t StationInfo::rxDroppedMisc

**Description:**

Number of receive failures

rxErrors
--------

::

   uint32_t NetDevStats::rxErrors

**Description:**

Number of received error packets

rxHighest
---------

::

   uint16_t Ieee80211McsInfo::rxHighest

**Description:**

Maximum rate for receiving data

rxMask
------

::

   uint8_t Ieee80211McsInfo::rxMask[IEEE80211_HT_MCS_MASK_LEN]

**Description:**

Mask for receiving data

rxPackets [1/2]
---------------

::

   uint32_t StationInfo::rxPackets

**Description:**

Received data packets

rxPackets [2/2]
---------------

::

   uint32_t NetDevStats::rxPackets

**Description:**

Total number of received packets

rxRate
------

::

   struct [RateInfo](rateinfo.md) StationInfo::rxRate

**Description:**

Receive rate

sAddr
-----

::

   uint32_t IpHeader::sAddr

**Description:**

Source address

selectQueue
-----------

::

   uint16_t(* NetDeviceInterFace::selectQueue) (struct [NetDevice](netdevice.md) *netDev, struct [NetBuf](netbuf.md) *netBuff)

**Description:**

Selects a priority queue.

seq
---

::

   uint8_t* KeyParams::seq

**Description:**

Content of a Temporal Key Integrity Protocol (TKIP) or Counter Mode
Cipher Block Chaining Message Authentication Code Protocol (CCMP) key

seqCtrl
-------

::

   uint16_t Ieee80211Mgmt::seqCtrl

**Description:**

Sequence control

seqLen
------

::

   int32_t KeyParams::seqLen

**Description:**

Length of a TKIP or CCMP key

seqNum
------

::

   uint32_t TcpHeader::seqNum

**Description:**

Sequence number

set
---

::

   uint32_t StaFlagUpdate::set

**Description:**

Flag value

setChannel
----------

::

   int32_t(* WifiMac80211Ops::setChannel) ([NetDevice](netdevice.md) *netDev)

**Description:**

Setting the channel

setDefaultKey
-------------

::

   int32_t(* WifiMac80211Ops::setDefaultKey) (struct [NetDevice](netdevice.md) *netdev, uint8_t keyIndex, bool unicast, bool multicas)

**Description:**

Setting the default key

setMacAddr [1/2]
----------------

::

   int32_t(* NetDeviceInterFace::setMacAddr) (struct [NetDevice](netdevice.md) *netDev, void *addr)

**Description:**

Sets the MAC address.

setMacAddr [2/2]
----------------

::

   int32_t(* WifiMac80211Ops::setMacAddr) ([NetDevice](netdevice.md) *netDev, [Mac80211SetMacParam](wlan.md#ga7566bdca5b1746ade791cd7f863f259b) *param)

**Description:**

Setting the MAC address

setMeshId
---------

::

   int32_t(* WifiMac80211Ops::setMeshId) ([NetDevice](netdevice.md) *netDev, const char *meshId, uint32_t meshIdLen)

**Description:**

Setting the mesh ID

setNetIfStatus
--------------

::

   void(* NetDeviceInterFace::setNetIfStatus) (struct [NetDevice](netdevice.md) *netDev, [NetIfStatus](wlan.md#ga0fb482694e5eac3f48c75de1749c8baf) status)

**Description:**

Sets the network port status.

setSsid
-------

::

   int32_t(* WifiMac80211Ops::setSsid) ([NetDevice](netdevice.md) *netDev, const uint8_t *ssid, uint32_t ssidLen)

**Description:**

Setting the SSID

signal [1/2]
------------

::

   int8_t StationInfo::signal

**Description:**

Signal strength

signal [2/2]
------------

::

   int32_t ScannedBssInfo::signal

**Description:**

Signal strength

signalAvg
---------

::

   int8_t StationInfo::signalAvg

**Description:**

Average signal strength

signalType
----------

::

   uint8_t Wiphy::signalType

**Description:**

Signal type

size
----

::

   uint32_t NetBufQueue::size

**Description:**

Number of network data buffers in the queue

source
------

::

   uint16_t UdpHeader::source

**Description:**

Source port number

specialEtherTypeProcess
-----------------------

::

   [ProcessingResult](wlan.md#ga9c1d6e7df4468671742cb76f72b67af1)(* NetDeviceInterFace::specialEtherTypeProcess) (const struct [NetDevice](netdevice.md) *netDev, struct [NetBuf](netbuf.md) *buff)

**Description:**

Performs private processing without involving network-layer data.

specialProcPriv
---------------

::

   void* NetDevice::specialProcPriv

**Description:**

Private structure for data processing

sPort
-----

::

   uint16_t TcpHeader::sPort

**Description:**

Source port number

srcAddr
-------

::

   uint8_t Ieee80211Mgmt::srcAddr[6]

**Description:**

Source MAC address

ssid [1/2]
----------

::

   uint8_t WifiSsid::ssid[IEEE80211_MAX_SSID_LEN]

**Description:**

SSID content, which contains a maximum of 32 bytes

ssid [2/2]
----------

::

   uint8_t* WifiConnectParams::ssid

**Description:**

SSID

ssidLen [1/3]
-------------

::

   uint8_t WifiSsid::ssidLen

**Description:**

SSID length

ssidLen [2/3]
-------------

::

   uint32_t WifiConnectParams::ssidLen

**Description:**

SSID length

ssidLen [3/3]
-------------

::

   uint8_t Mac80211Ssids::ssidLen

**Description:**

SSID length

ssids
-----

::

   struct [WifiSsid](wifissid.md)* WifiScanRequest::ssids

**Description:**

SSIDs to scan for

staFlags
--------

::

   struct [StaFlagUpdate](staflagupdate.md) StationInfo::staFlags

**Description:**

Station flag masks and values

startAp
-------

::

   int32_t(* WifiMac80211Ops::startAp) ([NetDevice](netdevice.md) *netDev)

**Description:**

Starting an AP

startScan
---------

::

   int32_t(* WifiMac80211Ops::startScan) ([NetDevice](netdevice.md) *netDev, struct [WifiScanRequest](wifiscanrequest.md) *param)

**Description:**

Starting a scan based on the specified parameters

state
-----

::

   char HdfWifiProductData::state

**Description:**

WLAN module state

stats
-----

::

   struct NetDevStats NetDevice::stats

**Description:**

Network statistics

statusCode [1/4]
----------------

::

   uint16_t Auth::statusCode

**Description:**

Authentication status code

statusCode [2/4]
----------------

::

   uint16_t AssocResp::statusCode

**Description:**

Status code

statusCode [3/4]
----------------

::

   uint16_t ReassocResp::statusCode

**Description:**

Status code

statusCode [4/4]
----------------

::

   uint16_t ConnetResult::statusCode

**Description:**

16-bit status code defined in the IEEE protocol

stop
----

::

   int32_t(* NetDeviceInterFace::stop) (struct [NetDevice](netdevice.md) *netDev)

**Description:**

Closes the data link layer.

stopAp
------

::

   int32_t(* WifiMac80211Ops::stopAp) ([NetDevice](netdevice.md) *netDev)

**Description:**

Stopping an AP

subtype
-------

::

   uint8_t StationDelParameters::subtype

**Description:**

Cancellation type

timestamp [1/2]
---------------

::

   uint64_t Beacon::timestamp

**Description:**

Timestamp

timestamp [2/2]
---------------

::

   uint64_t ProbeResp::timestamp

**Description:**

Timestamp

tos
---

::

   uint8_t IpHeader::tos

**Description:**

`Service <service.md>`__ type

totLen
------

::

   uint16_t IpHeader::totLen

**Description:**

Total length of an IP data packet

ttl
---

::

   uint8_t IpHeader::ttl

**Description:**

Generation time

txBytes [1/2]
-------------

::

   uint64_t StationInfo::txBytes

**Description:**

Transmitted bytes

txBytes [2/2]
-------------

::

   uint32_t NetDevStats::txBytes

**Description:**

Total number of transmitted bits

txDropped
---------

::

   uint32_t NetDevStats::txDropped

**Description:**

Packets dropped before transmission

txErrors
--------

::

   uint32_t NetDevStats::txErrors

**Description:**

Transmitted error packets

txFailed
--------

::

   uint32_t StationInfo::txFailed

**Description:**

Number of failed transmissions

txPackets [1/2]
---------------

::

   uint32_t StationInfo::txPackets

**Description:**

Transmitted data packets

txPackets [2/2]
---------------

::

   uint32_t NetDevStats::txPackets

**Description:**

Total number of transmitted packets

txParams
--------

::

   uint8_t Ieee80211McsInfo::txParams

**Description:**

Parameters for sending data

txPetries
---------

::

   uint32_t StationInfo::txPetries

**Description:**

Number of retransmissions

txRate
------

::

   struct [RateInfo](rateinfo.md) StationInfo::txRate

**Description:**

Transmission rate

type
----

::

   uint16_t HdfWifiChipData::type

**Description:**

Chip type

updateModule
------------

::

   int32_t(* WifiModuleIface::updateModule) (struct [WifiModule](wifimodule.md) *module)

**Description:**

Updating a WLAN module based on a specified configuration.

urgent
------

::

   uint16_t TcpHeader::urgent

**Description:**

Urgent pointer

use4Addr
--------

::

   int32_t VifParams::use4Addr

**Description:**

Whether to use a frame containing four addresses

variable [1/7]
--------------

::

   uint8_t Auth::variable[0]

**Description:**

Algorithm challenge information stored in a flexible array

variable [2/7]
--------------

::

   uint8_t AssocReq::variable[0]

**Description:**

SSID and rate information stored in a flexible array

variable [3/7]
--------------

::

   uint8_t AssocResp::variable[0]

**Description:**

Rate information stored in a flexible array

variable [4/7]
--------------

::

   uint8_t ReassocReq::variable[0]

**Description:**

SSID and rate information stored in a flexible array

variable [5/7]
--------------

::

   uint8_t ReassocResp::variable[0]

**Description:**

Rate information stored in a flexible array

variable [6/7]
--------------

::

   uint8_t Beacon::variable[0]

**Description:**

SSID and rate information

variable [7/7]
--------------

::

   uint8_t ProbeResp::variable[0]

**Description:**

SSID and rate information

versionAndHl
------------

::

   uint8_t IpHeader::versionAndHl

**Description:**

Version and header length

watchdogTime
------------

::

   int32_t NetDevice::watchdogTime

**Description:**

Watchdog duration

wdev
----

::

   struct [WirelessDev](wirelessdev.md)* WifiScanRequest::wdev

**Description:**

A specified wireless device to scan for

width
-----

::

   enum [WifiChannelType](wlan.md#ga9d902b330de99c24b2a8c3ba7120af21) ChannelDef::width

**Description:**

Bandwidth

window
------

::

   uint16_t TcpHeader::window

**Description:**

Window size

wiphy [1/2]
-----------

::

   struct [Wiphy](wiphy.md)* WirelessDev::wiphy

**Description:**

`Wiphy <wiphy.md>`__ device

wiphy [2/2]
-----------

::

   struct [Wiphy](wiphy.md)* WifiScanRequest::wiphy

**Description:**

A specified wiphy device to scan for

wlanType
--------

::

   [Protocol80211IfType](wlan.md#gac69954f56fcc99fc8aac68aa157831c7) IfType::wlanType

**Description:**

WLAN network port type: AP or STA

wpaVersions
-----------

::

   uint32_t CryptoSettings::wpaVersions

**Description:**

WLAN Protected Access (WPA) version

xmit
----

::

   [NetDevTxResult](wlan.md#ga9fb4e578a15db1b0087d7b3831591ced)(* NetDeviceInterFace::xmit) (struct [NetDevice](netdevice.md) *netDev, struct [NetBuf](netbuf.md) *netBuff)

**Description:**

Sends data.
