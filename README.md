# Ansible playbook for Scrapy on CentOS 7

This is an Ansible playbook to setup Scrapy on CentOS 7.

For more information about the Vagrant machines see [vagrant-scrapy](https://github.com/tovletoglou/vagrant-scrapy).

## Requirements

Tested CentOS 7

## Get started

Clone this project

```
git clone https://github.com/tovletoglou/ansible-playbook-scrapy.git
```

Run the playbook `playbook_ansible.yml`. This one will get all the roles and put them in `roles/` sub-directory (roles are not uploaded to ansible galaxy yet).

```
ansible-playbook -i hosts playbook_ansible.yml
```

Run the actual playbook `playbook_scrapy.yml` in order to provision the server.

```
ansible-playbook -i hosts playbook_scrapy.yml
```

## Developer information

The sub-directories in the `callback_plugins` directory are git projects integrated with the [git-subrepo](https://github.com/ingydotnet/git-subrepo). You can recognize them by the `.gitrepo` file.

Do not commit changes of the sub-projects on the main project.
