# -Howto-setup-your-first-web-server
Use three simple scripts to install services (programs) needed to run a VPS, virtual or dedicated web server.

I do want to note this is intended to be geared towards Ubuntu or similar debian based Operating Systems with the intent of providing a framework for getting set up to host your own web sites. That is, whether dedicated or virtual, the user already has operating system space within a namespace and dns zone that will allow them to host their own web sites.


If you do not know what that means never fear. It is a very simple concept to understand. Web sites are generally hosted, or served to end users, clients, and you, by web servers. These are generally little more than computers or virtual containers used for storing and running web content.


In most cases the "layers" typically discussed in networking courses are not of a great concern. The "layers" most web site owners know and work with most often are usually, those services or programs used to access their content server side, present that data to a browsing end user, and any relational database management systems in between which store data within a separate file structure usually due to the types of data involved.



And so this is my attempt to share three abstractions of these layers through bash install scripts which setup the basics needed for an Apache based server stack with the end goal of self hosting web content, literally, or virtually..And we will do this by running in order, "./relation", "./internet", and "./apacheen".

As explained through a similar tutorial on lowendtalk dot com: "..Thought I would post some old shell scripts I used to use for setting up my own and client machines.


For this you will need to put the following commands in files relation, internet, and apacheen from your Shemoves line to the exit and run preferably after the following..(meaning, run below first to update your packages before install, unless you have recently updated your repos).



apt-get update

apt-get upgrade

apt-get install aptitude

aptitude update

aptitude safe-upgrade

reboot

aptitude install ntp ntpdate

.."



