To configure file storage in an Azure storage account using the CLI, follow these steps:
1. Open a command prompt or terminal window and run the following command to create a new file share:
```
az storage share create --account-name mystorageaccount --account-key myaccountkey --name myshare
```

* Replace `mystorageaccount` with the name of your storage account, `myaccountkey` with the access key for your storage account, and `myshare` with the name you want to give your new file share.


2. Run the following command to mount the file share on a Linux virtual machine: 
```
sudo mount -t cifs //mystorageaccount.file.core.windows.net/myshare /mnt/myshare -o vers=3.0,username=mystorageaccount,password=myaccountkey,dir_mode=0777,file_mode=0777
```
Replace `mystorageaccount` with the name of your storage account, `myaccountkey` with the access key for your storage account, `myshare` with the name of your file share, and `/mnt/myshare` with the path on your Linux virtual machine where you want to mount the file share.

