backup-reporter
=========

This role installs and configures the backup-reporter.

Requirements
------------

Ansible 2.17+

Role Variables
--------------

You can see all vars in `defaults/main.yml` vars file.

Dependencies
------------

- python3 - for host installation
- docker - for docker container installation

Example Playbook
----------------

```yaml
- name: Ensure backup-reporter
  hosts: backup_reporters, backup_collectors
  remote_user: root

  roles:
    - backup-reporter
```

License
-------

Apache 2.0

Author Information
------------------

This role was created by [Sergey Evseev](https://github.com/Ageres210784).
