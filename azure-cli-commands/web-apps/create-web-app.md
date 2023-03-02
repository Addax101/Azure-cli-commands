## Create a new web app in Azure using the CLI
To create a new web app in Azure using the CLI, follow these steps:

* Open a command prompt or terminal window and run the following command to create a new resource group: `az group create --name myResourceGroup --location eastus`

Replace `myResourceGroup` with the name of the resource group you want to create, and `eastus` with the location where you want to create the resource group.

* Run the following command to create a new web app:
az webapp create \
--resource-group myResourceGroup \
--name myWebApp \
--runtime "PYTHON|3.8"

Replace `myResourceGroup` with the name of the resource group you created in step 1, myWebApp with the name you want to give your web app, and `PYTHON|3.8` with the runtime you want to use for your web app. You can also add other parameters to customize your web app, such as `--plan myPlan` to specify the name of an existing app service plan to use.

* Wait for the web app to be created. You can use the following command to check the status of the web app:
`az webapp show --resource-group myResourceGroup --name myWebApp --query state`

This command should return the state of the web app (e.g. "Running").

Congratulations! You have now created a new web app in Azure using the CLI.