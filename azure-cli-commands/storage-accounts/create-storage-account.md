## create-storage-account.md
To create a storage account in Azure using the CLI, follow these steps:

* Open a command prompt or terminal window and run the following command to create a new resource group:
`az group create --name myResourceGroup --location eastus`

Replace `myResourceGroup` with the name you want to give your new resource group, and `eastus` with the location you want to use for your storage account.

* Run the following command to create a new storage account:
`az storage account create \
--name mystorageaccount \
--resource-group myResourceGroup \
--location eastus \
--sku Standard_LRS \
--kind StorageV2`

Replace `mystorageaccount` with the name you want to give your new storage account.

* Wait for the storage account to be created. You can use the following command to check the status of the storage account:
`az storage account show --name mystorageaccount --resource-group myResourceGroup --query 'provisioningState'`

This command should return `"Succeeded" `once the storage account has been created.

Congratulations! You have now created a new storage account in Azure using the CLI.