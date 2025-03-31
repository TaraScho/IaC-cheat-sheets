# Pulumi

Define cloud infrastructure using familiar programming languages and deploy to any cloud provider.

[Pulumi Docs](https://www.pulumi.com/docs/)

## Fast Facts

| Language(s)   | Language Type | File Type(s) | Synthesizes to?                         |
|--------------|-------------|------------------|----------------------|
| TypeScript, Python, Go, Java, C#, YAML | Object-oriented programming languages and YAML | `.ts`, `.py`, `.go`, `.java`, `.cs`, `.yaml` | Cloud provider specific APIs (e.g., AWS SDK for AWS) |

## Abstractions

- **Resources**: Cloud provider resources defined as objects in your chosen programming language
- **Stacks**: Independent instances of your infrastructure (e.g., dev, staging, prod)
- **Projects**: A collection of related stacks that share the same program
- **Components**: Reusable modules that encapsulate common patterns

## State Management

Pulumi maintains state in several places:

- **Backend**: State is stored in a backend (Pulumi Service, S3, Azure Blob, etc.)
- **Local State**: 
  - `Pulumi.yaml` defines your project
  - `Pulumi.<stack>.yaml` contains stack-specific configuration
  - `Pulumi.<stack>.json` contains stack state
  - `node_modules/` or equivalent for language dependencies

## Available Linters

- [Pulumi Policy Pack](https://www.pulumi.com/docs/guides/crossguard/aws-guard/)
- [Pulumi ESLint Plugin](https://www.pulumi.com/docs/guides/using-eslint/)
- [Pulumi TypeScript](https://www.pulumi.com/docs/guides/typescript/)

## Important Commands

- `pulumi new` - Create a new Pulumi project
- `pulumi up` - Deploy stack changes
- `pulumi preview` - Preview stack changes
- `pulumi destroy` - Destroy stack resources
- `pulumi stack` - Manage stacks
- `pulumi config` - Manage stack configuration
- `pulumi refresh` - Refresh stack state
- `pulumi import` - Import existing resources
- `pulumi graph` - Generate dependency graph

## Other Important Concepts

- [Pulumi Automation API](https://www.pulumi.com/docs/guides/automation-api/)
- [Pulumi Policy as Code](https://www.pulumi.com/docs/guides/crossguard/)
- [Pulumi Testing](https://www.pulumi.com/docs/guides/testing/)
- [Pulumi Secrets](https://www.pulumi.com/docs/guides/secrets/)
- [Pulumi CI/CD](https://www.pulumi.com/docs/guides/continuous-delivery/)

## Good Resources for Getting Started

- [Pulumi Tutorials](https://www.pulumi.com/docs/get-started/)

## Good Resources

- [Pulumi Best Practices](https://www.pulumi.com/docs/guides/best-practices/)
- [Pulumi Blog](https://www.pulumi.com/blog/)
- [Pulumi Community](https://www.pulumi.com/community/)
- [Pulumi GitHub](https://github.com/pulumi/pulumi)
- [Pulumi Registry](https://www.pulumi.com/registry/)
- [Pulumi Examples](https://github.com/pulumi/examples)
- [Serverless Land](https://serverlessland.com/patterns?framework=Pulumi)
