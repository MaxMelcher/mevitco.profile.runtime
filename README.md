# Mevitco ProFile - simple large file transfer solution

This repository contains the ARM template to deploy the 'self-deployment', 'self-managed' runtime to Azure.

## Disclaimer / Terms

This 'self-deployment', 'self-managed' runtime comes without support. 
If you want to have supported environment and support the further development of the solution, please consider purchasing the 'Mevitco ProFile Runtime' in Azure Marketplace.

## Pre-Requisites

Deploy the 'Mevitco ProFile Container' in your subscription - it requires an Azure Container Registry (basic or higher). You can either deploy a new one or use an existing one.

[Mevitco ProFile Container](https://azuremarketplace.microsoft.com/en-us/marketplace/apps/mevitco.profile-container?tab=Overview)

## Deployment

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FMaxMelcher%2Fmevitco.profile.runtime%2Fmain%2FmainTemplate.json)

## Configuration

After deployment (~30 seconds), you need to change the docker container. See installation / configuration guide [https://profile.mevitco.de/installation]

## Customer Usage Attribution

Please note: the deployment of this ARM template is attributed to Mevitco UG (haftungsbeschränkt), see [Customer Usage Attribution](https://docs.microsoft.com/en-us/azure/marketplace/azure-partner-customer-usage-attribution). In short: It's good for the statistics.