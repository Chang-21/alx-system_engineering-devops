# 0X13.FIREWALL
in this project i learned about firewalls from their function, types and their history


<img src="https://s3.amazonaws.com/intranet-projects-files/holbertonschool-sysadmin_devops/284/V1HjQ1Y.png"/>

## Firewalls
+ Network security system that monitors and controls incoming and outgoing network traffic based on predetermined rules
+ they establishe a barrier between a trusted network and an untrusted network e.g the internet

### Types of firewalls
There are two main firewalls
+ network-based system
+ host-based system

More information on [firewalls](https://en.wikipedia.org/wiki/Firewall_%28computing%29) 

### Tasks

[0. Block all incoming traffic but](0x13-firewall)
Let’s install the ufw firewall and setup a few rules on web-01.

Requirements:
+ The requirements below must be applied to web-01 (feel free to do it on lb-01 and web-02, but it won’t be checked)
+ Configure ufw so that it blocks all incoming traffic, except the following TCP ports
     - 22 (SSH)
     - 443 (HTTPS SSL)
     - 80 (HTTP)

+ Share the ufw commands that you used in your answer file

[1. Port forwarding](100-port_forwarding)
Firewalls can not only filter requests, they can also forward them.

Requirements:
+ Configure web-01 so that its firewall redirects port 8080/TCP to port 80/TCP.
+ Your answer file should be a copy of the ufw configuration file that you modified to make this happen
