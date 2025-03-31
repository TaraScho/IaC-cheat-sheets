# Azure Bicep

Define Azure infrastructure using a simpler, more concise language that compiles to ARM templates.

[Azure Bicep Docs](https://learn.microsoft.com/en-us/azure/azure-resource-manager/bicep/)

## Fast Facts

| Language(s)   | Language Type | File Type(s) | Synthesizes to?                         |
|--------------|-------------|------------------|----------------------|
| Bicep | Declarative language | `.bicep` | Azure Resource Manager (ARM) JSON templates |

## Abstractions

- **Resources**: Azure resources defined using Bicep syntax
- **Parameters**: Input values that can be passed to your template
- **Variables**: Reusable values within your template
- **Outputs**: Values that can be referenced by other templates
- **Modules**: Reusable Bicep files that can be called from other files
- **Target Scopes**: The scope where resources are deployed (subscription, resource group, etc.)
- **Conditions**: Logic to control resource deployment
- **Loops**: Iterate over resources or properties

## State Management

Bicep maintains state in several places:

- **Azure**: The actual state of resources in Azure
- **Local State**: 
  - `*.bicep` files - Bicep template definitions
  - `parameters.json` - Parameter values
  - `.bicepconfig` - Bicep configuration file
  - `bicep.lock.json` - Lock file for dependencies

## Available Linters

- [Bicep Linter](https://learn.microsoft.com/en-us/azure/azure-resource-manager/bicep/linter)
- [ARM-TTK](https://github.com/Azure/arm-ttk)
- [Bicep VS Code Extension](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-bicep)

## Important Commands

- `az bicep build` - Compile Bicep to ARM JSON
- `az bicep decompile` - Convert ARM JSON to Bicep
- `az bicep publish` - Publish module to registry
- `az bicep restore` - Restore external modules
- `az bicep install` - Install Bicep CLI
- `az bicep upgrade` - Upgrade Bicep CLI
- `az bicep version` - Show Bicep version
- `az deployment sub create` - Deploy to subscription
- `az deployment group create` - Deploy to resource group

## Other Important Concepts

- [Bicep Modules](https://learn.microsoft.com/en-us/azure/azure-resource-manager/bicep/modules)
- [Bicep Parameters](https://learn.microsoft.com/en-us/azure/azure-resource-manager/bicep/parameters)
- [Bicep Variables](https://learn.microsoft.com/en-us/azure/azure-resource-manager/bicep/variables)
- [Bicep Outputs](https://learn.microsoft.com/en-us/azure/azure-resource-manager/bicep/outputs)
- [Bicep Functions](https://learn.microsoft.com/en-us/azure/azure-resource-manager/bicep/bicep-functions)
- [Bicep Loops](https://learn.microsoft.com/en-us/azure/azure-resource-manager/bicep/loops)
- [Bicep Conditions](https://learn.microsoft.com/en-us/azure/azure-resource-manager/bicep/conditions)
- [Bicep Dependencies](https://learn.microsoft.com/en-us/azure/azure-resource-manager/bicep/dependencies)

## Good Resources for Getting Started

- [Bicep Tutorial](https://learn.microsoft.com/en-us/azure/azure-resource-manager/bicep/learn-bicep)
- [Bicep Examples](https://github.com/Azure/bicep/tree/main/docs/examples)
- [Bicep Workshop](https://github.com/Azure/bicep/tree/main/docs/workshops)

## Good Resources

- [Bicep Best Practices](https://learn.microsoft.com/en-us/azure/azure-resource-manager/bicep/best-practices)
- [Bicep Registry](https://github.com/Azure/bicep-registry)
- [Azure Architecture Center](https://learn.microsoft.com/en-us/azure/architecture/)
- [Azure Blog](https://azure.microsoft.com/blog/)
- [Azure GitHub](https://github.com/Azure)
- [Azure Community](https://techcommunity.microsoft.com/t5/azure/ct-p/Azure)
- [Serverlessland](https://serverlessland.com/patterns?framework=Azure)
