Network
=======

Basic Concepts 
--------------

The network module implements basic functions of the TCP/IP protocol
stack and provides the standard POSIX socket interfaces.

   |image1| **NOTE:** Currently, the OS uses **lwIP** to provide network
   capabilities.

When to Use
-----------

For user-space development, the OpenHarmony kernel provides a set of
APIs for you to implement network functionalities, including creating
and disabling sockets, transmitting and receiving data, and setting
network attributes, in addition to standard POSIX socket functions
provided by the C library.

Description
-----------

**Table 1** Standard APIs in the C library

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1494810045717">

.. raw:: html

   <th class="cellrowborder" valign="top" width="15.17%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p294915015578">

Header File

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50.9%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p17949190205711">

Function

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="33.93%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p894950175712">

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

   <tr id="row19501105571">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p109504011576">

sys/socket.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p99508013571">

int accept(int socket, struct sockaddr *address,
socklen_t*\ address_len)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2095015035719">

Accepts incoming connection requests.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row209508065717">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p136322417199">

sys/socket.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p89509014573">

int bind(int s, const struct sockaddr \*name, socklen_t namelen)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p6950903575">

Binds an IP address to a socket.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row99511100571">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p23757247194">

sys/socket.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p59529055717">

int shutdown(int socket, int how)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p129527012573">

Shuts down a socket.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row49527011574">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p0392172441910">

sys/socket.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p29531909577">

int getpeername(int s, struct sockaddr *name, socklen_t*\ namelen)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p119534011576">

Retrieves the peer address of the specified socket.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row139532014576">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p34091724181911">

sys/socket.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p616711716015">

int getsockname(int s, struct sockaddr *name, socklen_t*\ namelen)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p181651471103">

Retrieves the local address of the specified socket.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row695520019572">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1842812441920">

sys/socket.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p2016357007">

int getsockopt(int s, struct sockaddr *name, socklen_t*\ namelen)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1716037404">

Retrieves the socket options.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row79551708579">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2442224121911">

sys/socket.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p6158671601">

int setsockopt(int sockfd, int level, int optname, void *optval,
socklen_t*\ optlen)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p415510716015">

Sets the socket options.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row595550165713">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1345422415197">

unistd.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p19153371020">

int close(int s)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p815119715017">

Closes a socket.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row139566085714">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p114692024121917">

sys/socket.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p181481371010">

int connect(int s, const struct sockaddr \*name, socklen_t namelen)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p41455713010">

Initiates a connection to a socket.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row89575035714">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p184811924191919">

sys/socket.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p21421376013">

int listen(int sockfd, int backlog)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p9139271308">

Listens for network connections.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row69581108574">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p349182412196">

sys/socket.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1813627005">

ssize_t recv(int socket, void \*buffer, size_t length, int flags)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1113318713018">

Receives data from another socket.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row89591609574">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p55011249191">

sys/socket.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p10131976020">

ssize_t recvmsg(int s, struct msghdr \*message, int flags)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2010837004">

Receives data from a specified socket based on the input parameters.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row8960903574">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1351310242192">

sys/socket.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p310519717015">

ssize_t recvfrom(int socket, void *buffer, size_t length, int flags,
struct sockaddr*\ address, socklen_t \*address_len)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p11102471608">

Receives data from a specified socket and obtains the IP address of the
data source.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row16961120195719">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p3525112420198">

sys/socket.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p101001872009">

ssize_t send(int s, const void \*dataptr, size_t size, int flags)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p197171402">

Sends data to another socket.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row59620075717">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p165381324121910">

sys/socket.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p6941671602">

ssize_t sendmsg(int s, const struct msghdr \*message, int flags)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p13912710013">

Sends data to another socket based on the input parameters.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row296213055716">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1055242414196">

sys/socket.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p588573013">

ssize_t sendto(int s, const void *dataptr, size_t size, int flags, const
struct sockaddr*\ to, socklen_t tolen)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p108612713014">

Sends data to another socket at the specified destination IP address.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1896320155718">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p165642024191919">

sys/socket.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p168413711019">

int socket(int domain, int type, int protocol)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1278772017">

Creates a socket.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row49644012571">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p3574152491918">

sys/select.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p575471204">

int select(int nfds, fd_set *readfds, fd_set*\ writefds, fd_set
*exceptfds, struct timeval*\ timeout)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p6721171012">

Monitors the I/O events of multiple file descriptors.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1965904571">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1958512413195">

sys/ioctl.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p27013715013">

int ioctl(int s, int request, …)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p867471405">

Obtains and sets socket options.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row179471552191312">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p4595192471910">

arpa/inet.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p189481522130">

const char *inet_ntop(int af, const void*\ src, char \*dst, socklen_t
size)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p494814527138">

Converts an IP address in binary format to a string.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row189663017574">

.. raw:: html

   <td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p335556182016">

arpa/inet.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50.9%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p46417716014">

int inet_pton(int af, const char *src, void*\ dst)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.93%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p176112713010">

Converts a string to an IP address in binary format.

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

Details on API differences:

-  **sendmsg**

   **Function prototype:**

   ssize_t sendmsg(int s, const struct msghdr \*message, int flags)

   **Function description:** sends a message on a socket.

   **Parameter description:**

   .. raw:: html

      <table>

   .. raw:: html

      <thead align="left">

   .. raw:: html

      <tr id="row13311125313516">

   .. raw:: html

      <th class="cellrowborder" valign="top" width="19.439999999999998%" id="mcps1.1.3.1.1">

   .. raw:: html

      <p id="p19311195312510">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </th>

   .. raw:: html

      <th class="cellrowborder" valign="top" width="80.56%" id="mcps1.1.3.1.2">

   .. raw:: html

      <p id="p19311205313512">

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

      <tr id="row1731175316511">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="19.439999999999998%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p153111753125118">

   s

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="80.56%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p031165311519">

   Indicates the socket.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row15311185317518">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="19.439999999999998%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p7311115319516">

   message

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="80.56%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p331125385118">

   Indicates the pointer to the message to be sent. The ancillary
   message is not supported.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row63111753195116">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="19.439999999999998%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p131175318519">

   flags

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="80.56%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p11799112211525">

   Indicates the socket flags for sending the message. The options are
   as follows:

   .. raw:: html

      </p>

   .. raw:: html

      <ul id="ul1179912222521">

   .. raw:: html

      <li>

   MSG_MORE: allows messages that have been sent for multiple times to
   be packaged and sent at a time.

   .. raw:: html

      </li>

   .. raw:: html

      <li>

   MSG_DONTWAIT: enables a non-blocking operation.

   .. raw:: html

      </li>

   .. raw:: html

      </ul>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      </tbody>

   .. raw:: html

      </table>

   **Return values:**

   -  Returns the number of bytes that have been sent if the operation
      is successful.
   -  Returns **-1** and sets **errno** if the operation fails.

-  **recvmsg**

   **Function prototype:**

   ssize_t recvmsg(int s, struct msghdr \*message, int flags)

   **Function description:** receives a message from a socket.

   **Parameter description:**

   .. raw:: html

      <table>

   .. raw:: html

      <thead align="left">

   .. raw:: html

      <tr id="row15477840185218">

   .. raw:: html

      <th class="cellrowborder" valign="top" width="21.42%" id="mcps1.1.3.1.1">

   .. raw:: html

      <p id="p8477104015217">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </th>

   .. raw:: html

      <th class="cellrowborder" valign="top" width="78.58000000000001%" id="mcps1.1.3.1.2">

   .. raw:: html

      <p id="p1447717402527">

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

      <tr id="row3477340125210">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="21.42%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p154771740155218">

   s

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="78.58000000000001%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p1347718402522">

   Indicates the socket.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row174771405527">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="21.42%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p54771440185218">

   message

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="78.58000000000001%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p5477164075215">

   Indicates the pointer to the address to receive the message. The
   ancillary message is not supported.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row9477174020529">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="21.42%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p747715404521">

   flags

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="78.58000000000001%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p99911829531">

   Indicates the socket flags for receiving the message. The options are
   as follows:

   .. raw:: html

      </p>

   .. raw:: html

      <ul id="ul1099113216538">

   .. raw:: html

      <li>

   MSG_PEEK: allows the message to be read without being removed.

   .. raw:: html

      </li>

   .. raw:: html

      <li>

   MSG_DONTWAIT: enables a non-blocking operation.

   .. raw:: html

      </li>

   .. raw:: html

      </ul>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      </tbody>

   .. raw:: html

      </table>

   **Return values:**

   -  Returns the number of bytes that have been received if the
      operation is successful.
   -  Returns **-1** and sets **errno** if the operation fails.

-  **ioctl**

   **Function prototype:**

   int ioctl(int s, int request, …)

   **Function description:** obtains or sets socket options.

   **Parameter description:**

   .. raw:: html

      <table>

   .. raw:: html

      <thead align="left">

   .. raw:: html

      <tr id="row16113161795318">

   .. raw:: html

      <th class="cellrowborder" valign="top" width="15.25%" id="mcps1.1.3.1.1">

   .. raw:: html

      <p id="p1811381712530">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </th>

   .. raw:: html

      <th class="cellrowborder" valign="top" width="84.75%" id="mcps1.1.3.1.2">

   .. raw:: html

      <p id="p20113161712534">

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

      <tr id="row18113191735318">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="15.25%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p9113617165312">

   s

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="84.75%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p16114317145314">

   Indicates the socket.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row5114121719536">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="15.25%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p17114117185312">

   request

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="84.75%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p137162040165319">

   Indicates the operation to perform on the socket options. The options
   are as follows:

   .. raw:: html

      </p>

   .. raw:: html

      <ul id="ul1671694075316">

   .. raw:: html

      <li>

   FIONREAD: obtains the number of bytes of the data that can be read
   from the socket.

   .. raw:: html

      </li>

   .. raw:: html

      <li>

   FIONBIO: sets whether the socket is non-blocked.

   .. raw:: html

      </li>

   .. raw:: html

      </ul>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      </tbody>

   .. raw:: html

      </table>

   **Return values:**

   -  Returns **0** if the operation is successful.
   -  Returns **-1** and sets **errno** if the operation fails.

.. |image1| image:: public_sys-resources/icon-note.gif
