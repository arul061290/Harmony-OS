Process
=======

Basic Concepts
--------------

Processes are resource management units in the OS. They can use or wait
to use CPUs and use system resources such as memory. They run
independently from one another.

The OpenHarmony kernel allows multiple processes to run simultaneously,
switch, and communicate, facilitating your management over service
programs. In this regard, you will have more time to devote to the
implementation of service functionalities.

Processes in the OpenHarmony kernel use the preemptive scheduling
mechanism, either round-robin (RR) scheduling or First In First Out
(FIFO) scheduling.

These processes are assigned 32 priorities (**0** to **31**). Among
them, user processes can be configured with 22 priorities from **10**
(highest) to **31** (lowest).

A high-priority process can preempt the resources of a low-priority
process. The low-priority process can be scheduled only after the
high-priority process is blocked or terminated.

Each user-space process has its own memory space, which is invisible to
other processes. In this way, processes are isolated from each other.

The user-space root process init is started by the kernel. Then other
user-space processes are created by the init process via the **fork**
call.

**A process may have the following states:**

-  **Init**: The process is being created.

-  **Ready**: The process is in the ready list and waits for being
   scheduled by the CPU.

-  **Running**: The process is running.

-  **Pend**: The process is blocked and suspended. When all threads in a
   process are blocked, the process is blocked and suspended.

-  **Zombies**: The process stops running and waits for the parent
   process to reclaim its control block resources.

**Figure 1** State transition of a process

|image1|

**Description of the process state transition:**

-  Init→Ready:

   When a process is created, the process enters the **Init** state to
   start initialization after obtaining the process control block. After
   the process is initialized, the process is inserted into the
   scheduling queue and therefore enters the **Ready** state.

-  Ready→Running:

   When a process switchover is triggered, the process with the highest
   priority in the ready list is executed and enters the **Running**
   state. If this process has no thread in the **Ready** state, the
   process is deleted from the ready list and resides only in the
   **Running** state. However, if it has threads in the **Ready** state,
   the process still stays in the ready list. In this case, the process
   is in both the **Ready** and **Running** states.

-  Running→Pend:

   If all threads in a process are entering the **Pend** state, the
   process will enter the **Pend** state together with its last thread.
   Then, a process switchover is triggered.

-  Pend→Ready/Pend→Running:

   When any thread in a **Pend** process restores to the **Ready**
   state, the process is added to the ready list and changes to the
   **Ready** state. If a process switchover occurs at this time, the
   process state changes from the **Ready** state to the **Running**
   state.

-  Ready→Pend:

   When the last ready thread in a process enters the **Pend** state,
   the process is deleted from the ready list, and the process changes
   from the **Ready** state to the **Pend** state.

-  Running→Ready:

   A process may change from the **Running** state to the **Ready**
   state in either of the following scenarios:

   1. After a process with a higher priority is created or restored,
      processes will be scheduled. The process with the highest priority
      in the ready list will change to the **Running** state, and the
      originally running process will change from the **Running** state
      to the **Ready** state.
   2. If a process has the **SCHED_RR** scheduling policy and shares the
      same priority with another process in the **Ready** state, this
      process will change from the **Running** state to the **Ready**
      state after its time slices are used up, and the other process
      with the same priority will change from the **Ready** state to the
      **Running** state.

-  Running→Zombies:

   After the main thread or all threads of a process are stopped, the
   process changes from the **Running** state to the **Zombies** state
   and waits for the parent process to reclaim resources.

When to Use
-----------

After processes are created, you can operate the resources only in your
own process space, except shared resources. In user space, processes can
be suspended, restored, and delayed. In addition, you can set and obtain
the scheduling priority and scheduling policy of processes. When a
process is terminated, it proactively releases its resources. However,
the PID resources of the process are reclaimed by the parent process via
**wait**/**waitpid** or when the parent process exits.

Available APIs
--------------

The following table describes the APIs provided by the process
management module of the OpenHarmony kernel.

**Table 1** APIs provided by the process management module

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row630210427446">

.. raw:: html

   <th class="cellrowborder" valign="top" width="13.020000000000001%" id="mcps1.2.5.1.1">

.. raw:: html

   <p id="p1430244284410">

Category

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="23.150000000000002%" id="mcps1.2.5.1.2">

.. raw:: html

   <p id="p9302164284416">

Function

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="28.93%" id="mcps1.2.5.1.3">

.. raw:: html

   <p id="p730211427445">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="34.9%" id="mcps1.2.5.1.4">

.. raw:: html

   <p id="p1430214294419">

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

   <tr id="row12302642134414">

.. raw:: html

   <td class="cellrowborder" rowspan="13" valign="top" width="13.020000000000001%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p430213427443">

Process

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="23.150000000000002%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p10302154219449">

fork

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.93%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p930218420449">

Creates a new process.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.9%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p230224211440">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row20302154218442">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p130314204419">

exit

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p53031426443">

Exits the process.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p113034423445">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row930314421443">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p13303124213442">

atexit

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1330324210442">

Registers the callback that will be called when the process is
terminated normally.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p3303144264414">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row113039426449">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1630394220444">

abort

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p133037421441">

Terminates the process.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p1330334216449">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1330317422445">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p113036427441">

getpid

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p17303642194412">

Obtains the process ID.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p14304942104420">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row3304204254412">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1430404218442">

getppid

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p9304134217443">

Obtains the parent process ID.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p1530418423449">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row610863618327">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p110811368324">

getpgrp

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p51091436133217">

Obtains the ID of the process group of the calling process.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p31094364326">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2379940183217">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1380184016329">

getpgid

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p8121101872215">

Obtains the process group ID of the process identified by pid.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p63802401326">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1981395963412">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p4814559123412">

setpgrp

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p171226183225">

Sets the process group ID of the calling process.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p8814959123416">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row194862793516">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p5948162703511">

setpgid

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p7122131852218">

Sets the process group ID of the process identified by pid.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p1994915279352">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row10304742114410">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p530474264418">

kill

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p2304174213441">

Sends a signal to a specified process.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <ul id="ul949915272011">

.. raw:: html

   <li>

Only signals 1 to 30 can be sent.

.. raw:: html

   </li>

.. raw:: html

   <li>

The default behavior for signals does not include STOP and CONTINUE and
terminates the process without a core dump.

.. raw:: html

   </li>

.. raw:: html

   <li>

SIGSTOP, SIGKILL, and SIGCONT cannot be masked.

.. raw:: html

   </li>

.. raw:: html

   <li>

After an asynchronous signal is sent to a process, the signal callback
is invoked only after the process is scheduled. For the sake of
security, the process can be killed only by itself, and the kernel
cannot forcibly kill the process by sending signals.

.. raw:: html

   </li>

.. raw:: html

   <li>

After the process is killed, SIGCHLD is sent to its parent process. The
sending action cannot be canceled.

.. raw:: html

   </li>

.. raw:: html

   <li>

A sleeping process cannot be woken up by a signal.

.. raw:: html

   </li>

.. raw:: html

   </ul>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1430454210446">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p830494212443">

wait

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p230464294410">

Waits for any child process to terminate and reclaims its resources.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p12512337347">

The status value is defined by the following macros:

.. raw:: html

   </p>

.. raw:: html

   <ul id="ul13349201524417">

.. raw:: html

   <li>

WIFEXITED(status): If the child process terminates normally, true is
returned. Otherwise, false is returned.

.. raw:: html

   </li>

.. raw:: html

   <li>

WEXITSTATUS(status): If WIFEXITED(status) is true, this macro can be
used to obtain the exit code that the child process passed to exit().

.. raw:: html

   </li>

.. raw:: html

   <li>

WTERMSIG(status): If a child process terminates abnormally, the child
process exit code obtained by the parent process through WTERMSIG is
always SIGUSR2. This is the only case supported.

.. raw:: html

   </li>

.. raw:: html

   <li>

The following operations are not supported: WIFSTOPPED, WSTOPSIG,
WCOREDUMP, and WIFCONTINUED.

.. raw:: html

   </li>

.. raw:: html

   </ul>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row13041742134416">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1530434217444">

waitpid

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p130564294420">

Waits for a specified child process to terminate and reclaims its
resources.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p969785263816">

The options to control the function behavior do not support WUNTRACED
and WCONTINUED.

.. raw:: html

   </p>

.. raw:: html

   <p id="p8497151543715">

The status value is defined by the following macros:

.. raw:: html

   </p>

.. raw:: html

   <ul id="ul7243133164416">

.. raw:: html

   <li>

WIFEXITED(status): If the child process terminates normally, true is
returned. Otherwise, false is returned.

.. raw:: html

   </li>

.. raw:: html

   <li>

WEXITSTATUS(status): If WIFEXITED(status) is true, this macro can be
used to obtain the exit code that the child process passed to exit().

.. raw:: html

   </li>

.. raw:: html

   <li>

WTERMSIG(status): If a child process terminates abnormally, the child
process exit code obtained by the parent process through WTERMSIG is
always SIGUSR2. This is the only case supported.

.. raw:: html

   </li>

.. raw:: html

   <li>

The following operations are not supported: WIFSTOPPED, WSTOPSIG,
WCOREDUMP, and WIFCONTINUED.

.. raw:: html

   </li>

.. raw:: html

   </ul>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row4305194294417">

.. raw:: html

   <td class="cellrowborder" rowspan="10" valign="top" width="13.020000000000001%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p5305194264419">

Scheduling

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="23.150000000000002%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p630544224416">

getpriority

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.93%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p174915589591">

Obtains the static priority of a specified ID.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" rowspan="2" valign="top" width="34.9%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <ul id="ul185518513478">

.. raw:: html

   <li>

PRIO_PGRP and PRIO_USER are not supported.

.. raw:: html

   </li>

.. raw:: html

   </ul>

.. raw:: html

   <ul id="ul85091358174711">

.. raw:: html

   <li>

The priority to obtain and set refers to the static priority. The
dynamic priority is not involved.

.. raw:: html

   </li>

.. raw:: html

   </ul>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row930511425448">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1730524217448">

setpriority

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p17750205817594">

Sets the static priority of a specified ID.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2305174216445">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p7305942104417">

sched_rr_get_interval

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1362018100165">

Obtains the execution time limit of a process.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p5306134212447">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row33061042104416">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p143061642164412">

sched_yield

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1262017102164">

Yields the running process.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p14306134220441">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row11306134234417">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p11306184264417">

sched_get_priority_max

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p123062423446">

Obtains the maximum static priority that can be used for a process.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" rowspan="4" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p11306154210440">

The scheduling policy can only be SCHED_FIFO or SCHED_RR.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row15306242124413">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p430612427448">

sched_get_priority_min

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p430618428442">

Obtains the minimum static priority that can be used for a process.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row730610428448">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p230684284419">

sched_getscheduler

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p20306184224417">

Obtains the scheduling policy of a process.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row630764215441">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1530719424444">

sched_setscheduler

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p13072042104416">

Sets a scheduling policy for a process.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row3307184274411">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p12307114274419">

sched_getparam

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p9307104210441">

Obtains scheduling parameters of a process.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p163071842194417">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row18307104210449">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1230784264419">

sched_setparam

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1530784215445">

Sets scheduling parameters related to a scheduling policy for a process.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p730714264415">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row17412918306">

.. raw:: html

   <td class="cellrowborder" rowspan="6" valign="top" width="13.020000000000001%" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p8528162314312">

exec

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="23.150000000000002%" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1951498305">

execl

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.93%" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p1612191842215">

Executes a specified user program file in ELF format.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="34.9%" headers="mcps1.2.5.1.4 ">

.. raw:: html

   <p id="p11679610113215">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row16964151163015">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p1996413117300">

execle

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p104059331261">

Executes a specified user program file in ELF format.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p3209101117329">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row9418101418309">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p741881443010">

execlp

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p493315383264">

Executes a specified user program file in ELF format.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p8741121112325">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2058611176305">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p155869170309">

execv

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p1644334112613">

Executes a specified user program file in ELF format.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p423311211323">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row182359476306">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p202351547163016">

execve

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p13152444192616">

Executes a specified user program file in ELF format.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p148072123324">

N/A

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row14242145013304">

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 ">

.. raw:: html

   <p id="p02437507305">

execvp

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 ">

.. raw:: html

   <p id="p06334469262">

Executes a specified user program file in ELF format.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 ">

.. raw:: html

   <p id="p333161353217">

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

.. |image1| image:: figures/en-us_image_0000001053930456.png
