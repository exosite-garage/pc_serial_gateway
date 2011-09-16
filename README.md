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
(1) install python<br>
http://www.python.org/download/<br>
http://www.python.org/download/releases/2.6.5/<br>
http://www.python.org/ftp/python/2.6.5/python-2.6.5.msi<br>

(2) install xmpppy<br>
http://xmpppy.sourceforge.net/<br>
http://sourceforge.net/projects/xmpppy/<br>
http://sourceforge.net/projects/xmpppy/files/xmpppy/0.4.0/xmpppy-0.4.0.win32.exe/download<br>

If running Debian Linux (or Ubuntu), you can > apt-get install python-xmpp

(3) install dnspython<br>
http://www.dnspython.org/<br>

If running Debian Linux (or Ubuntu), you can > apt-get install python-dns<br>
NOTE: this step is not always necessary, depends on xmpp server you use

(4) install serial<br>
http://pyserial.sourceforge.net/<br>
http://pypi.python.org/pypi/pyserial<br>

If running Debian Linux (or Ubuntu), you can > apt-get install python-serial

(5) install exompp<br>
https://github.com/exosite-labs/exompp-python<br>

This is a client library that supports the Exosite XMPP API

(6) configure it<br>
Open the file "options.cfg"<br>
--) update the serial port # in options.cfg to point to the port you are
using (use device manager in windows or a terminal program to list ports)<br>
--) update the default credentials in options.cfg to use your xmpp login<br>

(7) test it out<br>
get python script "pc_serial_gateway.py"<br>
--) attach a compatible device to a/the serial port<br>
--) run the script (> python pc_serial_gateway.py)<br>
--) verify the app connects to both the device and Exosite (no errors 
should be generated)<br>
--) log into portals.exosite.com and verify the data source is created and 
that data was generated<br>

(8) tweak it<br>
--) play around, use it, extend it!

========================================
Release History
========================================
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
