# Nagios with Ansible

Role for installing and configuring Nagios.

## Optional Parameters

 * `nagios_core_version` - Version of release from github
 * `nagios_core_sha256` - Checksum of tar.gz for release
 * `nagios_plugins_version` - Version of release from github
 * `nagios_plugins_sha256` - Checksum of tar.gz for release
 * `nagios_admin_password` - Password for admin user

## Testing

Credit: Tested with vagrant image from [@geerlingguy's Ansible for Devops](https://github.com/geerlingguy/ansible-for-devops)

Run the following from the test directory:

### Initial Install
```
ansible-galaxy install -r requirements.yml
vagrant up
```

### Reapply provisioning
```
vagrant provision
```

## TODO

 * Make idempotent  
 * Install starter objects
 * Replace UI admin user with read only user
