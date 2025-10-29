# 🌐 Next Gen pfSense Router

>   This setup establishes a functional pfSense firewall with Snort intrusion detection/prevention capabilities for monitoring and securing network traffic.

# 💡Summary Report: pfSense Setup and Snort IDS/IPS Setup<br>
🧱 pfSense Virtual Machine Setup (Virtual Box)<br>
Virtual Machine Creation:<br>
•	Created a new VM in Virtual Box named pfSense.<br>
•	Selected Type: BSD, Version: FreeBSD (64-bit).<br>
•	Allocated 512MB RAM and created a 16 GB dynamically allocated VDI virtual hard disk.<br>
Network Adapter Configuration:<br>
•	Adapter 1 (WAN): Enabled and attached to a Bridged Adapter using the host’s active network interface.<br>
•	Adapter 2 (LAN): Enabled and attached to an Internal Network (e.g., named "LAN").<br>
Mounting pfSense ISO and Installation:<br>
•	Mounted the pfSense installer ISO under VM storage settings.<br>
•	Launched the VM and installed pfSense, accepting default options.<br>
•	Network interfaces were assigned as:<br>
o	WAN (em0): Bridged Adapter<br>
o	LAN (em1): Internal Network<br>
Web Interface Configuration:<br>
•	Accessed the pfSense web GUI via a browser from another VM connected to the internal network.<br>
•	Default login used: --- / ----.<br>
•	Completed the initial configuration using the setup wizard.<br>
________________________________________
🔍Snort IDS/IPS Installation and Configuration<br>
Snort Installation:<br>
•	Accessed the pfSense web interface and navigated to System > Package Manager.<br>
•	Searched for and installed the Snort package.<br>
Snort Global Configuration:<br>
•	Navigated to Services > Snort and configured global settings:<br>
o	Enabled Snort on the WAN interface.<br>
o	Chose operating mode: IDS or IPS.<br>
Rule Updates:<br>
•	Downloaded the latest Snort rules via the Updates tab.<br>
•	Registered a Snort account if needed for rule access.<br>
Rule Set Configuration:<br>
•	Enabled selected rule categories (e.g., Emerging Threats, Snort GPLv2 Community Rules) under the Categories tab.<br>
Interface Setup:<br>
•	Configured Snort on the WAN interface:<br>
o	Enabled desired rule sets.<br>
o	Adjusted additional interface-specific settings as needed.<br>
Service Activation and Monitoring:<br>
•	Started the Snort service on the WAN interface.<br>
•	Monitored alerts via the Alerts tab to detect and analyze potential threats.<br>
