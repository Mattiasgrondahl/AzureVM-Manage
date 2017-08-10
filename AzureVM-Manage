#!/bin/bash
PS3='Please enter your choice: '
options=("Start" "Stop" "Login" "RDP" "About" "Quit")
select opt in "${options[@]}"
do
    case $opt in
        "Start")
            echo "Starting VM"
az vm start --resource-group win10 --name win10 --ids /subscriptions/1c2ef6d1-5bf9-4d6e-b2fa-xxxxxxxxxxx/resourceGroups/WIN10/providers/Microsoft.Compute/virtualMachines/win10
            ;;
        "Stop")
            echo "Stopping VM"
az vm stop --resource-group win10 --name win10 --ids /subscriptions/1c2ef6d1-5bf9-4d6e-b2fa-xxxxxxxxxxx/resourceGroups/WIN10/providers/Microsoft.Compute/virtualMachines/win10
            ;;
        "Login")
            echo "Login to Azure"
az login
            ;;
        "RDP")
            echo "Connect to RDP"
xfreerdp /u:username /v:xxx.northeurope.cloudapp.azure.com +clipboard +drives /size:90% /cert-tofu
            ;;
        "About")
            echo -e "About\n(1) You need to have Azure CLI 2.0 installed.\n(2) https://docs.microsoft.com/sv-se/cli/azure/install-azure-cli \n(3) Edit the Script $
            ;;
        "Quit")
            break
            ;;
        *) echo invalid option;;
    esac
done
