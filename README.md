# HW-03
In this homework, we will see how our vm interacts with different IP confiigurations using Bridge mode

VM: Ubuntu Server

## Hostname
![hostname](images/hostname.png)
---

## Scenario 1
Bridge + DHCP

1. Ip 
![Bridge + DHCP](images/bridge-DHCP.png)

2. ping to google.com
![ping-google](images/DHCP-ping.png)


---

## Scenario 2
Bridge + Manual IP, same subnet

1. IP
![Bridge + Manual IP, same subnet](images/bridge-same.png)


The virtual machine was configured with the IP address 10.10.10.10, which is outside the host network. Because of this, the VM cannot communicate with the router or access the Internet, so the ping to Google fails.
2. ping to google.com
![ping-google](images/same-subnet-ping.png)


---

## Scenario 3
Bridge + IP manual fuera de la subred
1. IP
![Bridge + Manual IP](images/bridge-out.png)

2. ping to google.com
![ping-google](images/out-ping.png)
---

## Hipervisor
![ip-mac](images/mac.png)
