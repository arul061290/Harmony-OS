Shell Command Development Guidelines
====================================

Development Guidelines
----------------------

You can perform the following operations to add shell commands:

1. Include the following header files:

   ::

      #include "shell.h"
      #include "shcmd.h"

2. Register commands. You can register commands either statically or
   dynamically when the system is running. In most cases, static
   registration is widely used by common system commands, and dynamic
   registration is widely used by user commands.

   1. Static registration:

      1. Register a command using a macro.

         The prototype of the macro is as follows:

         SHELLCMD_ENTRY(l, cmdType, cmdKey, paraNum, cmdHook)

         **Table 1** Parameters of the SHELLCMD_ENTRY macro

         .. raw:: html

            <table>

         .. raw:: html

            <thead align="left">

         .. raw:: html

            <tr id="row209856358456">

         .. raw:: html

            <th class="cellrowborder" valign="top" width="20.91%" id="mcps1.2.3.1.1">

         .. raw:: html

            <p id="p998583517456">

         Parameter

         .. raw:: html

            </p>

         .. raw:: html

            </th>

         .. raw:: html

            <th class="cellrowborder" valign="top" width="79.09%" id="mcps1.2.3.1.2">

         .. raw:: html

            <p id="p169851735174511">

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

            <tr id="row13985153574517">

         .. raw:: html

            <td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.2.3.1.1 ">

         .. raw:: html

            <p id="p6985113513452">

         l

         .. raw:: html

            </p>

         .. raw:: html

            </td>

         .. raw:: html

            <td class="cellrowborder" valign="top" width="79.09%" headers="mcps1.2.3.1.2 ">

         .. raw:: html

            <p id="p998573514457">

         Indicates the global variable name to be passed during the
         static registration. Note that the name cannot be the same as
         other symbol names in the system.

         .. raw:: html

            </p>

         .. raw:: html

            </td>

         .. raw:: html

            </tr>

         .. raw:: html

            <tr id="row398513594518">

         .. raw:: html

            <td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.2.3.1.1 ">

         .. raw:: html

            <p id="p59856356450">

         cmdType

         .. raw:: html

            </p>

         .. raw:: html

            </td>

         .. raw:: html

            <td class="cellrowborder" valign="top" width="79.09%" headers="mcps1.2.3.1.2 ">

         .. raw:: html

            <p id="p119859355458">

         Indicates the command type.

         .. raw:: html

            </p>

         .. raw:: html

            <ul id="ul11135144114816">

         .. raw:: html

            <li>

         .. raw:: html

            <p id="p21351144488">

         CMD_TYPE_EX: does not support standard command parameters and
         will mask the command keywords you entered. For example, if you
         enter ls /ramfs, only /ramfs will be passed to the registration
         function, and the ls command keyword will be masked.

         .. raw:: html

            </p>

         .. raw:: html

            </li>

         .. raw:: html

            <li>

         .. raw:: html

            <p id="p21353410482">

         CMD_TYPE_STD: supports standard command parameters. All the
         characters you entered will be passed to the registration
         function after being parsed.

         .. raw:: html

            </p>

         .. raw:: html

            </li>

         .. raw:: html

            </ul>

         .. raw:: html

            </td>

         .. raw:: html

            </tr>

         .. raw:: html

            <tr id="row20985153524519">

         .. raw:: html

            <td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.2.3.1.1 ">

         .. raw:: html

            <p id="p1098693510451">

         cmdKey

         .. raw:: html

            </p>

         .. raw:: html

            </td>

         .. raw:: html

            <td class="cellrowborder" valign="top" width="79.09%" headers="mcps1.2.3.1.2 ">

         .. raw:: html

            <p id="p11986735144514">

         Indicates the command keyword, which is the name used to access
         a shell function.

         .. raw:: html

            </p>

         .. raw:: html

            </td>

         .. raw:: html

            </tr>

         .. raw:: html

            <tr id="row1398683511450">

         .. raw:: html

            <td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.2.3.1.1 ">

         .. raw:: html

            <p id="p598613359451">

         paraNum

         .. raw:: html

            </p>

         .. raw:: html

            </td>

         .. raw:: html

            <td class="cellrowborder" valign="top" width="79.09%" headers="mcps1.2.3.1.2 ">

         .. raw:: html

            <p id="p11986535144516">

         Indicates the maximum number of input parameters in the
         execution function to be invoked. This parameter is not
         supported currently.

         .. raw:: html

            </p>

         .. raw:: html

            </td>

         .. raw:: html

            </tr>

         .. raw:: html

            <tr id="row39861935154516">

         .. raw:: html

            <td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.2.3.1.1 ">

         .. raw:: html

            <p id="p5986735114518">

         cmdHook

         .. raw:: html

            </p>

         .. raw:: html

            </td>

         .. raw:: html

            <td class="cellrowborder" valign="top" width="79.09%" headers="mcps1.2.3.1.2 ">

         .. raw:: html

            <p id="p398683574515">

         Indicates the address of the execution function, that is, the
         function that is actually executed by the command.

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

         Example: SHELLCMD_ENTRY(ls_shellcmd, CMD_TYPE_EX, “ls”, XARGS,
         (CMD_CBK_FUNC)osShellCmdLs)

      2. Add the required options to the
         **build/mk/liteos_tables_ldflags.mk** file.

         For example, when registering the **ls** command, add
         **-uls_shellcmd** to the **build/mk/liteos_tables_ldflags.mk**
         file. **-u** is followed by the first parameter of
         **SHELLCMD_ENTRY**.

   2. Dynamic registration:

      The prototype of the function to register is as follows:

      UINT32 osCmdReg(CmdT ype cmdType, CHAR \*cmdKey, UINT32 paraNum,
      CmdCallBackFunc cmdProc)

      **Table 2** Parameters of UINT32 osCmdReg

      .. raw:: html

         <table>

      .. raw:: html

         <thead align="left">

      .. raw:: html

         <tr id="row1644693318490">

      .. raw:: html

         <th class="cellrowborder" valign="top" width="20.91%" id="mcps1.2.3.1.1">

      .. raw:: html

         <p id="p1644618337493">

      Parameter

      .. raw:: html

         </p>

      .. raw:: html

         </th>

      .. raw:: html

         <th class="cellrowborder" valign="top" width="79.09%" id="mcps1.2.3.1.2">

      .. raw:: html

         <p id="p444603317491">

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

         <tr id="row844643374912">

      .. raw:: html

         <td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.2.3.1.1 ">

      .. raw:: html

         <p id="p14446133319498">

      cmdType

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         <td class="cellrowborder" valign="top" width="79.09%" headers="mcps1.2.3.1.2 ">

      .. raw:: html

         <p id="p174461339496">

      Indicates the command type.

      .. raw:: html

         </p>

      .. raw:: html

         <ul id="ul1244773317496">

      .. raw:: html

         <li>

      .. raw:: html

         <p id="p1844719331495">

      CMD_TYPE_EX: does not support standard command parameters and will
      mask the command keywords you entered. For example, if you enter
      ls /ramfs, only /ramfs will be passed to the registration
      function, and the ls command keyword will be masked.

      .. raw:: html

         </p>

      .. raw:: html

         </li>

      .. raw:: html

         <li>

      .. raw:: html

         <p id="p20447143315498">

      CMD_TYPE_STD: supports standard command parameters. All the
      characters you entered will be passed to the registration function
      after being parsed.

      .. raw:: html

         </p>

      .. raw:: html

         </li>

      .. raw:: html

         </ul>

      .. raw:: html

         </td>

      .. raw:: html

         </tr>

      .. raw:: html

         <tr id="row14471733184915">

      .. raw:: html

         <td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.2.3.1.1 ">

      .. raw:: html

         <p id="p744783319494">

      cmdKey

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         <td class="cellrowborder" valign="top" width="79.09%" headers="mcps1.2.3.1.2 ">

      .. raw:: html

         <p id="p18447833124914">

      Indicates the command keyword, which is the name used to access a
      shell function.

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         </tr>

      .. raw:: html

         <tr id="row17447143317495">

      .. raw:: html

         <td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.2.3.1.1 ">

      .. raw:: html

         <p id="p174477331495">

      paraNum

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         <td class="cellrowborder" valign="top" width="79.09%" headers="mcps1.2.3.1.2 ">

      .. raw:: html

         <p id="p8447233184914">

      Indicates the maximum number of input parameters in the execution
      function to be invoked. This parameter is not supported currently.
      The default value is XARGS(0xFFFFFFFF).

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         </tr>

      .. raw:: html

         <tr id="row10447233174913">

      .. raw:: html

         <td class="cellrowborder" valign="top" width="20.91%" headers="mcps1.2.3.1.1 ">

      .. raw:: html

         <p id="p18447183334920">

      cmdHook

      .. raw:: html

         </p>

      .. raw:: html

         </td>

      .. raw:: html

         <td class="cellrowborder" valign="top" width="79.09%" headers="mcps1.2.3.1.2 ">

      .. raw:: html

         <p id="p44471533184912">

      Indicates the address of the execution function, that is, the
      function that is actually executed by the command.

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

      Example: osCmdReg(CMD_TYPE_EX, “ls”, XARGS,
      (CMD_CBK_FUNC)osShellCmdLs)

   ..

      |image1| **NOTE:** The command keyword must be unique.
      Specifically, two different commands cannot share the same command
      keyword. Otherwise, only one command is executed. When executing
      user commands sharing the same keyword, the shell executes only
      the first command in the **help** commands.

3. Use the following function prototype to add built-in commands:

   UINT32 osShellCmdLs(UINT32 argc, CHAR \**argv)

   **Table 3** Parameters of osShellCmdLs

   .. raw:: html

      <table>

   .. raw:: html

      <thead align="left">

   .. raw:: html

      <tr id="row84451058105117">

   .. raw:: html

      <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1">

   .. raw:: html

      <p id="p1644515855111">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </th>

   .. raw:: html

      <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2">

   .. raw:: html

      <p id="p18445145805113">

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

      <tr id="row194461458185112">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p64461158145120">

   argc

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p1844625885112">

   Indicates the number of parameters in the shell command.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row144620587511">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

   .. raw:: html

      <p id="p244625811517">

   argv

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

   .. raw:: html

      <p id="p11446958105119">

   Indicates a pointer array, where each element points to a string. You
   can determine whether to pass the command keyword to the registration
   function by specifying the command type.

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

4. Enter the shell command in either of the following methods:

   -  Enter the shell command in the serial port tool.

   -  Enter the shell command in the Telnet tool. For details, see
      `telnet <telnet.rst>`__.

.. |image1| image:: public_sys-resources/icon-note.gif
