Role Name
=========
This role has the main target the installation of samba share to connect a s3 bucket s drive.

Requirements
------------

- Ubuntu instance
- A aws account with s3 access and one s3 bucket

Role Variables
--------------

STORAGE: '/mnt/storage'
samba_group: 'security'
samba_user: 'test'
samba_password: 'xxxxxxxxxx' # this is just a test password
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
