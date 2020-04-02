Role Name
=========

This role has as objective the implementation of wireguard server on ubuntu

Requirements
------------

ubuntu 18.04

Role Variables
--------------

```yaml
interfaceaddress: '10.100.100.1/24'
internaladdress: '10.0.1.2/32'
clientaddress: '10.100.100.2/22, 10.0.1.2/32'
vpnclientadd: '10.100.100.2/32'
listenport: '5018'
dns: '1.1.1.1'
publicip: '116.202.109.53'
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
