# Install & Configure Raspberry pi via Ansible scripts

## Prerequisites

```sh
ansible-galaxy install -r requirements.yaml
```

## Deploy
```sh
ansible-playbook -i inventory.yaml site.yaml
```

**NOTE:** Tested with Ansible 2.10.12 and Python v3.8.10