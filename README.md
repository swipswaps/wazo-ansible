# wazo-ansible

## Prerequisites for all recipes

* Enough machines running with Debian Stretch vanilla
* You can SSH easily into those machines (i.e. without password prompt)
* Ansible: `pip install ansible`


## UC Engine (all in one machine)

* Edit `inventories/uc-engine` and set your host in `[uc-engine-host]`
* Run:

```shell
ansible-galaxy install -r requirements-postgresql.yml

ansible-playbook -i inventories/uc-engine uc-engine.yml
```
