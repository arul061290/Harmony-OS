Differences from the Linux Standard Library
===========================================

This section describes the key differences between the standard library
carried by the OpenHarmony kernel and the Linux standard library. For
more information, see the API document of the C library.

Process
-------

1. Only the static priority is supported by OpenHarmony user-level
   processes. The priority ranges from 10 (highest priority) to 31
   (lowest priority).
2. Only the static priority is supported by OpenHarmony user-level
   threads. The priority ranges from 0 (highest priority) to 31 (lowest
   priority).
3. OpenHarmony scheduling policies can be **SCHED_RR** or
   **SCHED_FIFO**.
4. **sched_yield()** is used to yield the CPU occupied by the running
   process. **thrd_yield()** is used to yield the CPU occupied by the
   running thread.

Memory
------

Differences from Linux mmap
---------------------------

mmap prototype: void \*mmap (void \*addr, size_t length, int prot, int
flags, int fd, off_t offset)

The lifecycle implementation of **fd** is different from that of Linux
glibc. To be specific, the glibc can release the **fd** handle
immediately after successfully invoking the mmap for mapping. In the
OpenHarmony kernel, you are not allowed to close **fd** immediately
after the mapping is successful. You can close **fd** only after the
munmap is canceled. If you do not close the **fd**, the operating system
reclaims it when the process exits.

Code Example
------------

For Linux OS:

::

   int main(int argc, char *argv[])
   {
       int fd;
       void *addr = NULL;
       ...
       fd = open(argv[1], O_RDONLY);
       if (fd == -1){
           perror("open");
           exit(EXIT_FAILURE);
       }
       addr = mmap(NULL, length, PROT_READ, MAP_PRIVATE, fd, offset);
       if (addr == MAP_FAILED) {
           perror("mmap");
           exit(EXIT_FAILURE);
       }
       close(fd); /* close immediately, OpenHarmony do not support this way */ 
       ...
       exit(EXIT_SUCCESS);
   }

For OpenHarmony:

::

   int main(int argc, char *argv[])
   {
       int fd;
       void *addr = NULL;
       ...
       fd = open(argv[1], O_RDONLY);
       if (fd == -1){
           perror("open");
           exit(EXIT_FAILURE);
       }
       addr = mmap(NULL, length, PROT_READ, MAP_PRIVATE, fd, offset);
       if (addr == MAP_FAILED) {
           perror("mmap");
           exit(EXIT_FAILURE);
       }
       ...
       munmap(addr, length);
       close(fd); /* close after munmap */
       exit(EXIT_SUCCESS);
   }

File System
-----------

**System directory**: Users cannot modify the system directory or mount
devices to the system directory. The system directories include
**/dev**, **/proc**, **/app**, **/bin**, **/data**, **/etc**, **/lib**,
**/system** and **/usr**.

**User directory**: The user directory refers to **/storage**. Users can
create, read, and write files in this directory, but cannot mount
devices.

In addition to the system and user directories, you can create folders
to mount devices. Note that a mounted folder and its subfolders cannot
be mounted repeatedly or in nested mode. A non-empty folder cannot be
mounted.

Signal
------

-  The default behavior for signals does not include **STOP**,
   **CONTINUE**, and **COREDUMP**.
-  A sleeping process (for example, a process enters the sleeping status
   by calling the **sleep** function) cannot be woken up by a signal.
   Cause: The signal mechanism does not support wakeup. The behavior for
   a signal can be processed only when the process is scheduled by the
   CPU.
-  After a process exits, **SIGCHLD** is sent to its parent process. The
   sending action cannot be canceled.
-  Only signals 1 to 30 are supported. If the receiver receives the same
   signal multiple times, the callback function is executed only once.

Time
----

The time precision of OpenHarmony is tick, with the default value of 10
ms/tick. The discrepancy of the **sleep** and **timeout** functions is
less than or equal to 2 ticks.
