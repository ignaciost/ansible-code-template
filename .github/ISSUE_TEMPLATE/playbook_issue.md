---
name: Playbook Issue
about: Report an issue with an Ansible playbook or role
title: '[PLAYBOOK] '
labels: playbook, needs-triage
assignees: ''
---

## Playbook/Role Information
- **Name**: 
- **Version**: 
- **Path**: 

## Issue Type
- [ ] Task failure
- [ ] Idempotency issue
- [ ] Performance problem
- [ ] Variable/template issue
- [ ] Handler not triggering
- [ ] Other

## Environment
- **Ansible Version**: 
- **Control Node OS**: 
- **Target Node OS**: 
- **Connection Type**: [ssh/winrm/local/docker]

## Issue Description
Describe the issue you're experiencing with the playbook or role.

## Playbook Excerpt
```yaml
# Paste the relevant portion of your playbook here
```

## Command Used
```bash
# The ansible-playbook command you ran
ansible-playbook ...
```

## Output/Error
```
# Paste the output or error message
```

## Expected Result
What should have happened?

## Actual Result
What actually happened?

## Additional Information
- Have you tried running with `-vvv` for verbose output?
- Any custom modules or plugins involved?
- Relevant inventory details?
