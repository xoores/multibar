multibar-msg(1)
==============

SYNOPSIS
--------
| **multibar-msg** [*OPTIONS*] **action** *action-string*
| **multibar-msg** [*OPTIONS*] **action** *module* *action* [*data*]
| **multibar-msg** [*OPTIONS*] **cmd** *command*

DESCRIPTION
-----------
Polybar allows external control through *actions* and *commands*.
Actions control individual modules and commands control the bar itself.

The full IPC documentation is linked at the end of this document.

The available actions depend on the target module.
For actions, the payload is either a single action string or the module name,
the action name, and the optional data string specified separately.

In order for **multibar-msg** being able to send a message to a running
**polybar** process, the bar must have IPC enabled and both **multibar-msg** and
**polybar** must run under the same user.

OPTIONS
-------

.. program:: multibar-msg

.. option:: -h, --help

   Display help text and exit

.. option:: -p PID

   Send message only to **multibar** process running under the given process ID.
   If not specified, the message is sent to all running **multibar** processes.

EXAMPLES
--------

**multibar-msg** **cmd** *quit*
  Terminate all running **multibar** instances.

**multibar-msg** **action** *mymodule* *module_hide*

**multibar-msg** **action** "*#mymodule.module_hide*"
  Hide the module named *mymodule*.
  The first variant specifies the module and action names separately, the second uses an action string.

AUTHORS
-------
| Multibar is maintained by Xoores.
| Polybar was created by Michael Carlberg and is currently maintained by Patrick Ziegler.

SEE ALSO
--------
.. only:: man

  :manpage:`multibar`\(1),
  :manpage:`multibar`\(5)

  | IPC documentation: <https://polybar.rtfd.org/en/stable/user/ipc.html>


.. only:: not man

  :doc:`multibar.1`,
  :doc:`multibar.5`

  :doc:`/user/ipc`
