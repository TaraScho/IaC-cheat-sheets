# AWS Serverless Application Model (SAM)

Build serverless applications using a simplified syntax and deploy them to AWS Lambda and other serverless services.

[AWS SAM Docs](https://docs.aws.amazon.com/serverless-application-model/)

## Fast Facts

| Language(s)   | Language Type | File Type(s) | Synthesizes to?                         |
|--------------|-------------|------------------|----------------------|
| YAML or JSON (YAML most common) | Declarative language | `.yml`, `.yaml`, `.json` | CloudFormation templates |

## Abstractions

- **Resources**: Serverless resources like Lambda functions, API Gateway APIs, and DynamoDB tables
- **SAM Templates**: AWS SAM templates are an extension of AWS CloudFormation templates, with unique syntax types that use shorthand syntax with fewer lines of code than AWS CloudFormation.

## State Management

SAM maintains state in several places:

- **CloudFormation**: The synthesized CloudFormation template manages the infrastructure state
- **Local State**: 
  - `.aws-sam/` directory contains build artifacts and local state
  - `samconfig.toml` stores deployment configurations and parameters
  - `template.yaml` defines your serverless application structure

## Available Linters

- [SAM CLI](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-install.html) includes built-in template validation
- AWS SAM Accelerate for local development

## Important Commands

- `sam init` - Create a new SAM application
- `sam build` - Build your application
- `sam deploy` - Deploy your application
- `sam local invoke` - Test functions locally
- `sam local start-api` - Run API Gateway locally
- `sam logs` - View function logs
- `sam sync` - Sync local changes to AWS
- `sam validate` - Validate your template

## Other Important Concepts

- [SAM Accelerate](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-accelerate.html)
- [SAM Local](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-using-sam-local.html)
- [SAM Policy Templates](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-policy-templates.html)
- [SAM Parameter Store](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-using-parameter-store.html)

## Good Resources for Getting Started

## Good Resources

- [SAM Best Practices](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-best-practices.html)
- [SAM GitHub Repository](https://github.com/aws/aws-sam-cli)
- [Serverlessland](https://serverlessland.com/patterns?framework=AWS+SAM)
