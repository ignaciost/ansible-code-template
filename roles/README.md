# Roles Directory

Place your Ansible roles here.

## Creating a New Role

```bash
ansible-galaxy init my_role
```

## Role Structure

```
roles/
└── my_role/
    ├── README.md
    ├── defaults/
    │   └── main.yml
    ├── files/
    ├── handlers/
    │   └── main.yml
    ├── meta/
    │   └── main.yml
    ├── tasks/
    │   └── main.yml
    ├── templates/
    ├── tests/
    │   ├── inventory
    │   └── test.yml
    └── vars/
        └── main.yml
```

## Best Practices

- Each role should have a single, well-defined purpose
- Document role variables in README.md
- Use `defaults/main.yml` for default values
- Use `vars/main.yml` for role-specific variables that shouldn't be overridden
- Test roles independently with molecule (optional)
