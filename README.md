![dwm](/dwm.png)


My build of dwm
============================
dwm is an extremely fast, small, and dynamic window manager for X.

This custom version is patched with full-gaps and a command to take screenshots.


Requirements
------------
In order to build dwm you need the Xlib header files.
You will also need FontAwesome Brands 400 and Regular 900 to see the icons.
To take screenshots, install scrot and press print-screen.
THe script takes your screenshots and puts them in ~/Pictures

    sudo apt install install

Installation
------------
Edit config.mk to match your local setup (dwm is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install dwm:

    sudo make clean install


Running dwm
-----------
Add the following line to your .xinitrc to start dwm using startx:

    exec dwm

In order to connect dwm to a specific display, make sure that
the DISPLAY environment variable is set correctly, e.g.:

    DISPLAY=foo.bar:1 exec dwm

(This will start dwm on display :1 of the host foo.bar.)


Configuration
-------------
The configuration of dwm is done by creating a custom config.h
and (re)compiling the source code.
