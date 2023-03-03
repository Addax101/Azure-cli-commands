To configure file storage in an Azure storage account using the CLI, follow these steps:
1. Open a command prompt or terminal window and run the following command to create a new file share:
```
az storage share create --account-name mystorageaccount --account-key myaccountkey --name myshare
```

* Replace `mystorageaccount` with the name of your storage account, `myaccountkey` with the access key for your storage account, and `myshare` with the name you want to give your new file share.
