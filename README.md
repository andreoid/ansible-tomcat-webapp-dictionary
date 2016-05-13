# Ansible Customer Dictionary example

Examples of how to set up a dictionary of customer data which can then be used to deploy variants of web applications (e.g. different web apps into Tomcat)

### Version
0.0.1

### Installation
Requires Ansible 2.0+ as we're combining dictionaries

### Execution
Deploy all customers
```sh
$ ansible-playbook -i environments/all_customers/inventory.ini webapps.yml -c local
```
Deploy a single customer
```sh
ansible-playbook -i environments/just_apple/inventory.ini webapps.yml -c local
```