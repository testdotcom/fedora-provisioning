# Fedora Provisioning

Ansible playbook for provisioning a Fedora machine. The default target is the local machine (`ansible_connection: local`).

## Requirements

- Ansible (`ansible-core`) on the controller
- Passwordless sudo, or run the playbook with `--ask-become-pass`

## Usage

```bash
ansible-playbook main.yml --check --diff   # dry run
ansible-playbook main.yml                  # apply everything
ansible-playbook main.yml --tags zsh       # only the zsh role
```
