# Kubernetes Setup Ansible

Update the `inventory.ini` according to your server details. Run the following ansible scripts
```
ansible-playbook -i inventory.ini install.yaml
ansible-playbook -i inventory.ini etcd.yaml
ansible-playbook -i inventory.ini create_master.yaml
ansible-playbook -i inventory.ini join_master.yaml
ansible-playbook -i inventory.ini join_worker.yaml
ansible-playbook -i inventory.ini cillium.yaml
ansible-playbook -i inventory.ini longhorn.yaml
```