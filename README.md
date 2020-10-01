Log in to azure command on Azure CLI with `az login`

Use the following command below to create the resource group:
```
az group create --name jiveLogicApp --location central us
```

Use the following command below to deploy resources:
```
az deployment group create \
  --name deployServices \
  --resource-group jiveLogicApp \
  --template-file azuredeploy.json \
  --parameters $prodParameterFile
```
