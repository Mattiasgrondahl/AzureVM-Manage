# AzureVM-Manage

About:

This is a bash script that lets you run a couple of commands to login, start, stop and connect to an Azure VM
The background to all of this is to be able to keep the costs down by keeping the machine turned of when not used.

Prereq
1. You need to have Azure CLI 2.0 installed.
curl -L https://aka.ms/InstallAzureCli | bash
https://docs.microsoft.com/sv-se/cli/azure/install-azure-cli 

2. Edit the Script to match your subscription Id and your VM name
You can get the subscription id by running az account once logged in.

3. For the RDP connection to work you will need to have xfreerdp installed.
apt-get install freerdp-x11

