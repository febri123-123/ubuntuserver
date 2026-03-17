sudo su

cd /etc/netplan/nano 00-installer-config.yaml
------------------------------------------------
This is the network config written by 'subiquity'
network:
  ethernets:
    enp0s3:
      dhcp4: true
  version: 2
  ethernets:
    enp0s8:
      dhcp4: true
  version: 2
-------------------------------------------------
sudo netplan apply

ifconfig
 
