Magic Key Usage
===============

When to Use
-----------

When the system does not respond, you can use the magic key function to
check whether the system is locked and interrupted (the magic key also
does not respond) or view the system task running status.

If the interrupt is responded, you can use the magic key to check the
CPU usage (**cpup**) in the task information to find out the task that
occupies the CPU for a long period of time and causes other tasks in the
system not to respond. (Generally, the high-priority tasks always
preempt the CPU and cause the low-priority tasks not to respond.)

How to Use
----------

1. Configure macro **LOSCFG_ENABLE_MAGICKEY**.

The magic key depends on the **LOSCFG_ENABLE_MAGICKEY** macro. To use
the magic key, enable the **Enable MAGIC KEY** configuration item using
**menuconfig**.

Debug —> Enable MAGIC KEY

If this configuration item is disabled, the magic key is invalid.

   |image1| **NOTE:** 1. In **menuconfig**, you can move the cursor to
   **LOSCFG_ENABLE_MAGICKEY** and enter a question mark (?) to view the
   help information.

2. Press **Ctrl+R** to enable the magic key detection function.

When the UART or USB-to-virtual serial port is connected, press
**Ctrl+R** to enable the magic key detection function. The message
“Magic key on” is displayed. After you press **Ctrl+R** again, the magic
key detection function is disabled, and message “Magic key off” is
displayed. The functions of the magic key are as follows:

-  **Ctrl+Z**: help key, which is used to display the brief introduction
   to related magic keys.

-  **Ctrl+T**: displays task information.

-  **Ctrl+P**: The system proactively enters the panic state. After the
   panic-related information is printed, the system is suspended.

-  **Ctrl+E**: The system checks the integrity of the memory pool. If an
   error is detected, the system displays an error message. If no error
   is detected, the system displays “system memcheck over, all passed!”.

..

   |image2| **NOTICE:** When the magic key detection function is enabled
   and special characters need to be entered through the UART or
   USB-to-virtual serial port, ensure that the special characters are
   not the same as the magic key values. Otherwise, the magic key may be
   triggered by mistake, which may cause errors in the original design.

.. |image1| image:: public_sys-resources/icon-note.gif
.. |image2| image:: public_sys-resources/icon-notice.gif
