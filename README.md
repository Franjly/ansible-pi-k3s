# ansible-pi-k3s
Ansible playbooks for common provisioning tasks on clusters

## Requirements
1. Python 3
1. Ansible

## Usage
```bash
$ ansible-playbook -i inventory_change_default_user.yml 0_change-default-user.yml
$ ansible-playbook -i inventory.yml 1_base-config.yml
$ ansible-playbook -i inventory.yml 2_k3s-install.yml
```