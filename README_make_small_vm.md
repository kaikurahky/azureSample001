# Creates VM from Azure CLI
## Commands to execute

- az login
- az --version
- az group create --name testVM --location "eastus"

- az group deployment validate --resource-group testVM --template-uri https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/101-vm-simple-windows/azuredeploy.json --parameters adminUsername=$USERNAME --parameters adminPassword=$PASSWORD --parameters dnsLabelPrefix=$DNS_LABEL_PREFIX

- az group deployment create --name MyDeployment  --resource-group testVM --template-uri https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/101-vm-simple-windows/azuredeploy.json --parameters adminUsername=$USERNAME --parameters adminPassword=$PASSWORD --parameters dnsLabelPrefix=$DNS_LABEL_PREFIX 

## end of the file

