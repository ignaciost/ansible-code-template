# Group Variables

Place variables that apply to groups of hosts here.

## Structure

```
group_vars/
├── all.yml          # Variables for all hosts
├── webservers.yml   # Variables for webservers group
└── databases.yml    # Variables for databases group
```

## Example (all.yml)

```yaml
---
# Common variables for all hosts
ntp_server: time.example.com
dns_servers:
  - 8.8.8.8
  - 8.8.4.4

# Package management
package_state: present
```

## Best Practices

- Use `all.yml` for variables common to all hosts
- Create group-specific files for targeted variables
- Use ansible-vault for sensitive data
- Document variable purposes with comments
