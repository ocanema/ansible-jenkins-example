# Jenkins installation with Ansible

Installs:
- Java OpenJdk 8
- Latest Stable Jenkins version with default plugins
- Latest Maven 

## Working on:

- CentOS 7 


### Running on amazon

Copy the amazon key file named to `key.pem` to the `key_files` directory.

Add the amazon hosts on `inventory.yaml` file

Set `amazon` group on `site.yml` hosts.

Run the playbook:
```
ansible-playbook -i inventory.yaml site.yml
```

Amazon hosts general configuration is on `group_vars/amazon.yml` 