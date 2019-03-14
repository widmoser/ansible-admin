Digital Ocean Basic Setup
=========

This role sets up a vanilla digital ocean instance so that the server is secured.

Requirements
------------

None.

Role Variables
--------------

```yaml
admin_group: example
admin_users:
  - username: jdoe
    password: <some encrypted password>
    ssh_key: <public ssh key>
  - username: jane
    password: <some encrypted password>
    ssh_key: <public ssh key>
repository_name: jdoe/great-app

firewall_allowed_tcp_ports:
  - "22"
  - "80"
  - "443"
```

Dependencies
------------

None.

Example Playbook
----------------

License
-------

MIT
