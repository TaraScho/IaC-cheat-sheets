# OpenTofu

An open-source fork of Terraform that provides infrastructure as code capabilities with enhanced features and community-driven development.

[OpenTofu Docs](https://opentofu.org/docs/intro/)

## Fast Facts

| Language(s)   | Language Type | File Type(s) | Synthesizes to?                         |
|--------------|-------------|------------------|----------------------|
| HCL (HashiCorp Configuration Language) or JSON | Declarative language | `.tf`, `.tfvars`, `.tfstate`, `.tf.json` | Cloud provider APIs (e.g., AWS API for AWS) |

## Abstractions

- **Resources**: Cloud provider resources defined using HCL syntax
- **Data Sources**: Read-only resources that fetch data from cloud providers
- **Modules**: Reusable packages of OpenTofu configurations
- **Providers**: Plugins that let OpenTofu interact with cloud platforms
- **State**: A record of the current state of your infrastructure

## State Management

OpenTofu maintains state in several places:

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

- `tofu init` - Initialize a working directory
- `tofu plan` - Show execution plan
- `tofu apply` - Apply the changes
- `tofu destroy` - Destroy infrastructure
- `tofu fmt` - Format configuration files
- `tofu validate` - Validate configuration
- `tofu import` - Import existing resources
- `tofu workspace` - Manage workspaces
- `tofu state` - State management commands
- `tofu output` - Show output values

## Other Important Concepts

- [OpenTofu Outputs](https://opentofu.org/docs/language/values/outputs/)
- [OpenTofu Workspaces](https://opentofu.org/docs/language/state/workspaces/)
- [OpenTofu Modules](https://opentofu.org/docs/language/modules/)
- [OpenTofu Providers](https://opentofu.org/docs/language/providers/)
- [OpenTofu State](https://opentofu.org/docs/language/state/)
- [OpenTofu Variables](https://opentofu.org/docs/language/values/variables/)
- [OpenTofu Backends](https://opentofu.org/docs/language/settings/backends/)
- [OpenTofu State Locking](https://opentofu.org/docs/language/state/locking/)

## Good Resources for Getting Started

- [OpenTofu Tutorials](https://opentofu.org/docs/intro/tutorials/)
- [OpenTofu Examples](https://github.com/opentofu/opentofu/tree/main/examples)

## Good Resources

- [OpenTofu Best Practices](https://opentofu.org/docs/language/best-practices/)
- [OpenTofu Registry](https://registry.opentofu.org/)
- [OpenTofu Blog](https://opentofu.org/blog/)
- [OpenTofu GitHub](https://github.com/opentofu/opentofu)
- [OpenTofu Community](https://opentofu.org/community)
- [OpenTofu Security](https://opentofu.org/docs/language/security/)
- [Serverlessland](https://serverlessland.com/patterns?framework=OpenTofu)
