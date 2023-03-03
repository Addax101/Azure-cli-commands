## Stop an existing virtual machine in Azure using the CLI
To stop an existing virtual machine in Azure using the CLI, follow these steps:

1.  Open a command prompt or terminal window and run the following command to stop the virtual machine: 
```
az vm stop --resource-group myResourceGroup --name myVM
```

* Replace `myResourceGroup` with the name of the resource group where your virtual machine is located, and `myVM` with the name of the virtual machine you want to stop.

2. Wait for the virtual machine to stop. You can use the following command to check the status of the virtual machine:
```
az vm show --resource-group myResourceGroup --name myVM --show-details --query powerState
```


This command should return the power state of the virtual machine (e.g. "VM stopped").

> Congratulations! You have now stopped an existing virtual machine in Azure using the CLI.
