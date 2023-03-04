To create a new rule in a network security group (NSG) using the CLI, follow these steps:
1. Open a command prompt or terminal window and run the following command to create a new rule:
```
az network nsg rule create --resource-group myresourcegroup --nsg-name mynsg --name mynsg-rule --protocol Tcp --direction Inbound --source-address-prefix 0.0.0.0/0 --source-port-range "*" --destination-address-prefix "*" --destination-port-range 22 --access Allow --priority 1000
```
