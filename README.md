# pyvxbox
Python Bindings for vXboxInterface

This project is a thin wrapper around a C++ virtual
xbox controller library. This module searches for
the vXboxInterface.dll in its own directory.
Some information about ScpVbus and vXboxInterface can be
found here: http://vjoystick.sourceforge.net/site/index.php/vxbox.
Specifically, releases of the vXboxInterface can be found
at https://github.com/shauleiz/vXboxInterface/releases.
This project is similar in function to pyvjoy (a wrapper
around the vjoy library).

This library revolves around an XInputDevice object.
Example:

controller = pyvxbox.XInputDevice(1)
controller.PlugIn()
controller.SetBtn('A', True)
controller.SetBtn('A', False)
controller.UnPlug()

The above example creates a virtual controller for
port 1, plugs it in, presses and releases the A button,
and finally unplugs it.

Use this code however you like; I won't promise to look at
or maintain this project, but if I see pull request and have
time, I'll try to look at it.

Explicitly:

           DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE

Copyright (C) 2017 Alex Gonzales <musigonzales@gmail.com>

Everyone is permitted to copy and distribute verbatim or modified
copies of this license document, and changing it is allowed as long
as the name is changed.

           DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
  TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

 0. You just DO WHAT THE FUCK YOU WANT TO.
