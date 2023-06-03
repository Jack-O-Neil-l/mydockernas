# My docker / NAS Server (see below for prerequisites)
![alt text](https://github.com/Jack-O-Neil-l/mydockernas/blob/main/images/MyNasLogo.png?raw=true)

Prerequisites:
Install docker and docker compose

Optionnal:
Create a MacVlan (if you want to use AddGuard home as DNS server for your router or others devices)

```bash
docker network create -d macvlan \
    --subnet=192.168.1.0/24 \
    --gateway=192.168.1.1  \
    -o parent=enp0s3 \
     myvlan```
