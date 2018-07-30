ams-68k-bin
===========

AMS is the [Advanced Mac Substitute][AMS], a trap-level emulator for Mac OS.

This repository contains various 68K executables needed to run Mac apps using AMS.

Applications
------------

  * **TestApp** is a very basic Mac application that displays a movable, resizable window.
  * **NyanCat** is a black and white adaptation of Christopher Torres' Nyan Cat animation.
  * **IAGO** is a Reversi game released to the public domain by David Reed in 1984.

Modules
-------

  * `ams-core` consists of anything not covered below.
  * `ams-fs` implements the File Manager.
  * `ams-rsrc` implements the Resource Manager.
  * `ams-pack` contains the Package Manager (but no actual packages).
  * `ams-seg` contains the Segment Loader.
  * `ams-qd` provides QuickDraw and the Font Manager.
  * `ams-ui` includes the Window Manager, Control Manager, and Menu Manager.
  
Command-line programs
---------------------

  * `app` launches a Mac application.
  * `hello` is not needed by AMS, nor vice versa.  It's just a hand-coded 68K Hello World program, useful for testing that `xv68k` works.

[AMS]:  <https://www.v68k.org/advanced-mac-substitute/>
