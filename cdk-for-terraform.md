# CDK for Terraform (CDKTF)

Define Terraform infrastructure using familiar programming languages while leveraging Terraform's ecosystem and providers.

[CDKTF Docs](https://developer.hashicorp.com/terraform/cdktf)

## Fast Facts

| Language(s)   | Language Type | File Type(s) | Synthesizes to?                         |
|--------------|-------------|------------------|----------------------|
| TypeScript, Python, Java, C#, Go | Object Oriented Programming Languages | `.ts`, `.py`, `.java`, `.cs`, `.go` | Terraform HCL and JSON |

## Abstractions

- **Constructs**: Reusable cloud components that represent Terraform resources
- **Stacks**: A collection of constructs that represent a complete unit of deployment
- **App**: The root of your CDKTF application, containing one or more stacks
- **Providers**: Terraform providers that let you use cloud resources
- **Data Sources**: Read-only resources that fetch data from cloud providers

## State Management

CDKTF maintains state in several places:

- **Terraform State**: State is managed by Terraform (local, S3, Azure Storage, etc.)
- **Local State**: 
  - `cdk.out/` directory contains synthesized Terraform files
  - `cdktf.json` defines your CDKTF project
  - `cdktf.context.json` contains cached values
  - `node_modules/` or equivalent for language dependencies

## Available Linters

- [CDKTF ESLint Plugin](https://github.com/hashicorp/cdktf-eslint-plugin)
- [CDKTF TypeScript](https://github.com/hashicorp/cdktf-cli/tree/main/packages/cdktf-cli#typescript)
- [CDKTF Python](https://github.com/hashicorp/cdktf-cli/tree/main/packages/cdktf-cli#python)

## Important Commands

- `cdktf init` - Create a new CDKTF project
- `cdktf synth` - Synthesize Terraform configuration
- `cdktf deploy` - Deploy the stack
- `cdktf destroy` - Destroy the stack
- `cdktf diff` - Show changes to be applied
- `cdktf get` - Generate provider bindings
- `cdktf provider add` - Add a provider
- `cdktf provider upgrade` - Upgrade provider versions
- `cdktf provider remove` - Remove a provider

## Other Important Concepts

- [CDKTF Constructs](https://developer.hashicorp.com/terraform/cdktf/concepts/constructs)
- [CDKTF Stacks](https://developer.hashicorp.com/terraform/cdktf/concepts/stacks)
- [CDKTF Providers](https://developer.hashicorp.com/terraform/cdktf/concepts/providers)
- [CDKTF Testing](https://developer.hashicorp.com/terraform/cdktf/testing)
- [CDKTF Modules](https://developer.hashicorp.com/terraform/cdktf/concepts/modules)
- [CDKTF Remote State](https://developer.hashicorp.com/terraform/cdktf/concepts/remote-state)
- [CDKTF Variables](https://developer.hashicorp.com/terraform/cdktf/concepts/variables)

## Good Resources for Getting Started

- [CDKTF Tutorials](https://developer.hashicorp.com/terraform/tutorials/cdktf)
- [CDKTF Examples](https://github.com/hashicorp/cdktf-examples)

## Good Resources

- [CDKTF Best Practices](https://developer.hashicorp.com/terraform/cdktf/best-practices)
- [CDKTF GitHub](https://github.com/hashicorp/cdktf-cli)
- [CDKTF Blog](https://www.hashicorp.com/blog/category/terraform)
- [CDKTF Community](https://discuss.hashicorp.com/c/terraform-core/27)
- [CDKTF Registry](https://registry.terraform.io/browse/cdktf)
