# Domjudge Ansible

## Install Ansible

### Optional (1): Use poetry

```shell 
$ poetry install

$ poetry shell

(venv)$ ansible --version
```

### Optional (2):

[Ansible Installation Guide](https://docs.ansible.com/ansible/latest/installation_guide/index.html)

## Install Ansible community general modules

```shell
$ ansible-galaxy collection install community.general

$ ansible-galaxy collection install community.docker
```

```shell
$ ANSIBLE_CONFIG=./ansible.cfg ansible-playbook -i inventory/hosts.yaml playbook/site.yaml --ask-become-pass

$ ANSIBLE_CONFIG=./ansible.cfg ansible-playbook -i inventory/standalone.yaml playbook/site.yaml --ask-become-pass
```