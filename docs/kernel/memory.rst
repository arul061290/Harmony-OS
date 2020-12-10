Memory
======

Basic Concepts
--------------

Memory management is an important procedure in software development,
including memory allocation, usage, and reclamation.

Sound memory management approaches and strategies help you improve
software performance and reliability.

When to Use
-----------

For user-space development, the OpenHarmony memory management module
provides a set of APIs for you to perform memory-related operations,
such as memory application, release, remapping, and attribute setting,
in addition to standard APIs provided by the C library.

Available APIs
--------------

**Table 1** Standard APIs in the C library

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row7850171781719">

.. raw:: html

   <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p23316052015">

Header File

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p03417010208">

Function

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p14347010207">

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

   <tr id="row785091771710">

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p73450202019">

strings.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p934008201">

int bcmp(const void *s1, const void*\ s2, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p93412018209">

Compares byte sequences.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row14791155651713">

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p934605204">

strings.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p113414018209">

void bcopy(const void *src, void*\ dest, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1134180102016">

Copies byte sequences.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1734319481817">

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1134900205">

strings.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p18344012207">

void bzero(void \*s, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p23410042015">

Sets byte sequences to zero.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row79226010178">

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p435705201">

string.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p83520042019">

void *memccpy(void*\ dest, const void \*src, int c, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1720911419407">

Copies the first n bytes from the source memory area pointed to by src
to the destination memory area pointed to by dest. The copy checks
whether a character specified by c is found. If c is found, this
function returns the next character of character c in the destination
memory area.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1992212019173">

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p8355012013">

string.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1635180162014">

void *memchr(const void*\ s, int c, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p235306203">

Searches for the first occurrence of the character specified by c in the
n-byte memory area pointed to by s.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row19231001174">

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p23560172012">

string.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1335404201">

int memcmp(const void *s1, const void*\ s2, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p183518092016">

Compares two memory areas.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row189641849111717">

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p758113203203">

string.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p17581112013208">

void *memcpy(void*\ dest, const void \*src, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1958102014208">

Copies n bytes from the source memory area pointed to by src to the
destination memory area pointed to by dest.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2964114919178">

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p85811620182012">

string.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p3581112042013">

void *memmem(const void*\ haystack, size_t haystacklen, const void
\*needle, size_t needlelen)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p4581102032018">

Searches for a needle string in its haystack string.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row3965049101716">

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p17581820192011">

string.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1058119209207">

void *memmove(void*\ dest, const void \*src, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p55811020162015">

Copies n bytes from the source memory area pointed to by src to the
destination memory area pointed to by dest.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row12421329179">

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p358112042016">

string.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p18581720102016">

void *mempcpy(void*\ dest, const void \*src, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p25811520132017">

Copies n bytes from the source memory area pointed to by src to the
destination memory area pointed to by dest.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row343932141715">

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p358152062019">

string.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p20581720152017">

void *memset(void*\ s, int c, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p258102052019">

Copies a character to the specified memory area.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row19344649182">

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p93511010206">

stdlib.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p135180172016">

void \*malloc(size_t size)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p193580102017">

Dynamically allocates a memory block of size.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row923218311911">

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p8347042018">

stdlib.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p133415072012">

void \*calloc(size_t nmemb, size_t size)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2342062011">

Dynamically allocates nmemb memory blocks of size.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row612852462210">

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p11582162062013">

stdlib.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1558211209205">

void *realloc(void*\ ptr, size_t size)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p7582172082018">

Changes the size of the memory block pointed to by ptr to size bytes.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row32325321910">

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p15582192010204">

stdlib.h/malloc.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p458211205205">

void \*valloc(size_t size)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p6582420192014">

Allocates a block of memory with the specified size and aligns the
allocated memory by page size.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row450114218205">

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p93419062018">

stdlib.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1535303201">

void free(void \*ptr)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p173511072015">

Releases the memory space pointed to by ptr.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row96751881817">

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p14351408208">

malloc.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1735120142011">

size_t malloc_usable_size(void \*ptr)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p153513042014">

Obtains the size of the memory block pointed to by ptr.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row46759851816">

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1235140172015">

unistd.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p4351906203">

int getpagesize(void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p103513010204">

Obtains the page size.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row20901907199">

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1558232032010">

unistd.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p158232012203">

void \*sbrk(intptr_t increment)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1558212014202">

Changes the data segment size.

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

-  **mmap**

   **Function prototype:**

   void \*mmap(void \*addr, size_t length, int prot, int flags, int fd,
   off_t offset);

   **Function description:** applies for virtual memory.

   **Parameter description:**

   .. raw:: html

      <table>

   .. raw:: html

      <thead align="left">

   .. raw:: html

      <tr id="row1346572219429">

   .. raw:: html

      <th class="cellrowborder" valign="top" width="11.92%" id="mcps1.1.3.1.1">

   .. raw:: html

      <p id="p146632215425">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </th>

   .. raw:: html

      <th class="cellrowborder" valign="top" width="88.08%" id="mcps1.1.3.1.2">

   .. raw:: html

      <p id="p1446620227424">

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

      <tr id="row1346652216429">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="11.92%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p19466122104213">

   addr

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="88.08%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p1046692215426">

   Indicates the pointer to the start address of the mapping between the
   virtual address space of the calling process and a file or device. If
   this parameter is NULL, the kernel determines the address to start
   (recommended). Otherwise, the portability of the program will
   deteriorate, because the available addresses vary depending on the
   OS.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row8466182274215">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="11.92%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p5466162284220">

   length

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="88.08%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p17466152214420">

   Indicates the length of the mapping.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row154671722134211">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="11.92%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p0467142204215">

   prot

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="88.08%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p6467162234215">

   Indicates the permission to be granted on the mapping area. The
   options are as follows:

   .. raw:: html

      </p>

   .. raw:: html

      <ul id="ul166872913431">

   .. raw:: html

      <li>

   PROT_READ: The mapping area is readable.

   .. raw:: html

      </li>

   .. raw:: html

      <li>

   PROT_WRITE: The mapping area is writable.

   .. raw:: html

      </li>

   .. raw:: html

      <li>

   PROT_EXEC: The mapping area is executable.

   .. raw:: html

      </li>

   .. raw:: html

      <li>

   PROT_NONE: The mapping area cannot be accessed.

   .. raw:: html

      </li>

   .. raw:: html

      </ul>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row173845488436">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="11.92%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p1538474818437">

   flags

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="88.08%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p92503134411">

   Specifies whether updates are visible to other processes mapping the
   same segment. The options are as follows:

   .. raw:: html

      </p>

   .. raw:: html

      <ul id="ul1971648144411">

   .. raw:: html

      <li>

   MAP_PRIVATE: The mapping area is private, and updates to the mapping
   are invisible to other processes mapping the same segment.

   .. raw:: html

      </li>

   .. raw:: html

      <li>

   MAP_SHARED: Updates to the mapping are visible to other processes
   mapping the same segment, and are stored to the disk file.

   .. raw:: html

      </li>

   .. raw:: html

      </ul>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row771075312437">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="11.92%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p187105538438">

   fd

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="88.08%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p1871005374312">

   Indicates the file descriptor.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row1624023824419">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="11.92%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p62406387445">

   offset

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="88.08%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p92401382448">

   Indicates the offset into the file where the mapping will start.

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

   ..

      |image1| **NOTE:** For details about the implementation
      differences of **mmap** between the OS and Linux, see `Differences
      from the Linux Standard
      Library <differences-from-the-linux-standard-library.rst>`__.

   **Return values:**

   -  Returns the pointer to the page-aligned address where the mapping
      is placed if the operation is successful.
   -  Returns **(void \*)-1** if the operation fails.

-  **munmap**

   **Function prototype:**

   int munmap(void \*addr, size_t length);

   **Function description:** releases virtual memory.

   **Parameter description:**

   .. raw:: html

      <table>

   .. raw:: html

      <thead align="left">

   .. raw:: html

      <tr id="row11908192513464">

   .. raw:: html

      <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

   .. raw:: html

      <p id="p186351516144710">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </th>

   .. raw:: html

      <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

   .. raw:: html

      <p id="p1163581610472">

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

      <tr id="row6908112512469">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p10908325194614">

   addr

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p209081825114610">

   Indicates the pointer to the start address of the memory region to
   unmap.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row2908725174617">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p29084251467">

   length

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p11908152510468">

   Indicates the length of the address range to unmap.

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

   **Return values:**

   -  Returns **0** if the operation is successful.
   -  Returns **-1** if the operation fails.

-  **mprotect**

   **Function prototype:**

   int mprotect(void \*addr, size_t length, int prot);

   **Function description:** modifies the access permission on a memory
   region.

   **Parameter description:**

   .. raw:: html

      <table>

   .. raw:: html

      <thead align="left">

   .. raw:: html

      <tr id="row19636124813475">

   .. raw:: html

      <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

   .. raw:: html

      <p id="p26364483473">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </th>

   .. raw:: html

      <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

   .. raw:: html

      <p id="p13636748124717">

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

      <tr id="row176369484473">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p763615487477">

   addr

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p1763654844715">

   Indicates the pointer to the start address of the memory region to
   modify, which must be a multiple of the page size. If the access
   permission is abnormal, the kernel throws an exception and kills the
   process rather than send SIGSEGV signals to the current process.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row17636134824716">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p1163694824714">

   length

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p463613482472">

   Indicates the length of the memory region to modify.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row196361148184716">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p8636184810477">

   prot

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p474391424815">

   Indicates the permission of the memory region to modify. The options
   are as follows:

   .. raw:: html

      </p>

   .. raw:: html

      <ul id="ul333217192481">

   .. raw:: html

      <li>

   PROT_READ: The memory region is readable.

   .. raw:: html

      </li>

   .. raw:: html

      <li>

   PROT_WRITE: The memory region is writable.

   .. raw:: html

      </li>

   .. raw:: html

      <li>

   PROT_EXEC: The memory region is executable.

   .. raw:: html

      </li>

   .. raw:: html

      <li>

   PROT_NONE: The memory region cannot be accessed.

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
   -  Returns **-1** if the operation fails.

-  **mremap**

   **Function prototype:**

   void \*mremap(void \*old_address, size_t old_size, size_t new_size,
   int flags, void new_address);

   **Function description:** remaps the virtual memory address.

   **Parameter description:**

   .. raw:: html

      <table>

   .. raw:: html

      <thead align="left">

   .. raw:: html

      <tr id="row19544132134919">

   .. raw:: html

      <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

   .. raw:: html

      <p id="p205459214499">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </th>

   .. raw:: html

      <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

   .. raw:: html

      <p id="p4545102104911">

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

      <tr id="row75451321164918">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p125451321144916">

   old_address

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p1554522104914">

   Indicates the old address of the virtual memory block that needs to
   be expanded or shrunk. The old_address must be page-aligned.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row1545172118495">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p205452215498">

   old_size

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p954572164910">

   Indicates the old size of the virtual memory block.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row1754512144913">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p1854532184916">

   new_size

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p85451021164911">

   Indicates the new size of the virtual memory block.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row1545152120497">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

   .. raw:: html

      <p id="p145451221204913">

   flags

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

   .. raw:: html

      <p id="p2692195864912">

   Indicates the flags to control the remapping. If there is no
   sufficient space to expand the mapping in the current location, the
   operation will fail.

   .. raw:: html

      </p>

   .. raw:: html

      <ul id="ul14935819135019">

   .. raw:: html

      <li>

   MREMAP_MAYMOVE: allows the kernel to relocate the mapping to a new
   virtual address.

   .. raw:: html

      </li>

   .. raw:: html

      <li>

   MREMAP_FIXED: enables the mremap() function to accept the fifth
   parameter void \*new_address, which specifies that the mapping
   address must be page-aligned. All previous mappings within the
   address range specified by new_address and new_size are unmapped. If
   MREMAP_FIXED is specified, MREMAP_MAYMOVE must also be specified.

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

   -  Returns the pointer to the new virtual memory area if the
      operation is successful.
   -  Returns **(void \*)-1** if the operation fails.

.. |image1| image:: public_sys-resources/icon-note.gif
