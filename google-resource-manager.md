# Google Cloud Resource Manager

Manage and organize Google Cloud resources hierarchically using projects, folders, and organizations.

[Google Cloud Resource Manager Docs](https://cloud.google.com/resource-manager/docs)

## Fast Facts

| Language(s)   | Language Type | File Type(s) | Synthesizes to?                         |
|--------------|-------------|------------------|----------------------|
| YAML, JSON | Declarative language | `.yaml`, `.yml`, `.json` | Google Cloud API |

## Abstractions

- **Organizations**: The root node in the Google Cloud resource hierarchy
- **Folders**: Logical groupings of projects and other folders
- **Projects**: The base unit for organizing resources and enabling billing
- **IAM Policies**: Access control policies for resources
- **Resource Tags**: Key-value pairs for organizing and managing resources
- **Resource Types**: Different types of Google Cloud resources (Compute, Storage, etc.)

## State Management

Resource Manager maintains state in several places:

- **Google Cloud**: The actual state of resources in Google Cloud
- **Local State**: 
  - `gcloud` configuration files
  - Deployment manager configurations
  - Terraform state (if using Terraform)
  - Local configuration files

## Available Linters

- [Cloud Foundation Toolkit](https://github.com/GoogleCloudPlatform/cloud-foundation-toolkit)
- [Forseti Security](https://github.com/forseti-security/forseti-security)
- [Cloud Security Command Line](https://cloud.google.com/sdk/gcloud/reference/security)

## Important Commands

- `gcloud resource-manager folders create` - Create a new folder
- `gcloud projects create` - Create a new project
- `gcloud projects set-iam-policy` - Set IAM policy for a project
- `gcloud resource-manager tags create` - Create a new tag
- `gcloud resource-manager tags bindings create` - Create a tag binding
- `gcloud projects get-iam-policy` - Get IAM policy for a project
- `gcloud projects describe` - Get project details
- `gcloud projects list` - List all projects
- `gcloud resource-manager folders list` - List all folders

## Other Important Concepts

- [Resource Hierarchy](https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy)
- [IAM and Access Control](https://cloud.google.com/iam/docs)
- [Resource Tags](https://cloud.google.com/resource-manager/docs/tags/tags-overview)
- [Organization Policies](https://cloud.google.com/resource-manager/docs/organization-policy/overview)
- [Resource Quotas](https://cloud.google.com/resource-manager/docs/quotas)
- [Resource Labels](https://cloud.google.com/resource-manager/docs/creating-managing-labels)
- [Resource Monitoring](https://cloud.google.com/monitoring)

## Good Resources for Getting Started

- [Google Cloud Resource Manager Tutorial](https://cloud.google.com/resource-manager/docs/creating-managing-projects)
- [Cloud Foundation Toolkit Examples](https://github.com/GoogleCloudPlatform/cloud-foundation-toolkit/tree/master/dm/templates)
- [How to Get Started with Infrastructure as Code (IaC) on GCP](https://www.pluralsight.com/resources/blog/cloud/how-to-get-started-with-infrastructure-as-code-iac-on-gcp)

## Good Resources

- [Google Cloud Best Practices](https://cloud.google.com/docs/enterprise/best-practices-for-enterprise-organizations)
- [Cloud Foundation Toolkit](https://cloud.google.com/foundation-toolkit)
- [Google Cloud Blog](https://cloud.google.com/blog/products/identity-security)
- [Google Cloud GitHub](https://github.com/GoogleCloudPlatform)
- [Google Cloud Community](https://cloud.google.com/community)
- [Google Cloud Security](https://cloud.google.com/security)
- [Serverlessland](https://serverlessland.com/patterns?framework=GoogleCloud)
