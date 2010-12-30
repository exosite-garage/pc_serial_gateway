========================================
About
========================================
pc_serial_gateway.py is a python script that collects data from devices
connected to a serial port and publishes the data to Exosite via XMPP

License is BSD, Copyright 2010, Exosite LLC

Built/tested with Python 2.6.5

========================================
Quick Start
========================================
****************************************
1) install python
****************************************
http://www.python.org/download/
http://www.python.org/download/releases/2.6.5/
http://www.python.org/ftp/python/2.6.5/python-2.6.5.msi

****************************************
2) install xmpppy
****************************************
http://xmpppy.sourceforge.net/
http://sourceforge.net/projects/xmpppy/
http://sourceforge.net/projects/xmpppy/files/xmpppy/0.4.0/xmpppy-0.4.0.win32.exe/download

If running Debian Linux (or Ubuntu), you can > apt-get install python-xmpp

****************************************
3) install dnspython
****************************************
http://www.dnspython.org/

If running Debian Linux (or Ubuntu), you can > apt-get install python-dns
NOTE: this step is not always necessary, depends on xmpp server you use

****************************************
4) install serial
****************************************
http://pyserial.sourceforge.net/
http://pypi.python.org/pypi/pyserial

If running Debian Linux (or Ubuntu), you can > apt-get install python-serial

****************************************
5) configure it
****************************************
Open the file "options.cfg"
--) update the serial port # in options.cfg to point to the port you are
	using (use device manager in windows or a terminal program to list ports)
--) update the default credentials in options.cfg to use your xmpp login
--) add device name and CIK pairing to options.cfg (get CIK from Exosite
	Portals device page -> add new device, device_name should match 
	whatever is sent by the device hooked to the serial port)

****************************************
6) test it out
****************************************
get python script "exompp_serialgw.py" and "options.cfg"
--) attach a compatible device to a/the serial port
--) run the script (> python exompp_serialgw.py)
--) verify the app connects to both the device and Exosite (no errors 
    should be generated)
--) log into one.exosite.com and verify the data source is created and 
	that data was generated

****************************************
7) tweak it
****************************************
--) play around, use it, extend it!
