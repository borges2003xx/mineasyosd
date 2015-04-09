# How to load the char file #


As the config tool uses 57k6 baud for char file upload you need to load a firmware which also uses 57k6 baud.

The firmware baud rate depends on the GPS version you like to use.

You can set the GPS baud rate in the OSD\_Config.h file with the following define:

#define GPS\_BAUD\_RATE			9600

So, prior to char set upload, build and upload a firmware for 57k6 baud configuring the define as in the following:

#define GPS\_BAUD\_RATE			57600

After that firmware upload, do the char file upload.

How to upload the char file is explained here: http://code.google.com/p/arducam-osd/wiki/Cfg_Update_CharSet

Get the special minEASYOSD MCM file from my code section trunk/configs

After char file upload, choose the GPS baud rate you like:

#define GPS\_BAUD\_RATE			whateveryourgpsneeds

and build and upload this firmware.