# Home Infra
This repository automated the deployment of my homelab using ansible

# Ansible

Work in progress:

In order to run the setup:
1. Checkout the repository to your ansible host/build agents:
1. (Skip if using python 3.8.10 directly) Using virtualenv:

``` 
virtualenv py38env
source py38env/bin/activate
```

1. Install python/ansible dependencies:

```
pip install ansible
pip install paramiko
```

or

```
pip install -r requirements.txt
```

1. TODO: Update your group_vars: ansible_password & ansible_become_password (host admin password)
1. TODO: Update your hosts.ini: ip of 3 hosts
1. Create ansible vault password: .ansible_vault
1. Execute ansible command: 

```
ansible-playbook site.yml -i hosts.ini --vault-password-file .ansible_vault
```
