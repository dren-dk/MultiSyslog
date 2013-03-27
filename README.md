MultiSyslog
===========

Zero configuration remote syslog server

Copyright 2005-2013 Flemming Frandsen.
You may use this software under the terms of the BSD license.
See: https://github.com/dren-dk/MultiSyslog

This is a very small and simple script that will listen on port 514 and act as a remote syslog server,
but unlike existing syslog servers it will automatically let everybody log to it and store the log from
each remote host as a separate file.

By default the log files are created in /var/log/remote and IP addresses in the localhost, 10.0.0.0/8 and 192.168.0.0/16
ranges are allowed to log.

Edit the constants at the top of the script to configure it.

The script is made to be linked into /etc/rc3.d like all other sysv init style scripts, so you can start and stop it with:

sudo ./multi-syslog start
sudo ./multi-syslog stop


