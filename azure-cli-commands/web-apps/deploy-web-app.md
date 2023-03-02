## Deploy a web app in Azure using the CLI
To deploy a web app in Azure using the CLI, follow these steps:

* Open a command prompt or terminal window and navigate to the folder where your web app files are located.

Run the following command to deploy your web app:
`az webapp up \
--resource-group myResourceGroup \
--name myWebApp`

Replace `myResourceGroup` with the name of the resource group where your web app is located, and `myWebApp` with the name of the web app you want to deploy.

* Wait for the deployment to complete. You can use the following command to check the status of the web app: `az webapp show --resource-group myResourceGroup --name myWebApp --query state`

This command should return the state of the web app (e.g. "Running").

Congratulations! You have now deployed a web app in Azure using the CLI.