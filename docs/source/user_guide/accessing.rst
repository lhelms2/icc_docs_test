.. _access:

Accessing the System
=====================

Connecting
------------

The Campus Cluster can be accessed via Secure Shell (SSH) to the head nodes using your official University NetID login and password.
Generally Unix/Linux based systems have a ssh client by default, however desktops/laptops running versions of Windows prior to Windows 10 version 1803 do not. 
There is third party software available for Windows users to access the Campus Cluster. 
Please see this non-exhaustive list of `ssh clients <#ssh>`__ that can be used to access the Campus Cluster.

Below is a list of hostnames that provide round-robin access to head
nodes of the Campus Cluster instances as indicated:

+-----------------------+-----------------------+-----------------------+
| Access Method         | Hostname              | Head Node             |
+-----------------------+-----------------------+-----------------------+
| SSH                   | cc-login.campu        | namehN                |
|                       | scluster.illinois.edu | (ex.                  |
|                       |                       | cc-login1,golubh1)    |
+-----------------------+-----------------------+-----------------------+

SSH
----

A variety of SSH based clients are available for accessing the Campus
Cluster from your local system. There are two types of SSH clients,
clients that support both remote login access and data transfers and
clients that support data transfers only.

+-----------------+-----------------+-----------------+-----------------+
| SSH Client      | Remote Login    | Data Transfer   | Installs On     |
+-----------------+-----------------+-----------------+-----------------+
| `MobaXterm <htt | Yes             | Yes             | Windows         |
| p://mobaxterm.m |                 |                 |                 |
| obatek.net/>`__ |                 |                 |                 |
| is an enhanced  |                 |                 |                 |
| terminal with   |                 |                 |                 |
| an X server and |                 |                 |                 |
| a set of Unix   |                 |                 |                 |
| commands        |                 |                 |                 |
| (GNU/Cygwin)    |                 |                 |                 |
| packaged in the |                 |                 |                 |
| application.    |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| `SSH Secure     | Yes             | Yes             | Windows         |
| Sh              |                 |                 |                 |
| ell <https://ww |                 |                 |                 |
| w.google.com/se |                 |                 |                 |
| arch?ei=GH8hYKS |                 |                 |                 |
| FCoi4tAb9z4qwBA |                 |                 |                 |
| &q=SSHSecureShe |                 |                 |                 |
| ll+3.2.9&oq>`__ |                 |                 |                 |
| allows you to   |                 |                 |                 |
| securely login  |                 |                 |                 |
| to remote host  |                 |                 |                 |
| computers, to   |                 |                 |                 |
| execute         |                 |                 |                 |
| commands safely |                 |                 |                 |
| on a remote     |                 |                 |                 |
| computer, and   |                 |                 |                 |
| to provide      |                 |                 |                 |
| secure          |                 |                 |                 |
| encrypted and   |                 |                 |                 |
| authenticated   |                 |                 |                 |
| communications  |                 |                 |                 |
| between two     |                 |                 |                 |
| hosts in an     |                 |                 |                 |
| untrusted       |                 |                 |                 |
| network.        |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| `Tu             | Yes             | Yes             | Windows         |
| nnelier <http:/ |                 |                 |                 |
| /www.bitvise.co |                 |                 |                 |
| m/tunnelier>`__ |                 |                 |                 |
| is a flexible   |                 |                 |                 |
| SSH client      |                 |                 |                 |
| which includes  |                 |                 |                 |
| terminal        |                 |                 |                 |
| emulation,      |                 |                 |                 |
| graphical as    |                 |                 |                 |
| well as         |                 |                 |                 |
| command-line    |                 |                 |                 |
| SFTP support,   |                 |                 |                 |
| an FTP-to-SFTP  |                 |                 |                 |
| bridge,         |                 |                 |                 |
| additional      |                 |                 |                 |
| tunneling       |                 |                 |                 |
| features        |                 |                 |                 |
| including       |                 |                 |                 |
| dynamic port    |                 |                 |                 |
| forwarding      |                 |                 |                 |
| through         |                 |                 |                 |
| integrated      |                 |                 |                 |
| proxy.          |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| `P              | Yes             | Yes             | Windows         |
| uTTY <http://ww |                 |                 | Linux           |
| w.chiark.greene |                 |                 | Mac OS          |
| nd.org.uk/~sgta |                 |                 |                 |
| tham/putty/>`__ |                 |                 |                 |
| is an open      |                 |                 |                 |
| source terminal |                 |                 |                 |
| emulator        |                 |                 |                 |
| application     |                 |                 |                 |
| which can act   |                 |                 |                 |
| as a client for |                 |                 |                 |
| the SSH,        |                 |                 |                 |
| Telnet, rlogin, |                 |                 |                 |
| and raw TCP     |                 |                 |                 |
| computing       |                 |                 |                 |
| protocols and   |                 |                 |                 |
| as a serial     |                 |                 |                 |
| console client. |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| `FileZill       | No              | Yes             | Windows         |
| a <http://filez |                 |                 | Linux           |
| illa-project.or |                 |                 | Mac OS          |
| g/index.php>`__ |                 |                 |                 |
| is a fast and   |                 |                 |                 |
| reliable        |                 |                 |                 |
| cross-platform  |                 |                 |                 |
| FTP, FTPS and   |                 |                 |                 |
| SFTP client     |                 |                 |                 |
| with lots of    |                 |                 |                 |
| useful features |                 |                 |                 |
| and an          |                 |                 |                 |
| intuitive       |                 |                 |                 |
| graphical user  |                 |                 |                 |
| interface.      |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| `WinSCP <http:  | No              | Yes             | Windows         |
| //winscp.net/en |                 |                 |                 |
| g/index.php>`__ |                 |                 |                 |
| is an open      |                 |                 |                 |
| source free     |                 |                 |                 |
| SFTP client,    |                 |                 |                 |
| SCP client,     |                 |                 |                 |
| FTPS client and |                 |                 |                 |
| FTP client for  |                 |                 |                 |
| Windows. Its    |                 |                 |                 |
| main function   |                 |                 |                 |
| is file         |                 |                 |                 |
| transfer        |                 |                 |                 |
| between a local |                 |                 |                 |
| and a remote    |                 |                 |                 |
| computer.       |                 |                 |                 |
| Beyond this,    |                 |                 |                 |
| WinSCP offers   |                 |                 |                 |
| scripting and   |                 |                 |                 |
| basic file      |                 |                 |                 |
| manager         |                 |                 |                 |
| functionality.  |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+

**Note:** See the Campus Cluster’s `Storage and Data guide <https://campuscluster.illinois.edu/resources/docs/storage-and-data-guide>`__ for information on transferring files/data to and from the Campus Cluster.

Network Details for Illinois Investors
-----------------------------------------

The Campus Cluster is interconnected with the University of Illinois networks via the *Campus Advanced Research Network Environment* (CARNE) and is addressed out of fully-accessible public IP space, located outside of the Illinois campus firewall. 
This positioning of the Campus Cluster outside the campus firewall enables access to regional and national research networks at high speeds and without restrictions. 
This does mean, however, that for some special use cases where it is necessary for Campus Cluster nodes to initiate communication with hosts on the Illinois campus network (e.g., you are hosting a special license server behind the firewall), you will need to coordinate with your department IT pro to ensure that your hosts are in the appropriate `Illinois campus firewall group <https://techservices.illinois.edu/services/firewall>`__ . 
Outbound communication from Illinois to the Campus Cluster should work without issue, as well as any communications from the Campus Cluster outbound to regional and national research networks.
