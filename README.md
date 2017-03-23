my-lcd4linux-conf
=================
My lcd4linux.conf for a very small, cheap picture frame display (Pearl 2,4" Appotech AX206) on a Seagate Dockstar/Raspberry
Pi/Banana Pi.

This is just an example project to get used to GitHub.

Links/Credits
-------------
- lcd4linux: https://lcd4linux.bulix.org/
- DPFs on Seagate Dockstar: http://forum.doozan.com/list.php?9
- AX206 Hack: https://sourceforge.net/projects/dpf-ax/
- More on using an AX206: http://picframe.spritesserver.nl/wiki/index.php/DPF_with_AppoTech_AX206

Generate a specific configuration
---------------------------------

Because many definitions are identical across my little machines, a master configuration is held in `lcd4linux.master.conf` 
using `#ifeq TARGET` blocks to differentiate between predefined hardware sections.

Run `gpp lcd4linux.master.conf > lcd4linux.conf` to get a usable target/layout specific configuration file.

Pictures
--------

![Sample DPF display](https://github.com/hkramski/my-lcd4linux-conf/blob/master/demo-dpf-lcd4l-dockstar.png "Sample DPF display")

![Hardware](https://github.com/hkramski/my-lcd4linux-conf/blob/master/demo-dpf-bananapi.jpg "Hardware")
