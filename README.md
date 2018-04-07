# hellnode
hello nodejs app

Following the tuturial
[Create a Node.js web app in Azure](https://docs.microsoft.com/en-us/azure/app-service/app-service-web-get-started-nodejs)


20180403 Added files from hello nodejs sample for azure here.

## Create new github repo

https://github.com/biosgis/hellnode

## Clone the repo to local folder

## Create a project zip file 

hellnode.zip


## Create resource group

20180404 Azure Cloud Shell fail

ERROR MSG: 
Failed to connect terminal: websocket cannot be established. Press "Enter" to reconnect.

20180406

az group create --name biosgis --location "West US"

## Create an Azure App Service plan

az appservice plan create --name biosgis --resource-gropu biosgis --sku FREE

## Create a web app

az webapp create --resource-group biosgis --plan biosgis --name hellnode --runtime "NODE|6.9"

Manuel Method: 
1. Create (Add) app service, type: Node JS Empty Web App
2. App name: biosbeta.azurewebsites.net, Subscription: VSEnt, 
3. Resource Group: biosgis (Use existing), OS: Windows, 
4. App Service plan/Location: biosgis(West US), Application Insights: Off
5. Pin to dashboard =Yes, Create...

Created new website 

# Node JS empty site
[![Deploy to Azure](http://azuredeploy.net/deploybutton.png)](https://azuredeploy.net/)

## Deploy ZIP file

Go to https://biosbeta.scm.azurewebsites.net/ZipDeploy

Some file types will be downloaded, others displayed in browser, like 
https://biosbeta.scm.azurewebsites.net/api/vfs/site/wwwroot/server.js

Downloaded files from above site, but azuredeploy json file contains errors:
