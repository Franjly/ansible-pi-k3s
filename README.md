# ansible-pi-k3s
Ansible playbooks for common provisioning tasks on clusters

## Requirements
1. Python3
2. pip3 -> apt install python3-pip
3. Ansible -> pip3 install ansible --user && export PATH=$PATH:~/.local/bin
4. pip3 install openshift pyyaml kubernetes --user
5. ansible-galaxy collection install kubernetes.core

## Usage
```bash
$ ansible-playbook -i inventory_change_default_user.yml 0_change-default-user.yml
$ ansible-playbook -i inventory.yml 1_base-config.yml
$ ansible-playbook -i inventory.yml 2_k3s-install.yml --ask-become-pass
```