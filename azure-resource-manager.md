# Azure Resource Manager (ARM)

Define Azure infrastructure using JSON templates that describe the desired state of your Azure resources.

[Azure Resource Manager Docs](https://learn.microsoft.com/en-us/azure/azure-resource-manager/)

## Fast Facts

| Language(s)   | Language Type | File Type(s) | Synthesizes to?                         |
|--------------|-------------|------------------|----------------------|
| JSON | Declarative language | `.json` | Azure Resource Manager API calls |

## Abstractions

- **Resources**: Azure resources defined using JSON syntax
- **Parameters**: Input values that can be passed to your template
- **Variables**: Reusable values within your template
- **Outputs**: Values that can be referenced by other templates
- **Nested Templates**: Reusable JSON templates that can be called from other templates
- **Linked Templates**: External templates referenced by URL
- **Conditions**: Logic to control resource deployment
- **Copy**: Iterate over resources or properties

## State Management

ARM maintains state in several places:

- **Azure**: The actual state of resources in Azure
- **Local State**: 
  - `*.json` files - ARM template definitions
  - `parameters.json` - Parameter values
  - `variables.json` - Variable definitions
  - `nested/` - Nested template definitions

## Available Linters

- [ARM-TTK](https://github.com/Azure/arm-ttk)
- [ARM Linter](https://marketplace.visualstudio.com/items?itemName=samcraddock.arm-linter)
- [ARM Tools](https://marketplace.visualstudio.com/items?itemName=msazurermtools.azurerm-vscode-tools)

## Important Commands

- `az deployment sub create` - Deploy to subscription
- `az deployment group create` - Deploy to resource group
- `az deployment mg create` - Deploy to management group
- `az deployment tenant create` - Deploy to tenant
- `az deployment operation list` - List deployment operations
- `az deployment operation show` - Show deployment operation
- `az deployment validate` - Validate template
- `az deployment export` - Export deployment template
- `az deployment what-if` - Preview changes

## Other Important Concepts

- [ARM Template Structure](https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/template-syntax)
- [ARM Parameters](https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/parameters)
- [ARM Variables](https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/variables)
- [ARM Outputs](https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/outputs)
- [ARM Functions](https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/template-functions)
- [ARM Nested Templates](https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/linked-templates)
- [ARM Conditions](https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/conditional-deployment)
- [ARM Dependencies](https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/resource-dependency)

## Good Resources for Getting Started

- [ARM Template Tutorial](https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/template-tutorial-create-first-template)
- [ARM Quickstart Templates](https://github.com/Azure/azure-quickstart-templates)
- [ARM Template Workshop](https://github.com/Azure/azure-quickstart-templates/tree/master/quickstarts/microsoft.resources/template-tutorial)

## Good Resources

- [ARM Best Practices](https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/best-practices)
- [ARM Template Reference](https://learn.microsoft.com/en-us/azure/templates/)
- [Azure Architecture Center](https://learn.microsoft.com/en-us/azure/architecture/)
- [Azure Blog](https://azure.microsoft.com/blog/)
- [Azure GitHub](https://github.com/Azure)
- [Azure Community](https://techcommunity.microsoft.com/t5/azure/ct-p/Azure)
- [Serverlessland](https://serverlessland.com/patterns?framework=Azure)
