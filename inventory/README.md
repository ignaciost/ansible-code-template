# Inventory Directory

Place your inventory files here, organized by environment.

## Structure

```
inventory/
├── production/
│   ├── hosts.yml
│   └── group_vars/
│       └── all.yml
└── staging/
    ├── hosts.yml
    └── group_vars/
        └── all.yml
```

## Example Inventory (hosts.yml)

```yaml
---
all:
  children:
    webservers:
      hosts:
        web1.example.com:
          ansible_host: 192.168.1.10
        web2.example.com:
          ansible_host: 192.168.1.11
    databases:
      hosts:
        db1.example.com:
          ansible_host: 192.168.1.20
```

## Best Practices

- Separate inventories by environment (production, staging, development)
- Use descriptive group names
- Store sensitive data in ansible-vault encrypted files
- Use dynamic inventories for cloud environments when possible
