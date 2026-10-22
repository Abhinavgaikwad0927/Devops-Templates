
# Ansible Server Automation

## Overview.
Reusable Ansible project for Linux server configuration.

## Features
- Common package installation
- Nginx installation and service management
- Inventory-based server management
- Reusable Ansible roles
- Development and production inventory separation

## Prerequisites
- Ansible
- SSH access to target Linux servers
- Appropriate privilege escalation permissions

## Validate
ansible-inventory -i inventory/dev.ini --list
ansible-playbook --syntax-check playbooks/site.yml

## Execute
ansible-playbook playbooks/site.yml --limit webservers
