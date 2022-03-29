# Dapr Application Deployed to Azure Container Apps

## Creating state store

``` pwsh
az group create -n rg-azca-dev-001 -l westeurope --debug

az storage account create -n stazcadev001 -g rg-azca-dev-001 -l westeurope --sku Standard_LRS --debug
```

Manually created a container called `statestore`. 

Then added a file called `statestore.yaml` under `C:\Users\???\.dapr\components`, something like [this](https://docs.dapr.io/reference/components-reference/supported-state-stores/setup-azure-blobstorage/).
