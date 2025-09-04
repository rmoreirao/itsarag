az login
az group create --name rg-itsarag --location swedencentral
cd infra/aistudio/
az deployment group create --resource-group rg-itsarag --template-file main.bicep --parameters aiHubName=rmaih
