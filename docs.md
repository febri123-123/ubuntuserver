# Dokumentasi Konfigurasi Network Ubuntu 24.04

Dokumentasi ini berisi langkah-langkah merubah dan menambah konfigurasi 
network 
menggunakan Netplan.

### 1. Masuk sebagai Root
```bash

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

### 2.lalu verifikasi 
'''bash

ifconfig
 
atau

ip a
