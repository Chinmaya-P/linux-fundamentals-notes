## What I learned  
 Various network commands to determine the following:
 - IP address of the local machine and its network interfaces.
 - MAC Address of the local machine
 - Configuration and info about wireless network interfaces e.g. signal strength, frequency etc.
 - Neighbour Table (IP to MAC mapping table for devices connected in a local network )
 - ARP cache which shows MAC addresses mapped to IP addresses also
 - Routing Table, showing default gateway, network interfaces , and destination networks
 - Ping command used to test connectivity between devices in a local network using ICMP (Internet Control Message Protocol) packets
  
## Commands and Examples  
```bash
ip a
ip n
ip r
ifconfig
iwconfig
ip route show
arp -a
ping 192.168.0.1
```
  
## What Confused Me  
-  Why there are multiple commands which essentially do the exact same thing e.g. ip a and ifconfig, ip r and ip route show etc.
  
## Reflections  
-  Basic network commands are the beginning point to a greater understanding of networking and is important to be able to discover weak points in a network when it comes to pen-testing.
  
  
  