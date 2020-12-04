pthread.h
=========

**Overview**\ 
--------------

**Related Modules:**

`PROCESS <process.md>`__

**Description:**

Provides process- and thread-related structures (providing fields such
as thread attributes) and functions (including the functions for
creating and destroying threads, and setting the thread detach state and
blocking conditions).

**Since:**

1.0

**Version:**

1.0

**Summary**\ 
-------------

Functions
---------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row629732592084831">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1674192319084831">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1966658112084831">

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

   <tr id="row1338231546084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1420505920084831">

pthread_create (pthread_t *thread, const pthread_attr_t*\ attr, void
*(*\ start_routine)(void *), void*\ arg)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p158737550084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1499526583084831">

Creates a thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row141995018084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p274339001084831">

pthread_detach (pthread_t thread)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1427776902084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1748908653084831">

Detaches a thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1707637780084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1336791060084831">

pthread_exit (void \*retval)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1404496180084831">

\_Noreturn void

.. raw:: html

   </p>

.. raw:: html

   <p id="p316311595084831">

Terminates the calling thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row275643329084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1240326946084831">

pthread_join (pthread_t thread, void \**retval)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1911776136084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1654684601084831">

Waits for a thread to terminate.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row500385784084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p246570847084831">

pthread_self (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1471574492084831">

pthread_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1250721980084831">

Obtains the ID of the calling thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1322849588084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1399150485084831">

pthread_equal (pthread_t t1, pthread_t t2)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1624582945084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p591628834084831">

Compares whether two thread IDs are equal.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1123516869084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p310019677084831">

pthread_setcancelstate (int state, int \*oldstate)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1375925438084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p13320449084831">

Sets the cancelability state for the calling thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row327124959084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p530598869084831">

pthread_setcanceltype (int type, int \*oldtype)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1155242778084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p343036429084831">

Sets the cancelability type for the calling thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1525994075084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p969747806084831">

pthread_testcancel (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p800889596084831">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p846143272084831">

Requests delivery of any pending cancellation request.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1419595392084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p478578056084831">

pthread_cancel (pthread_t thread)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1515902843084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p653290080084831">

Sends a cancellation request to a thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1340992926084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p322243165084831">

pthread_kill (pthread_t thread, int sig)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1739966800084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1903311140084831">

Sends a signal to a thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1494854668084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p962490977084831">

pthread_getschedparam (pthread_t thread, int *policy, struct
sched_param*\ param)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1988845719084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1595724400084831">

Obtains the scheduling policy and parameters of a thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1065579712084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p491695424084831">

pthread_setschedparam (pthread_t thread, int policy, const struct
sched_param \*param)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p258015925084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1017117311084831">

Sets a scheduling policy and parameters for a thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1950245672084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p909485016084831">

pthread_setschedprio (pthread_t thread, int prio)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1532326522084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p2136329142084831">

Sets a static scheduling priority for a thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2022991064084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p636419163084831">

pthread_once (pthread_once_t *once_control, void(*\ init_routine)(void))

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p645947359084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1460939055084831">

Enables the initialization function to be called only once.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1755466003084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p814549636084831">

pthread_mutex_init (pthread_mutex_t \*__restrict m, const
pthread_mutexattr_t \*__restrict a)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1141511484084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1004020697084831">

Initializes a mutex.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1422353289084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1102319312084831">

pthread_mutex_lock (pthread_mutex_t \*m)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p238347624084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1153626701084831">

Locks a mutex.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1859001340084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p993807004084831">

pthread_mutex_unlock (pthread_mutex_t \*m)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p370172725084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p187360236084831">

Unlocks a mutex.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1235779003084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p438775945084831">

pthread_mutex_trylock (pthread_mutex_t \*m)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2133606930084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p660242088084831">

Attempts to lock a mutex.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row894940980084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1879399869084831">

pthread_mutex_timedlock (pthread_mutex_t \*__restrict m, const struct
timespec \*__restrict at)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1030474491084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1812469817084831">

Blocks the calling thread to lock a mutex.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row820503766084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p649748259084831">

pthread_mutex_destroy (pthread_mutex_t \*m)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p544988886084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1306499301084831">

Destroys a mutex.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1907510046084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p722057731084831">

pthread_cond_init (pthread_cond_t \*__restrict c, const
pthread_condattr_t \*__restrict a)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p415585396084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p327079038084831">

Initializes a condition variable.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row821779608084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1329383228084831">

pthread_cond_destroy (pthread_cond_t \*c)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p569925612084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p411021103084831">

Destroys a condition variable.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row382249280084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p522537576084831">

pthread_cond_wait (pthread_cond_t \*__restrict c, pthread_mutex_t
\*__restrict m)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p564636238084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p441388351084831">

Blocks the calling thread to wait for the condition set by
pthread_con_signal().

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1755515377084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p314053802084831">

pthread_cond_timedwait (pthread_cond_t \*__restrict c, pthread_mutex_t
\*__restrict m, const struct timespec \*__restrict ts)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1291622451084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1208583012084831">

Blocks the calling thread to wait for the condition set by
pthread_con_signal() for a period of time specified by ts.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1774150005084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p788467754084831">

pthread_cond_broadcast (pthread_cond_t \*c)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1063472185084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1860563641084831">

Unblocks all threads that are currently blocked on the condition
variable cond.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row108169007084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1194653832084831">

pthread_cond_signal (pthread_cond_t \*c)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1938786207084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p783221724084831">

Unblocks a thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1106926559084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p223804769084831">

pthread_rwlock_init (pthread_rwlock_t \*__restrict rw, const
pthread_rwlockattr_t \*__restrict a)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p338836281084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1909951793084831">

Initializes a read-write lock.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row580922433084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p844764665084831">

pthread_rwlock_destroy (pthread_rwlock_t \*rw)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2029789656084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1476903852084831">

Destroys a read-write lock.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2041332948084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1589325106084831">

pthread_rwlock_rdlock (pthread_rwlock_t \*rw)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1379663212084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p83981748084831">

Applies a read lock to a read-write lock.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row768609467084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p904300510084831">

pthread_rwlock_tryrdlock (pthread_rwlock_t \*rw)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1831401027084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1192924920084831">

Attempts to apply a read lock to a read-write lock.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1195914500084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p123286682084831">

pthread_rwlock_timedrdlock (pthread_rwlock_t \*__restrict rw, const
struct timespec \*__restrict at)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p770106311084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p2053532631084831">

Blocks the calling thread to lock a read-write lock for reading.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1753084030084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1813612984084831">

pthread_rwlock_wrlock (pthread_rwlock_t \*rw)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1492185166084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1267324456084831">

Applies a write lock to a read-write lock.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row918921628084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1230907731084831">

pthread_rwlock_trywrlock (pthread_rwlock_t \*rw)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p121975858084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1470047318084831">

Attempts to apply a write lock to a read-write lock.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1830089508084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p402225811084831">

pthread_rwlock_timedwrlock (pthread_rwlock_t \*__restrict rw, const
struct timespec \*__restrict at)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2120360381084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1059318709084831">

Blocks the calling thread to lock a read-write lock for writing.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1333552980084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p334579078084831">

pthread_rwlock_unlock (pthread_rwlock_t \*rw)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1745255417084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p483843727084831">

Unlocks a read-write lock.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row924591775084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1274497422084831">

pthread_spin_init (pthread_spinlock_t \*s, int shared)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1372482964084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p692957053084831">

Initializes a spin lock.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1274795186084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p720730290084831">

pthread_spin_destroy (pthread_spinlock_t \*s)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p591624441084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1853804188084831">

Destroys a spin lock.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row643274050084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2060205142084831">

pthread_spin_lock (pthread_spinlock_t \*s)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p32638432084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1599634186084831">

Locks a spin lock.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row748217708084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p973610773084831">

pthread_spin_trylock (pthread_spinlock_t \*s)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p521643920084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p416711561084831">

Attempts to lock a spin lock.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row342366889084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p626798791084831">

pthread_spin_unlock (pthread_spinlock_t \*s)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1723386011084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p42497869084831">

Unlocks a spin lock.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1517454319084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1307025977084831">

pthread_barrier_init (pthread_barrier_t \*__restrict b, const
pthread_barrierattr_t \*__restrict a, unsigned count)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p432503584084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1750743122084831">

Initializes a barrier.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1721000148084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p213461963084831">

pthread_barrier_destroy (pthread_barrier_t \*b)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p405612242084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1649906970084831">

Destroys a barrier.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row582820070084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p814744780084831">

pthread_barrier_wait (pthread_barrier_t \*b)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p624337739084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p55238447084831">

Synchronizes participating threads at a barrier.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row399081808084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2133870241084831">

pthread_key_create (pthread_key_t *key, void(*\ destructor)(void \*))

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2069186700084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1250767680084831">

Creates a key for thread data.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row524405397084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p261665856084831">

pthread_key_delete (pthread_key_t key)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1803698431084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1781913900084831">

Deletes a key for thread data.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1490494588084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1490043769084831">

pthread_getspecific (pthread_key_t key)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p819819440084831">

void \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p316080855084831">

Obtains specific thread data.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row97121947084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1657109082084831">

pthread_setspecific (pthread_key_t key, const void \*value)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1738412280084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1612135869084831">

Sets specific thread data.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1312726078084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2088739510084831">

pthread_attr_init (pthread_attr_t \*attr)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1405400537084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p600399390084831">

Initializes a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1715876912084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1406195704084831">

pthread_attr_destroy (pthread_attr_t \*attr)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p70541783084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p968125547084831">

Destroys a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1547551324084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p231857140084831">

pthread_attr_getguardsize (const pthread_attr_t *attr,
size_t*\ guardsize)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p329296708084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p617325603084831">

Obtains the guard size of a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row345992839084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1235092972084831">

pthread_attr_setguardsize (pthread_attr_t \*attr, size_t guardsize)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1973287078084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1291680086084831">

Sets the guard size for a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1887143004084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p592771056084831">

pthread_attr_getstacksize (const pthread_attr_t *attr,
size_t*\ stacksize)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p756280506084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1956529050084831">

Obtains the stack size of a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1108864808084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p44554055084831">

pthread_attr_setstacksize (pthread_attr_t \*attr, size_t stacksize)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2103548279084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p520366593084831">

Sets the stack size for a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row364800129084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p699710753084831">

pthread_attr_getdetachstate (const pthread_attr_t *attr,
int*\ detachstate)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p190337036084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1859032902084831">

Obtains the detach state of a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row555016421084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1629362014084831">

pthread_attr_setdetachstate (pthread_attr_t \*attr, int detachstate)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1167242567084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p661431418084831">

Sets the detach state for a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row149048428084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p881965056084831">

pthread_attr_getstack (const pthread_attr_t \*attr, void \**stackaddr,
size_t \*stacksize)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1048339901084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p672582673084831">

Obtains stack attributes of a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1861962987084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1130614847084831">

pthread_attr_setstack (pthread_attr_t *attr, void*\ stackaddr, size_t
stacksize)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p441152324084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p602856745084831">

Sets stack attributes for a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row889935092084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1480372976084831">

pthread_attr_getscope (const pthread_attr_t *arrt, int*\ scope)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1535245185084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1305851051084831">

Obtains contention scope attributes of a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1958429859084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p736339643084831">

pthread_attr_setscope (pthread_attr_t \*arrt, int scope)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1274973072084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p2007504309084831">

Sets contention scope attributes for a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1913027630084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1269545958084831">

pthread_attr_getschedpolicy (const pthread_attr_t *attr,
int*\ schedpolicy)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2061771971084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1049047212084831">

Obtains scheduling policy attributes of a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row397695594084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p483253293084831">

pthread_attr_setschedpolicy (pthread_attr_t \*attr, int schedpolicy)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1362811922084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1501814409084831">

Sets scheduling policy attributes for a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row48985152084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p691822041084831">

pthread_attr_getschedparam (const pthread_attr_t *attr, struct
sched_param*\ param)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1534724584084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p949790474084831">

Obtains scheduling parameter attributes of a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1642692139084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p106462006084831">

pthread_attr_setschedparam (pthread_attr_t *attr, const struct
sched_param*\ param)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p894355443084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p263621543084831">

Sets scheduling parameter attributes for a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1743889236084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1479594472084831">

pthread_attr_getinheritsched (const pthread_attr_t *attr,
int*\ inheritsched)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1433533892084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1814160414084831">

Obtains inherit scheduler attributes of a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1541463778084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p50885123084831">

pthread_attr_setinheritsched (pthread_attr_t \*attr, int inheritsched)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p405131685084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p547736646084831">

Sets inherit scheduler attributes for a thread attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row985735702084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p620580933084831">

pthread_mutexattr_destroy (pthread_mutexattr_t \*attr)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1877499107084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p557249148084831">

Destroys a mutex attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1834053130084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1602544983084831">

pthread_mutexattr_gettype (const pthread_mutexattr_t \*__restrict attr,
int \*__restrict type)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1933104397084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1656021059084831">

Obtains the mutex type attribute.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1335849793084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2051563756084831">

pthread_mutexattr_init (pthread_mutexattr_t \*attr)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1383560030084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p916298987084831">

Initializes a mutex attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1680577948084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1360726988084831">

pthread_mutexattr_settype (pthread_mutexattr_t \*attr, int type)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1787708123084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1889169699084831">

Sets the mutex type attribute.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1937461344084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1766030892084831">

pthread_condattr_init (pthread_condattr_t \*a)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p393537776084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p124172070084831">

Initializes a condition variable attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row842013558084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1102933516084831">

pthread_condattr_destroy (pthread_condattr_t \*a)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1948093895084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p645025015084831">

Destroys a condition variable attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1194238766084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p61272094084831">

pthread_condattr_setclock (pthread_condattr_t \*a, clockid_t clk)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p498304829084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p675838331084831">

Sets a clock for a condition variable attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1204595935084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p451371700084831">

pthread_condattr_getclock (const pthread_condattr_t \*__restrict a,
clockid_t \*__restrict clk)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p978804122084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p117694865084831">

Obtains the clock of a condition variable attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row865642635084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p94339740084831">

pthread_rwlockattr_init (pthread_rwlockattr_t \*attr)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1884251426084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1300943600084831">

Initializes a read-write lock attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1025309419084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1488661024084831">

pthread_rwlockattr_destroy (pthread_rwlockattr_t \*attr)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p889346200084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1292284431084831">

Destroys a read-write lock attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1000717963084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p456292394084831">

pthread_barrierattr_destroy (pthread_barrierattr_t \*a)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p919171016084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1681371465084831">

Destroys a barrier attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1007660618084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1372238609084831">

pthread_barrierattr_init (pthread_barrierattr_t \*a)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p643437975084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p2079628309084831">

Initializes a barrier attribute object.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1737437712084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p512421754084831">

pthread_atfork (void(*prepare)(void), void(*\ parent)(void),
void(*child)(void))

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p612378556084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1117042248084831">

Registers a fork handler to be called before and after fork().

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1035158548084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1805223837084831">

pthread_cleanup_push (void(*routine)(void*), void \*arg)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p637442076084831">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p881017134084831">

Pushes the routine to the top of the clean-up handler stack.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row61896709084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p270282937084831">

pthread_cleanup_pop (int execute)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1174941274084831">

void

.. raw:: html

   </p>

.. raw:: html

   <p id="p907610598084831">

Removes the routine at the top of the clean-up handler stack.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row81027234084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p180392888084831">

pthread_getattr_np (pthread_t thread, pthread_attr_t \*attr)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p759119449084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p2024641697084831">

Obtains the attributes of a created thread.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row213558680084831">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1245593825084831">

pthread_setname_np (pthread_t pthread, const char \*name)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p790630260084831">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1964451861084831">

Sets the thread name.

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
