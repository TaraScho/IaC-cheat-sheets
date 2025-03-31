# Terraform

Define and provision infrastructure using a declarative configuration language that works with multiple cloud providers.

[Terraform Docs](https://www.terraform.io/docs/)

## Fast Facts

| Language(s)   | Language Type | File Type(s) | Synthesizes to?                         |
|--------------|-------------|------------------|----------------------|
| HCL (HashiCorp Configuration Language) or JSON | Declarative language | `.tf`, `.tfvars`, `.tfstate`, `.tf.json` | Cloud provider APIs (e.g., AWS API for AWS) |

## Abstractions

- **Resources**: Cloud provider resources defined using HCL syntax
- **Data Sources**: Read-only resources that fetch data from cloud providers
- **Variables**: Input values that can be passed to your configuration
- **Modules**: Reusable packages of Terraform configurations
- **Providers**: Plugins that let Terraform interact with cloud platforms

## State Management

Terraform maintains state in several places:

- **Backend**: State is stored in a backend (local, S3, Azure Storage, etc.)
- **Local State**: 
  - `terraform.tfstate` contains the current state
  - `terraform.tfvars` contains variable values
  - `*.tf` files contain your infrastructure code
  - `.terraform/` directory contains provider plugins

## Available Linters

- [TFLint](https://github.com/terraform-linters/tflint)
- [Checkov](https://github.com/bridgecrewio/checkov)
- [TFSec](https://github.com/tfsec/tfsec)

## Important Commands

- `terraform init` - Initialize a working directory
- `terraform plan` - Show execution plan
- `terraform apply` - Apply the changes
- `terraform destroy` - Destroy infrastructure
- `terraform fmt` - Format configuration files
- `terraform validate` - Validate configuration
- `terraform import` - Import existing resources
- `terraform workspace` - Manage workspaces
- `terraform state` - State management commands
- `terraform output` - Show output values

## Other Important Concepts

- [Terraform Outputs](https://www.terraform.io/docs/configuration/outputs.html)
- [Terraform Workspaces](https://www.terraform.io/docs/state/workspaces.html)
- [Terraform Modules](https://www.terraform.io/docs/modules/index.html)
- [Terraform Providers](https://www.terraform.io/docs/providers/index.html)
- [Terraform State](https://www.terraform.io/docs/state/index.html)
- [Terraform Variables](https://www.terraform.io/docs/configuration/variables.html)
- [Terraform Backends](https://www.terraform.io/docs/backends/index.html)
- [Terraform Workspaces](https://www.terraform.io/docs/state/workspaces.html)

## Good Resources for Getting Started

- [Terraform Tutorials](https://learn.hashicorp.com/terraform)
- [Terraform Examples](https://github.com/hashicorp/terraform-provider-aws/tree/main/examples)

## Good Resources

- [Terraform Best Practices](https://www.terraform.io/docs/cloud/guides/recommended-practices/index.html)
- [Terraform Registry](https://registry.terraform.io/)
- [Terraform Blog](https://www.hashicorp.com/blog/category/terraform)
- [Terraform GitHub](https://github.com/hashicorp/terraform)
- [Terraform Community](https://discuss.hashicorp.com/c/terraform-core/27)
- [Terraform Security](https://www.terraform.io/docs/cloud/guides/security/index.html)
- [Serverlessland](https://serverlessland.com/patterns?framework=Terraform)

