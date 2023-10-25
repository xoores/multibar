multibar(1)
==========

SYNOPSIS
--------
**multibar** [*OPTIONS*]... [*BAR*]

DESCRIPTION
-----------
Multibar is a fork of Polybar poject. It aims to help users build beautiful and highly customizable status bars for their desktop environment, without the need of having a black belt in shell scripting.
If the *BAR* argument is not provided and the configuration file only contains one bar definition, multibar will display this bar.

OPTIONS
-------

.. program:: multibar

.. option:: -h, --help

   Display help text and exit

.. option:: -v, --version

   Display build details and exit
.. option:: -l, --log=LEVEL

   | Set the logging verbosity (default: **notice**)
   | *LEVEL* is one of: error, warning, notice, info, trace
.. option:: -q, --quiet

   Be quiet (will override -l)
.. option:: -c, --config=FILE

   Specify the path to the configuration file. By default, the configuration file is loaded from:

   * ``$XDG_CONFIG_HOME/multibar/config``
   * ``$XDG_CONFIG_HOME/multibar/config.ini``
   * ``$HOME/.config/multibar/config``
   * ``$HOME/.config/multibar/config.ini``
   * ``$XDG_CONFIG_DIRS/multibar/config.ini``
   * ``/etc/xdg/multibar/config.ini`` (only if ``XDG_CONFIG_DIRS`` is not set)
   * ``/etc/multibar/config.ini``
.. option:: -r, --reload

   Reload the application when the config file has been modified
.. option:: -d, --dump=PARAM

   Print the value of the specified parameter *PARAM* in bar section and exit
.. option:: -m, --list-monitors

   | Print list of available monitors and exit.
   | If some monitors are cloned, this will exclude all but one of them.
   | If multibar was compiled with RandR monitor support, only monitors are listed and not physical outputs.
.. option:: -M, --list-all-monitors

   | Print list of all available monitors and exit.
   | This includes cloned monitors as well as both physical outputs and RandR monitors (if supported).
   | Only the names listed here can be used as monitor names in multibar.
.. option:: -w, --print-wmname

   Print the generated *WM_NAME* and exit
.. option:: -s, --stdout

   Output the data to stdout instead of drawing it to the X window
.. option:: -p, --png=FILE

   Save png snapshot to *FILE* after running for 3 seconds

AUTHORS
-------
| Multibar is maintained by Xoores.
| Polybar was created by Michael Carlberg and is currently maintained by Patrick Ziegler.

REPORTING BUGS
--------------
Report issues on GitHub <https://github.com/xoores/multibar>

SEE ALSO
--------
.. only:: man

  :manpage:`multibar-msg`\(1),
  :manpage:`multibar`\(5)


.. only:: not man

  :doc:`multibar-msg.1`,
  :doc:`multibar.5`

| Full documentation at: <https://github.com/xoores/multibar>
| Polybar wiki: <https://github.com/polybar/polybar/wiki>
