# Obico-Debian
Obico Server set up Using Debian as base

<pre>
Add user to sudoers file:
https://www.tecmint.com/fix-user-is-not-in-the-sudoers-file-the-incident-will-be-reported-ubuntu/

sudo nano /etc/sudoers
<user> all:all all

sudo nano /etc/apt/sources.list
add contrib non-free on all main

exit and save text editor

get wifi hardware details 
lspci -nn | grep Network
apt-get update && apt-get install firmware-iwlwifi

reboot

check if wifi driver is install shoud start with wlp
ip a

Install Docker
https://docs.docker.com/engine/install/debian/#set-up-the-repository
Install Docker-Desktop
https://docs.docker.com/desktop/install/debian/
Post Install Script

==install Obico
https://github.com/TheSpaghettiDetective/obico-server


---------- DONE ------------------


OPTIONAL: VNC Install for GUI Checking


Install Xterm
sudo apt-get install xterm

Install VNC server for remote GUI access 
https://computingforgeeks.com/install-and-configure-tigervnc-vnc-server-on-debian/

Error on starting VNCservice "cleanly exited too early (< 3 seconds)!"
https://askubuntu.com/questions/1375111/vncserver-exited-too-early

</pre>
