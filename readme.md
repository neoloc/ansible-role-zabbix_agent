zabbix_agent Role
=========

A brief description of the role goes here.

[![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-neoloc.zabbix_agent-blue.svg)](https://galaxy.ansible.com/neoloc/ansible-role-zabbix_agent/)


Requirements
------------

None

Role Variables
--------------

```yaml
zabbix_agent_configure: true
zabbix_agent_server_address: zabbix-server
zabbix_agent_listen_port: 10050
zabbix_agent_server_active_address: zabbix-server
# Not mandatory, but possible to overwrite.
# zabbix_agent_source_ip: "127.0.0.1"

zabbix_agent_hostname: "{{ ansible_fqdn }}"
zabbix_agent_hostmetadata: system.uname
zabbix_agent_timeout: 3

# Enable logging of remote commands by setting this value to 1.
zabbix_agent_logremotecommands: "1"
```

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      roles:
         - neoloc.zabbix_agent

License
-------

See license.md

Author Information
------------------

[![Github](https://img.shields.io/badge/Github-neoloc-blue.svg)](https://github.com/neoloc)
