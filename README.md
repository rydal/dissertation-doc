<h1> Tuxconfig - A Linux device configuration platform and application </h1>

Hello and welcome to my project, my dissertation at Kent university and my contribution for the Linux community.

Despite it’s small memory footprint and install size, Linux is way behind
windows when it comes to choices of operating systems, rarely bundled with a
computer bought from a major supplier. One reason for this is the problem of
configuring devices using a terminal console, forcing the user to enter obscure
configuration commands to install the drivers to make a device work. Ubuntu,
a major Linux distribution, has this covered in it’s restricted driver application,
but the devices listed here are few and far between compared to the vast array
of devices available on the market.
Can there be, programmatically, a more effective means of installing obscure
hardware, removing the need to type in commands to configure a device in
place of a graphical tool to do so?
This paper presents tuxconfig, a client application and server back-end to do
just that.
This is not only an application to install a significant array third party drivers. It
is a platform from which knowledgeable Linux users can submit code to a
centralised database for standard users to download, compile and install
hardware drivers.
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
https://linuxconf.feedthepenguin.org/hehe/

The front end code, written in c++ using QT is referenced here:
https://github.com/rydal/tuxconfig-frontend 
The back end code, written in Java is here:
https://github.com/rydal/tuxconfig-backend
This repository is of my dissertation, available here:
https://github.com/rydal/dissertation-doc/dissertation.fodt

Feel free to email me at:
rb602@kent.ac.uk
