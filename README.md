## SOC Home Lab
pfSense Router + Snort (IDS/IPS)<br>
Ubuntu - Sec Op Node (Wazuh SIEM)<br>
Windows 11 - User Device Sim (Sysmon + Wazuh Agent)<br>
Kali Linux - (Attack simulation & testing)<br>
Fedora - Honeypot (fakes ftp, http, etc) <br>
🚨🔧💻🖥️🔌🌐🛡️💡📦🤖🖥️🧱🔍🎯

HomeLab Setup with a Firewall, SIEM Solution, Exploitable machines and an Attacker.
The lab comprises five virtual machines running on VirtualBox, each configured to perform a distinct role within the security operations workflow. <br>
- <a href="https://www.pfsense.org/"><img src="https://img.shields.io/badge/pfSense-394B5A?logo=pfsense&logoColor=white" /></a> Router (**192.168.1.1**): Serves as the network gateway, routing traffic from the WAN port into VirtualBox’s internal network. It runs a firewall and IDS/IPS powered by Snort, supports VPN management, and can create a DMZ to isolate and protect internal systems.
- <a href="https://ubuntu.com/"><img src="https://img.shields.io/badge/Ubuntu-E95420?logo=ubuntu&logoColor=white" /></a> Server (**192.168.1.25**): Runs Wazuh SIEM/XDR for centralized security operations management, serving as the primary system overseeing the Security Operations Center (SoC)
- <a href="https://fedoraproject.org/"><img src="https://img.shields.io/badge/Fedora-294172?logo=fedora&logoColor=white" /></a> Server (**192.168.1.42**): A honeypot server emulating multiple services to attract potential threats, with all captured traffic forwarded to the Wazuh server for analysis.
- <a href="https://www.microsoft.com/en-us/software-download/windows11"><img src="https://img.shields.io/badge/Windows%2011-0078D6?logo=windows&logoColor=white" /></a> Machine (**192.168.1.11**): Simulates an endpoint device, runs malware detection tools, and forwards security events to the SIEM for analysis.
- <a href="https://www.kali.org/"><img src="https://img.shields.io/badge/Kali_Linux-557C94?logo=linux&logoColor=white&style=for-the-badge" /></a> Machine (**192.168.1.8**): Adversary simulation system used to execute attack campaigns and evaluate detection capabilities.

# Hardware:<br>
Processor	Intel i5<br>
Logical Processors 	4<br>
Memory	16 GB DDR4<br>
Storage Space	237 gb SSD
