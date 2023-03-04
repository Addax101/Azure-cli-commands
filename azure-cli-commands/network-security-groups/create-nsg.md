## create-nsg.md
To create a new network security group (NSG) using the CLI, follow these steps:

1. Open a command prompt or terminal window and run the following command to create a new NSG:
```
az network nsg create --resource-group myresourcegroup --name mynsg
```

* Replace `myresourcegroup` with the name of the resource group you want to create the NSG in, and `mynsg` with the name you want to give your new NSG.

2. Run the following command to add a rule to your new NSG: 
```
az network nsg rule create --resource-group myresourcegroup --nsg-name mynsg --name mynsg-rule --protocol Tcp --direction Inbound --source-address-prefix 0.0.0.0/0 --source-port-range "*" --destination-address-prefix "*" --destination-port-range 22 --access Allow --priority 1000
```
* Replace `myresourcegroup` with the name of the resource group your NSG is in, `mynsg` with the name of your NSG, `mynsg-rule` with the name you want to give your new rule, and customize the rule parameters as necessary.

> Congratulations! You have now created a new NSG and added a rule to it using the CLI.
