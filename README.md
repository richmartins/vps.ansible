# VPS.ANSIBLE

setup for personal [ik](infomaniak.com) VPS

# Requirments

- [Ansible](https://www.ansible.com/)


# Usage

## Set ik IP to global host inventory `/etc/ansible/hosts`

## Create vault

    ansible-vault create vars/secret.yml

set ik_ssh_user and ik_ssh_key_path e.g.

    "ik_ssh_user": "my_user"
    "ik_ssh_key_path": "/path/to/key"

## Run

    ansible-playbook main.yml --ask-vault-pass