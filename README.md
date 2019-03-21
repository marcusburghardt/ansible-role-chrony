Role Name
=========

This role will:
- Ensure the presence of Chrony service.
- Ensure the presence of a valid configuration file.
- Ensure the service is started and enabled.
- Ensure the NTP service is stopped and masked.

The role was wrote to attend a common demand in infrastructures.

Admins:
- You just need to adjust the defailt/main.yml file if want some custom NTP servers.

Requirements
------------

Just a working repository.

Role Variables
--------------

In the defaults/main.yml and vars/<os_family>.yml there are some interesting variables to undestand better this role.

Dependencies
------------

None

Example Playbook
----------------

1) Install and use the default settings.

```

- hosts: linux-servers
  roles:
    - role: ansible-role-chrony
```

License
-------

MIT

Author Information
------------------

Marcus Burghardt - marcus.apb@gmail.com
@MBSEC - marcus@mbsec.com.br
https://mbsec.com.br

