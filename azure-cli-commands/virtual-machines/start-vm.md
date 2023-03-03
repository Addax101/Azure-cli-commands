## Start an existing virtual machine in Azure using the CLI
To start an existing virtual machine in Azure using the CLI, follow these steps:

1.  Open a command prompt or terminal window and run the following command to start the virtual machine: `az vm start --resource-group myResourceGroup --name myVM`

* Replace `myResourceGroup` with the name of the resource group where your virtual machine is located, and `myVM` with the name of the virtual machine you want to start.

2. Wait for the virtual machine to start. You can use the following command to check the status of the virtual machine: `az vm show --resource-group myResourceGroup --name myVM --show-details --query powerState`

This command should return the power state of the virtual machine (e.g. "VM running").

> Congratulations! You have now started an existing virtual machine in Azure using the CLI 
