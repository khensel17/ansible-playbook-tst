# ansible-playbook-tst

## Playbooks

| Name               | Description                                                   |
|--------------------|---------------------------------------------------------------|
| test | test description. |

## Roles and Collections

This project depends on other Ansible Roles and Collections. These roles and collections are gathered by ansible-galaxy with the ``requirements.yml`` file.

In this file you can find the dependencies and versions.

## Test

To test the above playbooks locally see the following steps.

### Install dependencies

```bash
python3 -m venv .venv
source .venv/bin/activate
python3 -m pip install -r requirements.txt

ansible-galaxy role install -r ./requirements.yml -p ./playbooks/roles --force
ansible-galaxy collection install -r ./requirements.yml -p ./playbooks/collections --force
```
