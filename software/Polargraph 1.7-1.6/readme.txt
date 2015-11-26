*  Polargraph Software
*
*  Written by Sandy Noble
*  Released under GNU License version 3.
*  http://www.polargraph.co.uk
*  http://code.google.com/p/polargraph/

30th April 2013.  Beltane.

This is the source code for the Polargraph software. 
It contains:

Controller v1.5

Binary (compiled) versions of the controller for

- 32 bit linux
- 64 bit linux
- Mac OSX
- 32 bit Windows
- 64 bit Windows

Along with source code for the controller in the processing-source 
folder.

It also includes the required Processing libraries (geomerative, Controlp5, 
Diewald CV kit) that the controller uses.  These are not necessarily
the most recent versions, but they are the versions that work.

Processing Libraries should be copied into the libraries subfolder in 
your Processing sketchbook folder.

This is written and compiled under Processing v1.5.  It has not been 
tested with the v2 beta.

This unfortunately requires the infernal Quicktime, and on windows at least, WinVDIG.
I used WinVDIG from http://www.eden.net.nz/7/20071008/.  This is to use
Processing's built-in video capture libraries.

Server v1.62 for MEGA and UNO based machines

The arduino-source folder has the code for the firmware that should 
be uploaded to your arduino.  There are currently three versions:

- polargraph_server_a1 for Arduino UNO based machines with an 
  Adafruit motor shield.  PLEASE NOTE THIS VERSION DOESN'T SEEM TO FIT
  ON A DUEMILANOVE ANY MORE.  The previous version (1.2x) still does.)

- polargraph_server_mega for ATMEGA1280 or 2560 based arduinos 
  (Arduino MEGA) with Adafruit motor shield.

- polargraph_server_polarshield for Arduino MEGA 2560 running with 
  an attached Polarshield, serial stepper drivers and LCD touchscreen.

Each version is in it's own folder along with a precompiled .hex that
can be loaded directly using something like XLoader (some info about this
http://www.polargraph.co.uk/2012/07/more-updating-firmware-without-using-arduino/)

In the arduino-source folder there is also a libraries folder that
has all the arduino libraries that you will need to compile the 
firmware.

- AccelStepper
- AFMotor (for those using the Adafruit motor shield)
- UTFT (for the polarshield)
- UTouch (for the polarshield)

UTouch sometimes benefits from calibration, so if you find your 
touchscreen is not responding properly to your touch, you might 
need to do that.  The calibration figures that are in there already 
are ok for my ITDB02-2.2 screens.  Mostly.

The arduino libraries should be copied into your arduino sketch folder.