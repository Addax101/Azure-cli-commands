## configure-blob-storage.md
To configure blob storage in an Azure storage account using the CLI, follow these steps:
* Open a command prompt or terminal window and run the following command to create a new container:
```
az storage container create --name mycontainer --account-name mystorageaccount --account-key myaccountkey 
```

Replace `mystorageaccount` with the name of your storage account, `myaccountkey` with the access key for your storage account, and `mycontainer` with the name you want to give your new container.




* Run the following command to upload a file to your new container: 
```az storage blob upload --account-name mystorageaccount --account-key myaccountkey --container-name mycontainer --name myfile --type block --source /path/to/local/file
```
** Replace `mystorageaccount` with the name of your storage account, `myaccountkey` with the access key for your storage account, `mycontainer` with the name of your container, `myfile` with the name you want to give your new file, and `/path/to/local/file` with the path to the local file you want to upload.

* Wait for the file to be uploaded. You can use the following command to check the status of the upload: `az storage blob list --account-name mystorageaccount --account-key myaccountkey --container-name mycontainer --query '[].name'`


