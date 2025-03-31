# Amazon Cloud Development Kit (CDK)

Defining cloud infrastructure in code using familiar Object Oriented Programming languages and provisioning it through AWS CloudFormation.

[AWS CDK Docs](https://docs.aws.amazon.com/cdk/api/v2/)

## Fast Facts

| Language(s)   | Language Type | File Type(s) | Synthesizes to?                         |
|--------------|-------------|------------------|----------------------|
| Official support for TypeScript, JavaScript, Python, Java, C#, Go or potentially build your own wrapper | Object Oriented Programming Languages | OOP language files (`.py`, `.ts` etc)   | JSON CloudFormation Templates |

## Abstractions

- **Constructs**: The basic building blocks of CDK that represent AWS resources. Constructs are classes that encapsulate AWS resources and their properties
- **Stacks**: A collection of one or more constructs that represent a complete unit of deployment
- **Apps**: A collection of one or more stacks that represent your entire CDK application

## State Management

Technically, the state lives in AWS CloudFormation, but you can also look at `cdk.out/` directory locally - this has several files related to state:

- `MyStack.template.json` – the output template.
- `manifest.json` – metadata about what CDK synthesized.
- `assembly-*.json` – app-level info about the deployment.
- `cdk.context.json` – cached values from lookups and other context-dependent operations

## Available Linters

- [CDK Nag](https://github.com/cdklabs/cdk-nag)
- [eslint-plugin-cdk](https://github.com/aws-cdk/eslint-plugin-cdk)

## Important Commands

- `cdk init app --language=[your project language]`
- `cdk bootstrap`
- `cdk synth`
- `cdk diff`
- `cdk deploy`
- `cdk destroy`
- `cdk doctor`
- `cdk watch`

## Other Important Concepts

- [CDK Pipelines](https://github.com/cdklabs/cdk-pipelines-github)
- [CDK Aspects](https://docs.aws.amazon.com/cdk/latest/guide/aspects.html)
- [CDK Custom Resources](https://docs.aws.amazon.com/cdk/latest/guide/custom_resources.html)
- [CDK Asset Bundling](https://docs.aws.amazon.com/cdk/latest/guide/assets.html)
- [CDK Context](https://docs.aws.amazon.com/cdk/latest/guide/context.html)

## Good Resources for Getting Started

- [CDK Workshop](https://cdkworkshop.com/)
- [CDK Examples](https://github.com/aws-samples/aws-cdk-examples)

## Good Resources

- [CDK Labs](https://github.com/cdklabs)
- [CDK Best Practices](https://docs.aws.amazon.com/cdk/latest/guide/best-practices.html)
- [CDK Construct Hub](https://constructs.dev/)
- [Serverlessland](https://serverlessland.com/patterns?framework=AWS+CDK)