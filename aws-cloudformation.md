# AWS CloudFormation

Define Cloud Infrastructure in CloudFormation stacks and deploy stacks in AWS.

[CloudFormation Docs](https://docs.aws.amazon.com/cloudformation/)

## Fast Facts

| Language(s)   | Language Type | File Type(s) | Synthesizes to?                         |
|--------------|-------------|------------------|----------------------|
| YAML or JSON (YAML most common option)| Declaritive language | `.yml`, `.yaml`, `.json` | CloudFormation templates stored in S3 |

## Abstractions

- **Resources**: The basic building blocks of CloudFormation that represent AWS services (like EC2 instances, S3 buckets, IAM roles). Each resource has properties that define its configuration and behavior
- **Stacks**: A collection of AWS resources that you manage as a single unit
- **Stack sets**: Enable you to create, update, or delete stacks across multiple accounts and regions with a single operation
- **Nested stacks**: Allow you to create reusable templates and reference them from other templates

## State Management

CloudFormation maintains the state of your infrastructure in AWS:

- **Stack Resources**: All resources created and managed by CloudFormation
- **Stack Events**: History of all changes made to your stack
- **Stack Outputs**: Values that you can use to reference resources in other stacks
- **Change Sets**: Preview of changes before applying them to your stack

## Available Linters

- [cfn-lint](https://github.com/aws-cloudformation/cfn-lint)
- [CloudFormation Guard](https://github.com/aws-cloudformation/cloudformation-guard)

## Important Commands

- `aws cloudformation create-stack`
- `aws cloudformation update-stack`
- `aws cloudformation delete-stack`
- `aws cloudformation describe-stacks`
- `aws cloudformation list-stacks`
- `aws cloudformation create-change-set`

## Other Important Concepts

- [Custom Resources](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/template-custom-resources.html)
- [Stack Policies](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/protect-stack-resources.html)
- [Stack Exports](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-stack-exports.html)
- [Stack Drift Detection](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-stack-drift.html)

## Good Resources for Getting Started

- [AWS CloudFormation User Guide](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/Welcome.html)

## Good Resources

- [AWS CloudFormation Best Practices](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/best-practices.html)