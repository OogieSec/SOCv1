# SOC Home Lab

This SOC Home Lab is intended to provide a workspace for me to simulate and experiment with security solutions before deploying them in production environments. 

This lab will consist of five virtual machines running on VirtualBox and each will provide a specific task. 

- pfSense Router (192.168.1.1): Acts as the network gateway, routing traffic from WAN port and into your virtualbox's Internal network. Runs firewall and IDS/IPS via Snort, can manage VPNs, and create DMZ to segregate the internal network
- Ubuntu Server (192.168.1.25): Running Wazuh SIEM/XDR for security operations management, the main machine managing the SoC
- Fedora Server (192.168.1.42): Honeypot server faking various services and forwarding traffic to the Wazuh server
- Windows 11 Machine (192.168.1.11): Simulates a user device, runs malware detection, and forwards events to the SIEM
- Kali Linux Machine (192.168.1.8): Adversary simulation device for running attack campaigns and testing detection capabilities

Software used in lab: <br>
<a href="https://www.virtualbox.org/"><img src="https://img.shields.io/badge/VirtualBox-blue?logo=virtualbox&logoColor=white" /></a>  <br>
<a href="https://www.pfsense.org/"><img src="https://img.shields.io/badge/pfSense-394B5A?logo=pfsense&logoColor=white" /></a><br>
<a href="https://ubuntu.com/"><img src="https://img.shields.io/badge/Ubuntu-E95420?logo=ubuntu&logoColor=white" /></a><br>
<a href="https://www.microsoft.com/en-us/software-download/windows11"><img src="https://img.shields.io/badge/Windows%2011-0078D6?logo=windows&logoColor=white" /></a><br>
<a href="https://fedoraproject.org/"><img src="https://img.shields.io/badge/Fedora-294172?logo=fedora&logoColor=white" /></a><br>
<a href="https://www.kali.org/"><img src="https://img.shields.io/badge/Kali_Linux-557C94?logo=linux&logoColor=white&style=for-the-badge" /></a><br>
