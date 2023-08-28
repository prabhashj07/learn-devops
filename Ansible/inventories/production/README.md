# Production Inventory

This directory contains the inventory information for the production environment. It includes the following files and directories:

- `hosts`: This file defines the inventory of hosts and groups for the production environment.
- `group_vars/`: This directory contains YAML files with group-specific variables used in playbooks and roles targeting the production environment.

Modify the `hosts` file to include your production server information and organize hosts into groups. You can also define group-specific variables in the `group_vars/` directory to customize behavior for different host groups.

For example playbooks and roles, refer to this inventory using the `-i` flag:

```bash
ansible-playbook -i inventories/production/hosts playbook.yml
