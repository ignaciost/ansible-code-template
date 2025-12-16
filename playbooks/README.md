# Playbooks Directory

Place your Ansible playbooks here.

## Example

```yaml
---
- name: Example playbook
  hosts: all
  become: yes
  
  tasks:
    - name: Ensure a package is installed
      ansible.builtin.package:
        name: vim
        state: present
```

## Best Practices

- Use descriptive names for playbooks (e.g., `webserver-setup.yml`, `database-backup.yml`)
- Include proper documentation at the top of each playbook
- Use roles for reusable components
- Keep playbooks focused on specific tasks or configurations
