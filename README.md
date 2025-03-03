# Hack-a-Home-Trojan-Horse-Project
CyberSecurity project penetration testing a virtual homenetwork that I built
Hack-a-Home: Trojan Horse
Hakeem, Brandon

Project Overview:
The objective of this project was to simulate a home network using EVE-NG, and then perform the penetration test to attempt to identify the vulnerabilities in the network, emphasizing firmware. This report will include the details of network configuration, the method used for penetration testing, the results of the penetration testing, and the part played by firewalls even in the home networks of individuals who are not very tech-savvy.

1. Network Architecture:

1. 1 EVE-NG Lab Configuration:
The virtual lab was built using the following network components: The virtual lab was built using the following network components:

AlienVault Cybersecurity: Used on a large scale as a Security Information and Event Management system for detecting and mitigating network threats.
Cisco CSR 1000V (XE 16. x): A Cisco 9300 hw-based virtual router utilizing Cisco IOS XE software for emulating enterprise routing and security.
Juniper vEVO Router: A copy of Juniper’s routing platform operating in a virtual environment with enhanced networking capabilities and security.
OPNsense: A free-firewall software meant for routing in ensuring that the edges of the networks are secured.
VyOS: A network operating system that integrates the aspects of commercial routing, firewalls, as well as VPNs.

1. 2 Network Setup:
The virtual network consisted of a typical home network with extra levels of difficulty, such as multiple subnets, firewalls, and routers for different devices and areas. The intention was to provide conditions as close to the real world and the use of various devices as possible and to be able to check out potential weaknesses.

2. Penetration Testing Methodology:

2. 1 Tools and Techniques:

Nmap: Its utility was applied to network mapping and recognizing of available ports, services, and possible weaknesses inside the network.
PuTTY: For running the SSH connections and for the management of switches and routers in the network.
VirtualBox and QEMU: Used to provision and control virtual machines in the context of the EVE-NG platform.

2. 2 Commands Used:

Initial Network Scan: sudo nmap –scan business law for dummies -host-depth high horizontal 192. 168. 1. 0/24
Focused Scans on Identified Hosts: Focused Scans on Identified Hosts:
nmap -sS -O -p 1-65535 192. 168. 1. 191
smbclient -L \\\\192. 168. 1. 191
vncviewer 192.168.1.191:5900

3. Findings and Analysis:

3. 1 Vulnerabilities Discovered:

Open VNC Ports: Present on one of the network devices; this is dangerous as it might allow remote access.
SMB Services: SMB was operational at some of the devices without passing through the authentication process thus making the devices reachable.
Outdated Firmware: The virtual devices had exposed firmware in some of the virtual devices which if not updated were vulnerable to being exploited.

3. 2 Importance of Firmware Updates
Firmware updates are extremely important as far as the security of the network devices is concerned. What emerged from the testing was that firmware could and was a big weakness to attackers, as they can take advantage of outdated firmware which has holes that have been fixed in subsequent firmware. Regular updates of firmware are important even for home networks since threats to a network can change over time.

4. Importance of Firewalls:

4. 1 Firewall Configurations:
The deployment of OPNsense and VyOS firewalls was instrumental in protecting the network. These firewalls were configured to:
Filter traffic between different network zones.
Block unauthorized access to sensitive services.
Log and monitor suspicious activity.


4. 2 Firewall Effectiveness:
Network firewalls considerably diminished the havoc that was possible with the networking. At times, there were attempts at penetration into the network however, these were futile in the face of firewalls which successfully denied the intruders access and offered log data that could be used in investigations.

5. Conclusion:
From this project, people learned the need to make sure their networks are well secured, even if they are at home. Working in the EVE-NG laboratory proved to be valuable and allowed researching multiple aspects of network security – effects of firmware updates and others, the importance of firewalls, etc. The study proved that vulnerabilities as such can be exploited when the usual aspects of protection, like the update of firmware, and configuration of a firewall are not dealt with accordingly.

In the case where there are fewer computer/network-literate users, they must at the bare minimum correctly configure the firewalls and have up-to-date firmware on their network device for the best security available to them.

6. Recommendations:

Regular Firmware Updates: Make sure that firmware on all devices connected to the network is updated to the current state to minimize threats known to be present.
Firewall Implementation: Use available firewalls to mediate traffic and protect areas of your network.
Continuous Monitoring: The following are some recommendations: Using programs like Alien Vault for constant surveillance so that any visible clear threats can be dealt with immediately.











