Script to make nfsen start at boot.
Tested on CentOS 6.x, probably works on other linux systems.

Linked and referenced from https://www.forwardingplane.net/2014/01/install-nfsen-and-nfdump-on-centos-6-5-for-netflow-and-or-sflow-collection/
This script was lifted from this post http://sourceforge.net/p/nfsen/mailman/message/29434166/ and posted here for future use and change tracking. 

To make this work reference the above links for installation instructions or:

Move this file into /etc/init.d/ as the file nfsen

mv nfsen /etc/init.d/
cd /etc/init.d/
chmod 755 nfsen && chkconfig --add nfsen && chkconfig nfsen on

