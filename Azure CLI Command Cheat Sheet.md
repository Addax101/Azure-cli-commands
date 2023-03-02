Azure CLI Command Cheat Sheet
1. az login
Description: Log in to an Azure account.
Usage: az login
2. az account set
Description: Set the active subscription for the current Azure account.
Usage: az account set --subscription <subscription-id>
3. az group create
Description: Create a new resource group in Azure.
Usage: az group create --name <group-name> --location <location>
4. az group delete
Description: Delete a resource group in Azure.
Usage: az group delete --name <group-name>
5. az vm create
Description: Create a new virtual machine in Azure.
Usage: az vm create --name <vm-name> --resource-group <group-name> --image <image-name> --admin-username <username> --admin-password <password> --authentication-type <auth-type>
6. az vm start
Description: Start a virtual machine in Azure.
Usage: az vm start --name <vm-name> --resource-group <group-name>
7. az vm stop
Description: Stop a virtual machine in Azure.
Usage: az vm stop --name <vm-name> --resource-group <group-name>
8. az vm list
Description: List all virtual machines in a resource group.
Usage: az vm list --resource-group <group-name>
9. az webapp create
Description: Create a new web app in Azure.
Usage: az webapp create --name <app-name> --resource-group <group-name> --plan <plan-name>
10. az webapp list
Description: List all web apps in a resource group.
Usage: az webapp list --resource-group <group-name>
11. az webapp delete
Description: Delete a web app in Azure.
Usage: az webapp delete --name <app-name> --resource-group <group-name>
12. az webapp config set
Description: Set configuration settings for a web app in Azure.
Usage: az webapp config set --name <app-name> --resource-group <group-name> --java-version <version> --java-container <container> --java-container-version <container-version>
13. az mysql server create
Description: Create a new MySQL server in Azure.
Usage: az mysql server create --resource-group <group-name> --name <server-name> --location <location> --admin-user <username> --admin-password <password> --sku-name <sku-name>
14. az mysql server firewall-rule create
Description: Create a new firewall rule for a MySQL server in Azure.
Usage: az mysql server firewall-rule create --resource-group <group-name> --server-name <server-name> --name <rule-name> --start-ip-address <start-ip> --end-ip-address <end-ip>
15. az mysql db create
Description: Create a new MySQL database in Azure.
Usage: az mysql db create --resource-group <group-name> --server-name <server-name> --name <db-name>
16. az mysql db list
Description: List all MySQL databases in a server.
Usage: az mysql db list --resource-group <group-name> --server-name <server-name>
