Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should
be mentioned here. For instance, if the role uses the EC2 module, it may be a
good idea to mention in this section that the boto package is required.

Role Variables
--------------

STORAGE: '/mnt/storage'
samba_group: 'security'
samba_user: 'test'
samba_password: '4zUVkmXnHfZ6xmvU2aQDcn' # this is just a test password
BUCKET: "test-backup-orp01"
REGION: "eu-central-1"
S3URL: 'https://s3-eu-central-1.amazonaws.com'

Dependencies
------------
aws credentials with s3 access
```bash
export s3_access_key="xxxxx"
export s3_secret_key="xxxxx"
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables
passed in as parameters) is always nice for users too:

```yaml
    - hosts: servers
      roles:
         - { role: sambaS3, x: 42 }
```

License
-------

BSD

Author Information
------------------

[Orlando Rosa Pereira](https://github.com/Orpere)
