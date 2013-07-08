usbtree
=======

Show USB devices (and associated disks and input devices) in tree format.

This is a replacement for the old "usbtree" command that stopped
working when /proc/bus/usb/devices went away. Although "lsusb -t"
produces almost the same output, it seems to have some issues ("No
such file or directory" errors).

This tool defaults to omitting interfaces and buses (which aren't of
much interest to most users), but does include things like disks,
inputs and TTYs that are found attached to USB devices.
