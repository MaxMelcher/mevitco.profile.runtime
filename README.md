# Mevitco ProFile - simple large file transfer solution

This repository contains the ARM template to deploy the 'self-deployment', 'self-managed' runtime to Azure.

## Disclaimer / Terms

This 'self-deployment', 'self-managed' runtime comes without support. 
If you want to have supported environment and support the further development of the solution, please consider purchasing the 'Mevitco ProFile Runtime' in Azure Marketplace.

## Pre-Requisites

Deploy the 'Mevitco ProFile Container' in your subscription - it requires an Azure Container Registry (basic or higher). You can either deploy a new one or use an existing one.

[Mevitco ProFile Container](https://azuremarketplace.microsoft.com/en-us/marketplace/apps/mevitco.profile-container?tab=Overview)

You need to have contributor access to a subscription or resource group.

## Deployment

With the following button you can deploy the runtime into your Azure subscription.
* Azure Web App (P1V2)
* Azure Storage Account (hot, RA-GRS)
* Pre-Configuration for the container solution

The parameters that you need to provide: 

* Subscription
* Resource Group (new or existing)
* Profile Name: the name of the website and the storage account. Must be globally unique. Please check [yourname].azurewebsites.net for availability before you deploy.
* Region (Azure region to deploy both the Storage and the App Service)
* Admin Password (required to access statistics and setup page)
* Admin Email (required to show the statistics and setup page, requires authentication)
* Azure Container Registry Login Server, e.g mevitco.azurecr.io
* Azure Container Registry Username
* Azure Container Registry Password

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FMaxMelcher%2Fmevitco.profile.runtime%2Fmain%2FmainTemplate.json)

Deployment takes roughly 30 seconds.

## Post-Deployment Configuration

After deployment (~30 seconds). Afterwards the container will be automatically downloaded and provisioned (~60 seconds).

It will be available at https://[Profile Name].azurewebsites.net (replace the Profile Name with the name you provided during provisioning).

Afterwards you can configure the solution: [https://profile.mevitco.de/installation](https://profile.mevitco.de/installation)

## Customer Usage Attribution

Please note: the deployment of this ARM template is attributed to Mevitco UG (haftungsbeschränkt), see [Customer Usage Attribution](https://docs.microsoft.com/en-us/azure/marketplace/azure-partner-customer-usage-attribution). In short: It's good for the statistics.