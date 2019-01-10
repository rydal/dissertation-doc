<h1> Tuxconfig - A Linux device configuration platform and application </h1>

Hello and welcome to my project, my dissertation at Kent university and my contribution for the Linux community.


This is both a platform for submitting device configurations and a client server system to install them on the host device.
Submissions are made to a central server, before being verified as not malicious. The client user can download and install the
device configurations and vote on their success. Unsuccessful configurations will be voted down by the system, whilst successful configurations are voted up by the system.

In cases where a more suitable driver is available the user has the option to install it.
A backup is made of the /etc/modules.* directory and /lib which can be restored in cases where an install breaks a machine.

It is a proof of concept and still needs some work, the following are it's limitations:
At the moment it only works on Ubuntu 18.04. Adding multiple device support is possible.
In order to prevent false votes on the success of a device I propose adding a database table of the device serial numbers of hardware
ensuring each device can only be voted on once, as well as cryptographically signing the information to the server using a public key.
It needs to launch when a new device is plugged in.

What I need for this to be successful:

In order to prevent malicious software and trojan horses being downloaded from the configuration repository I need a team to review
configurations as submitted to GitHub. 

I am more than happy to continue work on this project as well as manage git pull requests.
I have been using System() calls to bash to get things done quickly, obviously a final version will not use such methods.

Web page at:
https://linuxconf.feedthepenguin.org/hehe/index.jsp

The front end code, written in c++ using QT is referenced here:
https://git.cs.kent.ac.uk/rb602/tuxconfig-qt

The back end code, written in Java is here:
https://git.cs.kent.ac.uk/rb602/dissertation-code-server

This repository is of my dissertation, available here:
https://git.cs.kent.ac.uk/rb602/dissertation-doc/blob/master/dissertation.fodt

Feel free to email me at:
rb602@kent.ac.uk