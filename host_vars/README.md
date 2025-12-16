# Host Variables

Place variables specific to individual hosts here.

## Structure

```
host_vars/
├── web1.example.com.yml
├── web2.example.com.yml
└── db1.example.com.yml
```

## Example (web1.example.com.yml)

```yaml
---
# Host-specific variables for web1.example.com
server_role: primary
backup_enabled: true
max_connections: 1000
```

## Best Practices

- Use host variables sparingly - prefer group variables when possible
- Name files after the inventory hostname
- Use ansible-vault for host-specific secrets
- Keep host variables organized and well-documented
