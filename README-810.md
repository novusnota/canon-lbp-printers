# Linux Canon CAPT drivers

Linux Canon CAPT driver
-----------------------

In this package there is a linux driver for Canon printer using CAPT 
protocol.

The general structure of the application is based on Rildo Pragana's 
driver for Samsung ML-85G, see : http://pragana.net - "Adventures in 
Linux Programming".

It should support both A4 and Letter sized paper, but I only tested it
with A4 sized paper.

Install
-------

Type:

# make

Then log in as root and type:

#make install

You need to have USB Printer support in your kernel. To install the
needed module, type, as root:
#modprobe usblp

And a new device should appear (/dev/usb/lp0). Type, as root:
#chmod a+rw /dev/usb/lp0

To give access to the printer to users (this is also needed for CUPS
to work.)

Install in CUPS
---------------

Follow the instructions presented on this page :
http://www.linuxprinting.org/cups-doc.html

When installing, do not select an USB port, but a dummy serial port
(for example Serial Port #8).

To align the margin, change TopSkip and LeftSkip parameters.
