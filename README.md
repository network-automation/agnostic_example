# Ansible Network Automation - Agnostic Examples
  This Github repository is for showcasing [cli_command](https://docs.ansible.com/ansible/latest/modules/cli_command_module.html) and [cli_config](https://docs.ansible.com/ansible/latest/modules/cli_config_module.html) agnostic network automation modules for the [network_cli connection plugin](https://docs.ansible.com/ansible/latest/plugins/connection/network_cli.html).

## Playbooks

 - [show_interfaces.yml](show_interfaces.yml) - this playbook issues `show ip interface brief` on Cisco IOS and Arista EOS, and `show interface terse` on Juniper Junos.  Then displays the output to the terminal window.
 - [backup.yml](backup.yml) - performs a backup of the running configuration on Arista EOS, Cisco IOS and Juniper Junos.

## Explanation of Additional Files

 - ansible.cfg - this is the [Ansible Configuration File](https://docs.ansible.com/ansible/latest/installation_guide/intro_configuration.html#configuration-file).  This is not required but points to my inventory, in this case a file called `hosts`
 - hosts - this is an INI formatted [inventory file](https://docs.ansible.com/ansible/latest/user_guide/intro_inventory.html).  This is to be used as an example.
 - group_vars - this is a directory that contains [variables separated by group](https://docs.ansible.com/ansible/latest/user_guide/playbooks_variables.html).  It is recommended to have a group per network platform type to store platform specific variables.

---
![Red Hat Ansible Automation](images/networkautomation.png)

- [Red Hat® Ansible® Network Automation](https://www.ansible.com/networking): automate networking devices from Arista (EOS), Cisco (IOS, IOS XR, NX-OS), Juniper (JunOS), Open vSwitch, and VyOS and many more! Includes [Ansible Tower](https://www.ansible.com/tower) curated content specifically for network use cases.
