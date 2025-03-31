# Ansible

Automate infrastructure provisioning, configuration management, and application deployment using a simple, human-readable language.

[Ansible Docs](https://docs.ansible.com/)

## Fast Facts

| Language(s)   | Language Type | File Type(s) | Synthesizes to?                         |
|--------------|-------------|------------------|----------------------|
| YAML, Jinja2 | Declarative language and templating | `.yml`, `.yaml`, `.j2` | SSH commands and API calls |

## Abstractions

- **Playbooks**: YAML files that define automation tasks and workflows
- **Roles**: Reusable collections of tasks, variables, and templates
- **Tasks**: Individual units of work to be executed
- **Variables**: Dynamic values that can be used in playbooks
- **Templates**: Jinja2 templates for generating configuration files
- **Inventory**: Lists of hosts and groups to manage
- **Modules**: Reusable units of code that execute specific tasks
- **Collections**: Distribution format for Ansible content

## State Management

Ansible maintains state in several places:

- **Target Systems**: The actual state of managed systems
- **Local State**: 
  - `ansible.cfg` - Ansible configuration file
  - `inventory` files - Host and group definitions
  - `group_vars/` and `host_vars/` - Variable definitions
  - `roles/` - Role definitions
  - `playbooks/` - Playbook definitions

## Available Linters

- [ansible-lint](https://github.com/ansible-community/ansible-lint)
- [yamllint](https://github.com/adrienverge/yamllint)
- [ansible-review](https://github.com/willhallonline/ansible-review)
- [molecule](https://github.com/ansible-community/molecule) for testing

## Important Commands

- `ansible-playbook` - Run playbooks
- `ansible-galaxy` - Manage collections and roles
- `ansible-vault` - Encrypt sensitive data
- `ansible-inventory` - Display inventory information
- `ansible-doc` - Display documentation
- `ansible-pull` - Pull playbooks from VCS
- `ansible-config` - View/edit Ansible configuration
- `ansible-console` - Interactive REPL
- `ansible-test` - Test collections and roles

## Other Important Concepts

- [Ansible Roles](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_reuse_roles.html)
- [Ansible Collections](https://docs.ansible.com/ansible/latest/collections_guide/collections.html)
- [Ansible Variables](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_variables.html)
- [Ansible Templates](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_templating.html)
- [Ansible Facts](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_vars_facts.html)
- [Ansible Tags](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_tags.html)
- [Ansible Handlers](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_handlers.html)
- [Ansible Conditionals](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_conditionals.html)

## Good Resources for Getting Started

- [Ansible Getting Started Guide](https://docs.ansible.com/ansible/latest/getting_started/index.html)
- [Ansible Examples](https://github.com/ansible/ansible-examples)
- [Ansible Workshop](https://ansible.github.io/workshops/)

## Good Resources

- [Ansible Best Practices](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_best_practices.html)
- [Ansible Galaxy](https://galaxy.ansible.com/)
- [Ansible Blog](https://www.ansible.com/blog)
- [Ansible GitHub](https://github.com/ansible)
- [Ansible Community](https://ansible.com/community)
- [Ansible Security](https://docs.ansible.com/ansible/latest/security.html)