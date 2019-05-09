sql_exporter
============

Ansible role for install database agnostic SQL exporter for Prometheus.

Requirements
------------

Ansible.

Role Variables
--------------

All variables which can be overridden are stored in [defaults/main.yml](defaults/main.yml) file as well as in table below.

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| `sql_exporter_version` | 0.5 | sql_exporter package version. |
| `sql_exporter_web_listen_address` | "0.0.0.0:9399" | Address on which sql_exporter will listen |
| `sql_exporter_config_dir` | /etc/sql_exporter | |

Dependencies
------------

None.

Example Playbook
----------------

Use it in a playbook as follows:

```yaml
- hosts: all
  roles:
    - sql_exporter
```

Configuration notes
-------------------

Some helpful tips are in original sql_exporter [README.md](https://github.com/free/sql_exporter/blob/master/README.md):  
https://github.com/free/sql_exporter/blob/master/README.md

License
-------

BSD

Credits
-------

This role is inspired by https://github.com/cloudalchemy/ansible-mysqld-exporter  
This sql_exporter is created by: https://github.com/free/sql_exporter and this is only wrap-up in Ansible role.
