# Azure-Container-App
Azure Container Apps take the concept of a managed Kubernetes cluster a step further and manages the cluster environment as well as provides other managed services on top of the cluster.
Task 1: Create and configure an Azure Container App and environment
Azure Container Apps take the concept of a managed Kubernetes cluster a step further and manages the cluster environment as well as provides other managed services on top of the cluster. Unlike an Azure Kubernetes cluster, where you must still manage the cluster, an Azure Container Apps instance removes some of the complexity to setting up a Kubernetes cluster.
From the Azure portal, search for and select Container Apps.
From Container Apps, select Create.
Use the following information to fill out the details on the Basics tab.*.
Setting
Action
Subscription
Select your Azure subscription
Resource group
az104-rg9
Container app name
my-app
Region
East US (Or a region available near you)
Container Apps Environment
Select Create new > Set Environment name to my-environment > Create

On the Container tab, ensure that Use quickstart image is enabled and that the quickstart image is set to Simple hello world container.
Select the Review and create and then Create.
Note: Wait for the container app to deploy. This will take a couple of minutes.
Task 2: Test and verify deployment of the Azure Container App
By default, the Azure container app that you create will accept traffic on port 80 using the sample Hello World application. Azure Container Apps will provide a DNS name for the application. Copy and navigate to this URL to ensure that the application is up and running.
Select Go to resource to view your new container app.
Select the link next to Application URL to view your application.

Verify you receive the Your Azure Container Apps app is live message.
Cleanup your resources
If you are working with your own subscription take a minute to delete the lab resources. This will ensure resources are freed up and cost is minimized. The easiest way to delete the lab resources is to delete the lab resource group.
In the Azure portal, select the resource group, select Delete the resource group, Enter resource group name, and then click Delete.
Using Azure PowerShell, Remove-AzResourceGroup -Name resourceGroupName.
Using the CLI, az group delete --name resourceGroupName.
