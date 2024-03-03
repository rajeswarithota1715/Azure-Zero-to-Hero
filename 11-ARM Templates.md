#  Azure Resource manager Templates 

ARM us responsible dor creating resoirces in Azure
there are multiple ways to create the resources in Azure

*  Azure UI/Portal
*  Azure CLI
*  ARM Templates
*  Bicep
*  SDK

you can create the resources by using any of the above method , whatever the methos you used you need to provide the required details to create the resources , 
it will send those deatils to Azure resource Manager , ARM will connect to Azure using some API's and create the resources .

you might think why can't these directly connect to Azure insted of ARM , the answer is to provide the Standardization


ARM templates is one of the service provide by Azure to create the resources , ARM templates are written in JSON format 

User will create ARM Templates using JSON , ARM templates will submit the request to ARM , ARM will create the resources in Azure 

User writes -> ARM Templates in JSON-> ARM -> Azure resource

we need Azure CLI to submit the ARM Template to ARM
use VS code with Azure Resource Manager extensionfor easy writing the code as you will get auto recommendations and defaults syntax 
where you just need to change the values accordingly .

**ARM Template for Storage**
<pre>
  {
    "$schema": "https://schema.management.azure.com/schemas/2019-04-01/deploymentTemplate.json#",
    "contentVersion": "1.0.0.0",
    "parameters": {},
    "functions": [],
    "variables": {},
    "resources": [
        {
            "name": "abhioshekveeramalla11232",
            "type": "Microsoft.Storage/storageAccounts",
            "apiVersion": "2023-01-01",
            "tags": {
                "displayName": "abhioshekveeramalla11232"
            },
            "location": "[resourceGroup().location]",
            "kind": "StorageV2",
            "sku": {
                "name": "Premium_LRS",
                "tier": "Premium"
            }
        }
    ],
    "outputs": {}
}
</pre>

<pre>
  Create a resource group
  az group create --name vscode --location 'Central US'
  switch to the right folder where your coed is there and run the below command
  az deployment group create --resource-group vscode --template-file 01-storage-account.json
</pre>
