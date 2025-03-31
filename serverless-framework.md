# Serverless Framework

Build and deploy serverless applications across multiple cloud providers with a unified development experience. (Although multi-cloud is no longer supported, it was historically).

[Serverless Framework Docs](https://www.serverless.com/framework/docs/)

## Fast Facts

| Language(s)   | Language Type | File Type(s) | Synthesizes to?                         |
|--------------|-------------|------------------|----------------------|
| YAML or JSON (YAML most common) | Declarative language | `serverless.yml`, `serverless.json` | Cloud provider specific templates (e.g., CloudFormation for AWS) |

## Abstractions

- **Services**: The main unit of deployment, containing all functions, events, resources, and configurations
- **Resources**: Cloud provider resources (like DynamoDB tables, S3 buckets)
- **Plugins**: Extensions that add functionality to the framework

## State Management

Serverless Framework maintains state in several places:

- **Cloud Provider**: The deployed infrastructure state (e.g., CloudFormation for AWS)
- **Local State**: 
  - `.serverless/` directory contains deployment artifacts and state
  - `serverless.yml` defines your serverless application structure
  - `.env` files for environment variables
  - `package.json` for Node.js dependencies and scripts

## Available Linters

- [serverless-eslint](https://github.com/nishantjain91/serverless-eslint)
- [serverless-iam-roles-per-function](https://github.com/functionaltree/serverless-iam-roles-per-function)
- [serverless-pseudo-parameters](https://github.com/simondotm/serverless-pseudo-parameters)

## Important Commands

- `serverless create` - Create a new serverless project
- `serverless deploy` - Deploy your service
- `serverless remove` - Remove deployed service
- `serverless info` - Display information about the deployed service
- `serverless invoke` - Invoke deployed function
- `serverless logs` - Display function logs
- `serverless print` - Print your compiled and resolved config
- `serverless package` - Package your service
- `serverless offline` - Run service locally

## Other Important Concepts

- [Serverless Dashboard](https://www.serverless.com/dashboard/)
- [Serverless Variables](https://www.serverless.com/framework/docs/providers/aws/guide/variables/)
- [Serverless IAM](https://www.serverless.com/framework/docs/providers/aws/guide/iam/)
- [Serverless Monitoring](https://www.serverless.com/framework/docs/providers/aws/guide/monitoring/)
- [Serverless CI/CD](https://www.serverless.com/framework/docs/guides/cicd/)

## Good Resources for Getting Started

- [Serverless Framework Examples](https://github.com/serverless/examples)
- [Serverless Framework Workshops](https://www.serverless.com/learn/)

## Good Resources

- [Serverless Framework Best Practices](https://www.serverless.com/framework/docs/best-practices/)
- [Serverless Framework Blog](https://www.serverless.com/blog/)
- [Serverless Framework Forum](https://forum.serverless.com/)
- [Serverless Framework GitHub](https://github.com/serverless/serverless)
- [Serverless Land](https://serverlessland.com/patterns?framework=Serverless+Framework)
