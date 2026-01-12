# sdvd-nas

### Specifications
> Model
> - Lenovo Tiny M700

> Operating System
> - TrueNAS Community 25.10.1

> CPU - Intel i5-6500T
> - 4 Cores
> -  4 Threads
> - 2.5 GHz Base Frequency

> Memory
> - 16GB (2x8GB SODDR4)

> Storage
> - 500GB NVME (OS and Extras)
> - 1TB SATA SSD (Network Storage)

### Overview
sdvd-nas serves as a storage solution for my mini homelab. The most common use I have for it is to contain my ISOs and Container Templates for my proxmox cluster. I have given each of the nodes in the cluster access to the SMB share. From what I've read online, it seems like ZFS share would be the prefered choice normally, but I'm not planning on using the NAS for VM storage, so I decided to stick with an SMB share.

At the moment, I have a 1TB SATA SSD as my main storage pool. This should be more than enough starting out, but I know won't last for all of my plans for my homelab. Because of this, my plan is to upgrade as I go. 

### Pictures

![info page](/Resources/sdvd-nas%20info.png)
![storage page](/Resources/sdvd-nas%20storage.png)

### Applications
- FileBrowser : This allows me to have a web hosted file browser into my NAS storage. I have a cloudflare tunnel hosted on my Raspberry Pi and use this to host the webpage.
- HomeAssistant : HomeAssistant is a smarthome open source software that allows for control of many different smart and IoT devices through a webpage.

### Virtual Machine
> sdvd-nasvm
> - 4 Virtual CPUs
> - 8 GB RAM
> - 64 GB Storage
> - Ubuntu Server

This virtual machine runs a handful of more essential services in docker containers. These services are as follows.
> - Pihole : DNS based adblocking service. 