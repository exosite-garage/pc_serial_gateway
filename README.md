========================================
About
========================================
pc_serial_gateway.py is a python script that collects data from devices
connected to a serial port and publishes the data to Exosite via XMPP

License is BSD, Copyright 2011, Exosite LLC (see LICENSE file)

Built/tested with Python 2.6.5

========================================
Quick Start
========================================
(1) install python
http://www.python.org/download/
http://www.python.org/download/releases/2.6.5/
http://www.python.org/ftp/python/2.6.5/python-2.6.5.msi

(2) install xmpppy
http://xmpppy.sourceforge.net/
http://sourceforge.net/projects/xmpppy/
http://sourceforge.net/projects/xmpppy/files/xmpppy/0.4.0/xmpppy-0.4.0.win32.exe/download

If running Debian Linux (or Ubuntu), you can > apt-get install python-xmpp

(3) install dnspython
http://www.dnspython.org/

If running Debian Linux (or Ubuntu), you can > apt-get install python-dns
NOTE: this step is not always necessary, depends on xmpp server you use

(4) install serial
http://pyserial.sourceforge.net/
http://pypi.python.org/pypi/pyserial

If running Debian Linux (or Ubuntu), you can > apt-get install python-serial

(5) install exompp
https://github.com/exosite-labs/exompp-python

This is a client library that supports the Exosite XMPP API

(6) configure it
Open the file "options.cfg"
--) update the serial port # in options.cfg to point to the port you are
using (use device manager in windows or a terminal program to list ports)<br>
--) update the default credentials in options.cfg to use your xmpp login<br>

(7) test it out
get python script "pc_serial_gateway.py"
--) attach a compatible device to a/the serial port<br>
--) run the script (> python pc_serial_gateway.py)<br>
--) verify the app connects to both the device and Exosite (no errors 
should be generated)<br>
--) log into portals.exosite.com and verify the data source is created and 
that data was generated<br>

(8) tweak it
--) play around, use it, extend it!

========================================
Release History
========================================
----------------------------------------
2011-07-24
----------------------------------------
--) updated comments regarding alias creation<br>

----------------------------------------
2011-09-15
----------------------------------------
--) updated for synapse nodes cik vs. device name support v.2011-07-24<br>
--) updated support to pyexompp v.0.2<br>

----------------------------------------
2011-06-08
----------------------------------------
--) removed xmpp code to use pyexompp<br>

----------------------------------------
2011-01-07
----------------------------------------
--) initial release<br>

----------------------------------------
