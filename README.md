![Ansible Lint](https://github.com/johanneskastl/ansible-role-create_krb5_conf/workflows/Ansible%20Lint/badge.svg)

create_krb5_conf
=========

Create a krb5.conf file

Requirements
------------

None.

Role Variables
--------------

- `kerberos_realm`: The realm to be used for kerberos.
- `dns_lookup_realm`: (Default: false) Indicate whether DNS TXT records should be used to determine the Kerberos realm of a host.
- `dns_lookup_kdc`: (Default: true) Indicate whether DNS SRV records should be used to locate the KDCs and other servers for a realm.

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: 'johanneskastl.create_krb5_conf' }

License
-------

BSD-3-Clause

Author Information
------------------

I am Johannes Kastl, reachable via kastl@b1-systems.de.
