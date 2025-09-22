# Configuration for Windows Machine
-	Setting up the Wazuh Agent<br>
-  Attacking Mysql Service
# Setting up the Wazuh Agent
- After successful installation and initial update, head over to https://UBUNTU_IP to access the Wazuh Dashboard
- Open the left side bar, expand the Agents management view

- Go to Summary > Deploy New Agent

-Follow the on screen insturctions! they're sufficient alone to get this done

1. Select the package to download and install on your system
2. Server address
3. Optional settings
4. Run the following commands to download and install the agent
5. Start the agent

Step 1: Enable SMB

1. Enable Network Discovery and File Sharing
2. Open Settings → Win + I
3. Go to:
- Network & Internet → Advanced network settings → Advanced sharing settings
4. Under Private network, turn ON:
-  Network discovery
-  File and printer sharing
5. Under All networks, scroll down and:

6. Set Password protected sharing → Off (optional, makes access easier for testing)

7. Allow public folder sharing → On

💡 Tip: If you don’t see "Private network," make sure your network profile is set to Private:

- Go to Settings → Network & Internet → Wi-Fi / Ethernet → select your connection → set Network profile to Private.
