# SOC Home Lab

This SOC Home Lab is intended to provide a workspace for me to simulate and experiment with security solutions before deploying them in production environments. 

This lab will consist of five virtual machines running on VirtualBox and each will provide a specific task. <br>
- pfSense Router (192.168.1.1): Serves as the network gateway, routing traffic from the WAN port into VirtualBox’s internal network. It runs a firewall and IDS/IPS powered by Snort, supports VPN management, and can create a DMZ to isolate and protect internal systems.
- Ubuntu Server (192.168.1.25): Runs Wazuh SIEM/XDR for centralized security operations management, serving as the primary system overseeing the Security Operations Center (SoC)
- Fedora Server (192.168.1.42): A honeypot server emulating multiple services to attract potential threats, with all captured traffic forwarded to the Wazuh server for analysis.
- Windows 11 Machine (192.168.1.11): Simulates an endpoint device, runs malware detection tools, and forwards security events to the SIEM for analysis.
- Kali Linux Machine (192.168.1.8): Adversary simulation system used to execute attack campaigns and evaluate detection capabilities.
  
Software used in this lab: <br><br>
<a href="https://www.kali.org/"><img src="https://img.shields.io/badge/Kali_Linux-557C94?logo=linux&logoColor=white&style=for-the-badge" /></a>
<a href="https://www.virtualbox.org/"><img src="https://img.shields.io/badge/VirtualBox-blue?logo=virtualbox&logoColor=white" /></a> 
<a href="https://ubuntu.com/"><img src="https://img.shields.io/badge/Ubuntu-E95420?logo=ubuntu&logoColor=white" /></a>
<a href="https://www.microsoft.com/en-us/software-download/windows11"><img src="https://img.shields.io/badge/Windows%2011-0078D6?logo=windows&logoColor=white" /></a>
<a href="https://fedoraproject.org/"><img src="https://img.shields.io/badge/Fedora-294172?logo=fedora&logoColor=white" /></a>
<a href="https://www.pfsense.org/"><img src="https://img.shields.io/badge/pfSense-394B5A?logo=pfsense&logoColor=white" /></a>
