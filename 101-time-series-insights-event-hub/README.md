# Azure Time Series Insights ARM deployment

[![Deploy to Azure](https://azuredeploy.net/deploybutton.svg)](https://azuredeploy.net/?repository=https://github.com/murdockcrc/azure-quickstart-templates/tree/luisdel-tsi/101-time-series-insights-event-hub)

Use these automation scripts to automate the deployment and configuration of a TSI (Time Series Insights) environment.

These automation artifacts assume you are use the Azure CLI to provision the environment. Typically, the command flow would look like this:

``` bash
az login
azure account set --subscription <subscription-id>
az group deployment create --name tsi-<some-id> --resource-group <rg-name> --template-file azuredeploy.json --parameters azuredeploy.parameters.json
```