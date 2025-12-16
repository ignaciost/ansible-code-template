# Ansible Code Template

A template repository for developing Ansible code with best practices, issue templates, GitHub Actions workflows, and PR templates.

## Features

This template includes:

- 📋 **Issue Templates** - Standardized templates for bug reports, feature requests, and playbook issues
- 🔄 **Pull Request Template** - Comprehensive PR template with checklists for Ansible code changes
- 🚀 **GitHub Actions Workflows** - Automated CI/CD pipelines for:
  - Ansible Lint
  - YAML Lint
  - Ansible Syntax Checks
- ⚙️ **Configuration Files** - Pre-configured `.yamllint` and `.ansible-lint` settings

## Getting Started

### Using This Template

1. Click the "Use this template" button at the top of this repository
2. Create your new Ansible repository from this template
3. Clone your new repository
4. Start adding your Ansible playbooks, roles, and tasks

### Project Structure

```
.
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.md
│   │   ├── feature_request.md
│   │   ├── playbook_issue.md
│   │   └── config.yml
│   ├── workflows/
│   │   ├── ansible-lint.yml
│   │   ├── yaml-lint.yml
│   │   └── ansible-syntax-check.yml
│   └── pull_request_template.md
├── .ansible-lint
├── .yamllint
└── README.md
```

### Recommended Directory Structure for Your Ansible Project

Add the following directories to your project as needed:

```
├── playbooks/          # Your Ansible playbooks
├── roles/              # Ansible roles
├── inventory/          # Inventory files
│   ├── production/
│   └── staging/
├── group_vars/         # Group variables
├── host_vars/          # Host variables
├── tasks/              # Standalone tasks
├── handlers/           # Handlers
├── templates/          # Jinja2 templates
├── files/              # Static files
└── vars/               # Variable files
```

## GitHub Actions Workflows

### Ansible Lint

Runs `ansible-lint` on all Ansible files to ensure best practices and catch common issues.

- Triggers: Push and PR to `main` and `develop` branches
- Configuration: `.ansible-lint`

### YAML Lint

Validates YAML syntax and formatting across all YAML files.

- Triggers: Push and PR to `main` and `develop` branches
- Configuration: `.yamllint`

### Ansible Syntax Check

Performs syntax validation on Ansible playbooks.

- Triggers: Push and PR to `main` and `develop` branches

## Issue Templates

### Bug Report
Use this template to report bugs in your Ansible code, including environment details and error outputs.

### Feature Request
Suggest new features or improvements to the Ansible project.

### Playbook Issue
Report specific issues with playbooks or roles, including idempotency problems, task failures, or performance issues.

## Pull Request Template

The PR template includes sections for:
- Description of changes
- Type of change
- Ansible components modified
- Testing performed
- Checklist for code quality

## Customization

### Modifying Workflows

Edit the workflow files in `.github/workflows/` to customize:
- Trigger branches
- Python/Ansible versions
- Additional testing steps

### Adjusting Linter Rules

- **ansible-lint**: Edit `.ansible-lint` to skip or modify rules
- **yamllint**: Edit `.yamllint` to adjust YAML formatting rules

### Adding More Templates

Add additional issue templates in `.github/ISSUE_TEMPLATE/` following the existing format.

## Development

### Prerequisites

- Python 3.9+
- Ansible 2.9+
- ansible-lint
- yamllint

### Installation

```bash
# Install required Python packages
pip install ansible ansible-lint yamllint

# Or use a requirements file
pip install -r requirements.txt
```

### Local Testing

```bash
# Run ansible-lint
ansible-lint .

# Run yamllint
yamllint .

# Syntax check a playbook
ansible-playbook playbooks/your-playbook.yml --syntax-check

# Dry run a playbook
ansible-playbook playbooks/your-playbook.yml --check
```

## Contributing

1. Create a feature branch from `develop`
2. Make your changes
3. Ensure all tests pass locally
4. Submit a pull request using the PR template

## Resources

- [Ansible Documentation](https://docs.ansible.com/)
- [Ansible Best Practices](https://docs.ansible.com/ansible/latest/user_guide/playbooks_best_practices.html)
- [Ansible Lint Documentation](https://ansible-lint.readthedocs.io/)
- [YAML Lint Documentation](https://yamllint.readthedocs.io/)

## License

This template is provided as-is for use in your Ansible projects.
