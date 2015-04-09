# How to compile and flash the code #


How to compile and flash arduino code is documented many times on the web.

A good entry point for how to start with arduino and to compile the code is here: http://arduino.cc/en/Guide/HomePage

A good entry point for how to flash the code is here: http://code.google.com/p/arducam-osd/wiki/Cfg_Update_Firmware

But don't use their hex file of course, but compile the right one for minEASYOSD.

The code is here:

http://code.google.com/p/mineasyosd/source/checkout

You have to configure 3 things in the file OSD\_Config.h before compiling the code:

Choose the baud rate your GPS is using by changing the following line

#define GPS\_BAUD\_RATE			9600

Chose the correct format your GPS is using by commenting / uncommenting the following lines

UBX is default and tested already:

#define GPS\_PROTOCOL\_UBX

NMEA is currently untested:

//#define GPS\_PROTOCOL\_NMEA

Chose if you like the radar panel by commenting / uncommenting the following line

#define SHOW\_RADAR


And use the 'OSD Config Tool' from my code section trunk/Tools, it's the same as of my other project minOPOSD.