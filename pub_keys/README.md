Role Name
=========

This role has as objective manage key rotation

Requirements
------------

ubuntu 18.04

Role Variables
--------------

```yaml
# add the user here
user_ssh: root

keys:
    - "https://gitlab.com/orlando43.keys"
    - "https://gitlab.com/user2.keys"
    - "https://gitlab.com/user3.keys"
```

Dependencies
------------

ssh keys or url to the hosted pub keys

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables
passed in as parameters) is always nice for users too:

```yaml
    - hosts: servers
      roles:
         - { role: base, x: 42 }
```

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a
website (HTML is not allowed).
