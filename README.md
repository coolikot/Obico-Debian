# Obico-Debian
Obico Server set up Using Debian as base

<pre>
Add user to sudoers file:
https://www.tecmint.com/fix-user-is-not-in-the-sudoers-file-the-incident-will-be-reported-ubuntu/

sudo nano /etc/sudoers
<user>        ALL=(ALL:ALL) ALL
</pre>
![image](https://github.com/coolikot/Obico-Debian/assets/85612975/8ea26f20-8b3d-49ba-a4f0-75590bfd2234)
<pre>
save and exit text editor (using ctrl+x)

sudo nano /etc/apt/sources.list
add contrib non-free on all main
</pre>
![image](https://github.com/coolikot/Obico-Debian/assets/85612975/84a68230-aee6-4d46-9c69-7a177c0550dc)
<pre>
save and exit text editor (using ctrl+x)

get wifi hardware details 
lspci -nn | grep Network
</pre>
![image](https://github.com/coolikot/Obico-Debian/assets/85612975/ee3d1470-5c53-45d5-8960-9e8891f84b4d)
<pre>
apt-get update && apt-get install firmware-iwlwifi

reboot

check if wifi driver is install shoud start with wlp
ip a
</pre>
![image](https://github.com/coolikot/Obico-Debian/assets/85612975/beb1b882-b2ca-4fc0-be0b-dc0ba087a557)
<pre>

Install Docker
https://docs.docker.com/engine/install/debian/#set-up-the-repository
Install Docker-Desktop
</pre>
![image](https://github.com/coolikot/Obico-Debian/assets/85612975/0c49823d-84e2-402d-b4a5-cc0b00a2aee0)
<pre>
https://docs.docker.com/desktop/install/debian/
Post Install Script

==install Obico
https://github.com/TheSpaghettiDetective/obico-server
</pre>
![image](https://github.com/coolikot/Obico-Debian/assets/85612975/475ed7f1-8b1b-4cda-b42f-53372274c461)
<pre>

---------- DONE ------------------


OPTIONAL: VNC Install for GUI Checking


Install Xterm
sudo apt-get install xterm

Install VNC server for remote GUI access 
https://computingforgeeks.com/install-and-configure-tigervnc-vnc-server-on-debian/

Error on starting VNCservice "cleanly exited too early (< 3 seconds)!"
https://askubuntu.com/questions/1375111/vncserver-exited-too-early

</pre>
