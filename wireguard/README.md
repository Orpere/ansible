Role Name
=========

This role has as objective the implementation of wireguard server on ubuntu

Requirements
------------

ubuntu 18.04

Role Variables
--------------

```yaml
interfaceaddress: '10.100.100.1/24' # range filtered by the vpn
allowedips_server: '10.100.100.2/32' # IP authorized to access
```

Dependencies
------------

ppa:wireguard/wireguard

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables
passed in as parameters) is always nice for users too:

```yaml
    - hosts: servers
      roles:
         - { role: wireguard, x: 42 }
```

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a
website (HTML is not allowed).
