Thread
======

Basic Concepts
--------------

Threads are the minimum running units that compete for system resources.
They can use or wait to use CPUs and use system resources such as
memory. They run independently from one another.

Threads in each process of the OpenHarmony kernel run and are scheduled
independently. The scheduling of threads in a process is not affected by
threads in other processes.

Threads in the OpenHarmony kernel use the preemptive scheduling
mechanism, either round-robin (RR) scheduling or First In First Out
(FIFO) scheduling.

Threads in the OpenHarmony kernel are assigned 32 priorities, ranging
from **0** (highest) to **31** (lowest).

A high-priority thread in a process can preempt the resources of a
low-priority thread in this process. The low-priority thread can be
scheduled only after the high-priority thread is blocked or terminated.

**A thread may have the following states:**

-  **Init**: The thread is being created.

-  **Ready**: The thread is in the ready list and waits for being
   scheduled by the CPU.

-  **Running**: The thread is running.

-  **Blocked**: The thread is blocked and suspended. The **Blocked**
   states include **pend** (blocked due to lock, event, or semaphore
   issues), **suspend** (active pending), **delay** (blocked due to
   delays), and **pendtime** (blocked by waiting timeout of locks,
   events, or semaphores).

-  **Exit**: The thread stops running and waits for the parent thread to
   reclaim its control block resources.

**Figure 1** State transition of a thread

|image1|

**Description of the thread state transition:**

-  Init→Ready:

   When a thread is created, the thread enters the **Init** state to
   start initialization after obtaining the control block. After the
   thread is initialized, the thread is inserted into the scheduling
   queue and therefore enters the **Ready** state.

-  Ready→Running:

   When a thread switchover is triggered, the thread with the highest
   priority in the ready list is executed and enters the **Running**
   state. This thread will be deleted from the ready list.

-  Running→Blocked:

   When a running thread is blocked (for example, is pended, delayed, or
   reading semaphores), the thread is deleted from the ready list, and
   its state changes from **Running** to **Blocked**. Then, a thread
   switchover is triggered to run the thread with the highest priority
   in the ready list.

-  Blocked→Ready/Blocked→Running:

   After the blocked thread is restored (for example, the thread is
   restored, the delay times out, the semaphore reading times out, or
   semaphores have been read), the thread is added to the ready list and
   changes from the **Blocked** state to the **Ready** state. In this
   case, if the priority of the restored thread is higher than that of
   the running thread, a thread switchover occurs to run the restored
   thread, and therefore the restored thread changes from the **Ready**
   state to the **Running** state.

-  Ready→Blocked:

   A thread may also be blocked (suspended) in the **Ready** state. The
   blocked thread will change from the **Ready** state to the
   **Blocked** state and is deleted from the ready list. In this case,
   the thread will not be scheduled until it is restored.

-  Running→Ready:

   After a thread with a higher priority is created or restored, threads
   will be scheduled. The thread with the highest priority in the ready
   list will change to the **Running** state. The originally running
   thread will change from the **Running** state to the **Ready** state
   and be added to the ready list.

-  Running→Exit:

   When a running thread is terminated, its state changes from
   **Running** to **Exit**. The thread without the
   **PTHREAD_CREATE_DETACHED** attribute will present the **Exit** state
   after being terminated.

-  Blocked→Exit:

   If an API is called to delete a blocked thread, the thread changes
   from the **Blocked** state to the **Exit** state.

When to Use
-----------

After a thread is created, it can be scheduled, suspended, restored, and
delayed in user space. In addition, you can set and obtain the
scheduling priority and scheduling policy of the thread.

Available APIs
--------------

The following table describes the APIs provided by the thread management
module of the OpenHarmony kernel.

**Table 1** APIs provided by the thread management module

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row16880122144619">

.. raw:: html

   <th class="cellrowborder" valign="top" width="14.29%" id="mcps1.2.5.1.1">

.. raw:: html

   <p id="p88808214619">

Header File

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="28.57%" id="mcps1.2.5.1.2">

.. raw:: html

   <p id="p16880182174611">

Function

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="22.45%" id="mcps1.2.5.1.3">

.. raw:: html

   <p id="p198806214469">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="34.69%" id="mcps1.2.5.1.4">

.. raw:: html

   <p id="p1188013294618">

Remarks

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

   <tr id="row1188092104619">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p488052134616">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p108808218461">

pthread_attr_destroy

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p18809234612">

Destroys a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p1988012213468">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row28802274616">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p148806212469">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p7880720461">

pthread_attr_getinheritsched

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p588012104619">

Obtains inherit scheduler attributes of a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p11880524466">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1888132164611">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p8881202114618">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p13881142154614">

pthread_attr_getschedparam

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p12881142144612">

Obtains scheduling parameter attributes of a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p988112204611">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row788102134613">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p16881122114611">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p388111215466">

pthread_attr_getschedpolicy

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p19881152174612">

Obtains scheduling policy attributes of a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p988112294619">

OpenHarmony supports the SCHED_FIFO and SCHED_RR scheduling policies.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row14881423468">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p588152114611">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p188811626465">

pthread_attr_getstacksize

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p08825214467">

Obtains the stack size of a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p8882827467">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row088212144619">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p688215274612">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p88827218466">

pthread_attr_init

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p14447368158">

Initializes a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p12882202134618">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1788214210462">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p3882525463">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1882528461">

pthread_attr_setdetachstate

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p11455363157">

Sets the detach state for a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p1788202174613">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row188829211469">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1088222134619">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p588272204612">

pthread_attr_setinheritsched

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p14611364154">

Sets inherit scheduler attributes for a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p3883102174611">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1588310244610">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p118831210461">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p188318214611">

pthread_attr_setschedparam

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p1746636141515">

Sets scheduling parameter attributes for a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p44251243115214">

A larger value represents a higher priority of the thread in the system.

.. raw:: html

   </p>

.. raw:: html

   <p id="p142941635183917">

Note: The inheritsched field of the pthread_attr_t attribute must be set
to PTHREAD_EXPLICIT_SCHED. Otherwise, the configured thread scheduling
priority does not take effect. The default value is
PTHREAD_INHERIT_SCHED.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row118831264610">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1688315220469">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1488320217468">

pthread_attr_setschedpolicy

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p154615365156">

Sets scheduling policy attributes for a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p28831823468">

OpenHarmony supports the SCHED_FIFO and SCHED_RR scheduling policies.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row888320244618">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p88840216460">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p3884328461">

pthread_attr_setstacksize

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p158841329461">

Sets the stack size for a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p1488412244619">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row168841629468">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p988452104612">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p19884162194610">

pthread_getattr_np

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p64812367153">

Obtains the attributes of a created thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p108847254615">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row28842029469">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1788412214613">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p188411220465">

pthread_cancel

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p08001317121519">

Sends a cancellation request to a thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p1288416254611">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row788418214464">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p128844204618">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p17885182194616">

pthread_testcancel

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p1279931731513">

Requests delivery of any pending cancellation request.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p1588552204613">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row98857211461">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p5885102174614">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1388582144612">

pthread_setcanceltype

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p2079991771517">

Sets the cancelability type for the calling thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p138854224619">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1988516211466">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p68851929468">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p288515234613">

pthread_setcancelstate

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p8799217101512">

Sets the cancelability state for the calling thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p488518224620">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1288520284619">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p158851125462">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p188511211463">

pthread_create

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p18798171712153">

Creates a thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p14886192124615">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1288614204611">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p388610218462">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p108861274620">

pthread_detach

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p379831718156">

Detaches a thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p38861126461">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row188614213467">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p14886826461">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p108861527469">

pthread_equal

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p18799817181516">

Compares whether two thread IDs are equal.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p588612219467">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1488619294613">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p108867214619">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p988752164613">

pthread_exit

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p979871741512">

Terminates the calling thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p28871522460">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row88871220467">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p188877244617">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p188879212461">

pthread_getschedparam

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p158001717101517">

Obtains the scheduling policy and parameters of a thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p198871128465">

OpenHarmony supports the SCHED_FIFO and SCHED_RR scheduling policies.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row198871527462">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1188715284613">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p088715274620">

pthread_join

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p2079921719159">

Waits for a thread to terminate.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p2088815214462">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row13888142184617">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p688802124614">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1088820215469">

pthread_self

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p1179931761515">

Obtains the ID of the calling thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p588802164611">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row15888132124614">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p8888627462">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1888811214620">

pthread_setschedprio

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p1888816219469">

Sets a static scheduling priority for a thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p48881822463">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row12889142194616">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1988915284613">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p148891026466">

pthread_kill

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p128001017121510">

Sends a signal to a thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p9889522466">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row19889624465">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p0889620469">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p58894244612">

pthread_once

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p4801617171515">

Enables the initialization function to be called only once.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p16889122204617">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row288917219462">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1688913294617">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p2889152174613">

pthread_atfork

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p198899219461">

Registers a fork handler to be called before and after fork().

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p2889520467">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row988922114611">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p88897234618">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1588952114611">

pthread_cleanup_pop

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p2048113619157">

Removes the routine at the top of the clean-up handler stack.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p178901424460">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row188906284610">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p8890152134616">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p589017244615">

pthread_cleanup_push

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p114823610159">

Pushes the routine to the top of the clean-up handler stack.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p1890828463">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row189012284618">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p68908224615">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1589011234615">

pthread_barrier_destroy

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p188901723467">

Destroys a barrier (an advanced real-time thread).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p88902244620">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row089015218467">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1689011254619">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p48908214468">

pthread_barrier_init

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p7890172124617">

Initializes a barrier (an advanced real-time thread).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p1689015217461">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row8890182114615">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p118907215468">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p128902215466">

pthread_barrier_wait

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p1189112204618">

Synchronizes participating threads at a barrier.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p208911722464">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row589110216461">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p08911826466">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p18891321469">

pthread_barrierattr_destroy

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p1048203611514">

Destroys a barrier attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p1989112124612">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row9891624468">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p108914214465">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1289182104618">

pthread_barrierattr_init

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p1848113618159">

Initializes a barrier attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p12891202104615">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row118914214464">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1289116214465">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1989116254616">

pthread_mutex_destroy

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p3891927469">

Destroys a mutex.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p1189111220464">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row18891326468">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p68915219469">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p689212124610">

pthread_mutex_init

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p189262174615">

Initializes a mutex.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p089216210461">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1689213216461">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p38923244615">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p989216213462">

pthread_mutex_lock

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p1089216218469">

Locks a mutex.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p58921028469">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row989214284614">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p168927213469">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1389262154612">

pthread_mutex_trylock

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p9892182114619">

Attempts to lock a mutex.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p28926213469">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1989218264610">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1892122164617">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p8893132114614">

pthread_mutex_unlock

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p7893182154611">

Unlocks a mutex.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p1689318210466">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row10893192194614">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1789317254618">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1089320217465">

pthread_mutexattr_destroy

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p168933274614">

Destroys a mutex attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p11893326462">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row7893523465">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p128937234619">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p38931922469">

pthread_mutexattr_gettype

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p547173614155">

Obtains the mutex type attribute.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p118932211469">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row15893526464">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1989416284611">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1389413212461">

pthread_mutexattr_init

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p447133671516">

Initializes a mutex attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p1189415254616">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1894102194616">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1289432134614">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p18941928465">

pthread_mutexattr_settype

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p1247203611159">

Sets the mutex type attribute.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p168941328465">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row48942215466">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p108942217463">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1189418216468">

pthread_mutex_timedlock

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p580191751513">

Blocks the calling thread to lock a mutex.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p0894122134613">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1894122134612">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p689414212466">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1189517234613">

pthread_rwlock_destroy

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p7895429466">

Destroys a read-write lock.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p10895122174617">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row989562144613">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p389542184611">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p13895142104612">

pthread_rwlock_init

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p0895172114615">

Initializes a read-write lock.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p78951827462">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row118953217461">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p689516216461">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p58955244611">

pthread_rwlock_rdlock

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p15803181719154">

Applies a read lock to a read-write lock.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p889502164620">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row689515218467">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p178956218463">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p17895152134618">

pthread_rwlock_timedrdlock

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p5803181721513">

Blocks the calling thread to lock a read-write lock for reading.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p1589622114618">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row789615254618">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p168961622467">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1889612124610">

pthread_rwlock_timedwrlock

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p11431336191520">

Blocks the calling thread to lock a read-write lock for writing.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p188966244617">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row38966284617">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1389620264616">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p138961222469">

pthread_rwlock_tryrdlock

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p1780314172156">

Attempts to apply a read lock to a read-write lock.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p989642174614">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row20896142154616">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1689622204620">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p38981620462">

pthread_rwlock_trywrlock

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p1443936191520">

Attempts to apply a write lock to a read-write lock.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p128981725468">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row489815210461">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p18899821465">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1789913217469">

pthread_rwlock_unlock

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p143193651512">

Unlocks a read-write lock.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p390010211465">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1890032124612">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p159009219466">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1190010214469">

pthread_rwlock_wrlock

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p14803517111519">

Applies a write lock to a read-write lock.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p1390011294618">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row590032124613">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p890022144619">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1290010244614">

pthread_rwlockattr_destroy

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p154719365157">

Destroys a read-write lock attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p19900428461">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row190042174617">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1190010284610">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1890017217462">

pthread_rwlockattr_init

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p247133661511">

Initializes a read-write lock attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p17900192154611">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row10900320461">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p5901229462">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p149018294618">

pthread_cond_broadcast

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p16802181771514">

Unblocks all threads that are currently blocked on the condition
variable cond.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p1290118264619">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row590115234620">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p15901202194613">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1190119212466">

pthread_cond_destroy

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p19802017191512">

Destroys a condition variable.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p1390122114610">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1890192164611">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p3901112204616">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1890102184618">

pthread_cond_init

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p48025173153">

Initializes a condition variable.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p119011210466">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row129011214615">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p9902523468">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p59021722460">

pthread_cond_signal

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p58024177158">

Unblocks a thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p179022244615">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row13902423461">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p69022025464">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1190252134620">

pthread_cond_timedwait

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p158024175151">

Blocks the calling thread to wait for the condition set by
pthread_con_signal() for a period of time specified by ts.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p109020264613">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row189022218464">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p09021228463">

pthread.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p3902324460">

pthread_cond_wait

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p1690262154612">

Blocks the calling thread to wait for the condition set by
pthread_con_signal().

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p19902122104611">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row159027218467">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p990318212464">

semaphore.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p109039234617">

sem_destroy

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p195081328171710">

Destroys a specified anonymous semaphore that is no longer used.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p190318214460">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1690342194611">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1490318217469">

semaphore.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p0903162124610">

sem_getvalue

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p650892891712">

Obtains the count value of a specified semaphore.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p69036234614">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1490312214464">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p159031284618">

semaphore.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1790315254617">

sem_init

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p2508328121711">

Creates and initializes an anonymous semaphore.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p129038211463">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1490416211462">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p3904126469">

semaphore.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p090416220464">

sem_post

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p6508162813176">

Increments the semaphore count by 1.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p090414218463">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row14904162164618">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1590432194620">

semaphore.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p29041822467">

sem_timedwait

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p139049213468">

Obtains the semaphore, with a timeout period specified.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p690452114613">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row390411211468">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p199049214612">

semaphore.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1190413217467">

sem_trywait

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p18509102891714">

Attempts to obtain the semaphore.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p39048213469">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row3905152174616">

.. raw:: html

   <td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p690513215466">

semaphore.h

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p15905926462">

sem_wait

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p950912813172">

Obtains the semaphore.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p109051725466">

N/A

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

.. |image1| image:: figures/en-us_image_0000001054569218.png
