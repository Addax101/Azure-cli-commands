To delete a network security group (NSG) using the CLI, follow these steps:

1. Open a command prompt or terminal window and run the following command to delete the NSG:
```
az network nsg delete --resource-group myresourcegroup --name mynsg
```
* Replace `myresourcegroup` with the name of the resource group your NSG is in, and `mynsg` with the name of your NSG.

2. Confirm that you want to delete the NSG by entering `y` when prompted.
> Congratulations! You have now deleted your NSG using the CLI.
