
## Create a new virtual machine in Azure using the CLI
To create a new virtual machine in Azure using the CLI, follow these steps:

* Open a command prompt or terminal window and run the following command to create a new resource group:
`az group create --name myResourceGroup --location eastus`

Replace myResourceGroup with the name of the resource group you want to create, and eastus with the location where you want to create the resource group.

* Run the following command to create a new virtual machine:

`az vm create \
--resource-group myResourceGroup \
--name myVM \
--image UbuntuLTS \
--admin-username azureuser \
--generate-ssh-keys`

Replace `myResourceGroup` with the name of the resource group you created in step 1, `myVM` with the name you want to give your virtual machine, and `UbuntuLTS` with the name of the operating system image you want to use. You can also replace `azureuser` with the username you want to use to connect to the virtual machine, and remove the `--generate-ssh-keys` parameter if you want to use your own SSH keys.

* Wait for the virtual machine to be created. You can use the following command to check the status of the virtual machine:
`az vm show --resource-group myResourceGroup --name myVM --show-details --query powerState`

This command should return the power state of the virtual machine (e.g. "VM running").

Congratulations! You have now created a new virtual machine in Azure using the CLI.
