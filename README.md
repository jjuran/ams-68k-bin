ams-68k-bin
===========

AMS is the [Advanced Mac Substitute][AMS], a trap-level emulator for Mac OS.

This repository contains various 68K executables needed to run Mac apps using AMS.

Applications
------------

  * **Welcome** is a parody of the "Welcome to Macintosh" loading screen.
  * **Tic-tac-toe** is a Tic-tac-toe board with multiple Undo and saved games.
  * **Nyanochrome Cat** is a black and white adaptation of Christopher Torres' Nyan Cat animation.
  * **IAGO** is a Reversi game released to the public domain by David Reed in 1984.

Modules
-------

  * `ams-core` provides most of the OS:
    * low-level cursor support
    * interrupt handlers
    * Vertical Retrace Manager
    * OS Utilities
    * Memory Manager
    * Gestalt Manager
    * OS Event Manager
    * Toolbox Event Manager
  * `ams-io` implements the Device Manager and several device drivers:
    * Serial Driver
    * Sound Driver
  * `ams-fs` implements the File Manager and supported filesystems:
    * MFS
    * MacBinary and MacBinary+
    * Host bridge for read-only startup and writable Documents volumes
  * `ams-rsrc` implements the Resource Manager.
  * `ams-pack` contains the Package Manager (but no actual packages).
  * `ams-seg` contains the Segment Loader.
  * `ams-qd` provides QuickDraw, the Font Manager, and routines for fixed-point math and bit manipulation.
  * `ams-ui` includes various facilities to support a user interface:
    * Window Manager (including the standard documents and dialogs WDEF)
    * Control Manager (including the standard buttons CDEF)
    * Menu Manager (including the standard MDEF)
    * Dialog Manager
    * Scrap Manager
    * Icon Manager
    * List Manager
    * Standard File Package
    * International Utilities Package
    * Binary/Decimal Conversion Package
    * String Utilities

Command-line programs
---------------------

  * `app` launches a Mac application.
  * `hello` is not needed by AMS, nor vice versa.  It's just a hand-coded 68K Hello World program, useful for testing that `xv68k` works.

[AMS]:  <https://www.v68k.org/advanced-mac-substitute/>
