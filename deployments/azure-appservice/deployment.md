## Create Resource Group
`az group create --name [resource-group-name] --location swedencentral`

## Create AppService Plan where the Webapps are hosted
`az appservice plan create --name AppServicePlan4Vampi --resource-group [resource-group-name] --is-linux`

## Create Webapps ; one that is vulnerable, one that is made not vulnerable with intent
`az webapp create --resource-group [resource-group-name] --plan AppServicePlan4Vampi --name [webapp-secure-name] --multicontainer-config-type compose --multicontainer-config-file docker-compose-vampi-secure.yaml`
`az webapp create --resource-group [resource-group-name] --plan AppServicePlan4Vampi --name [webapp-isecure-name] --multicontainer-config-type compose --multicontainer-config-file docker-compose-vampi-insecure.yaml`
