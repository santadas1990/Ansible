# Ansible Playbooks

This repository contains Ansible playbooks and roles for infrastructure automation.

## Directory Structure

```
.
├── ansible.cfg          # Ansible configuration file
├── inventory.ini        # Inventory file with host definitions
├── simple_playbook.yml  # Example playbook
├── group_vars/          # Group variables
├── host_vars/           # Host-specific variables
├── roles/               # Ansible roles
└── README.md            # This file
```

## Getting Started

### Prerequisites

- Ansible 2.9+ installed
- SSH access to target hosts
- Python installed on target hosts

### Configuration

1. Edit `inventory.ini` to add your target hosts
2. Update `group_vars/all.yml` with global variables
3. Modify playbooks as needed

### Running Playbooks

```bash
# Run the example playbook
ansible-playbook simple_playbook.yml

# Run playbook on specific hosts
ansible-playbook simple_playbook.yml -l webservers

# Run with extra verbosity
ansible-playbook simple_playbook.yml -vv
```

## Roles

Add your reusable roles in the `roles/` directory.

## Documentation

For more information, visit [Ansible Documentation](https://docs.ansible.com/)
