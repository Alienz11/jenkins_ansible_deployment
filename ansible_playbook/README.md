# Ansible Playbooks

These are the ansible playbooks stored on the ansible server, used to make deployments.

You can manually deploy these playbooks by using the following commands

`ansible-playbook <ansible-playbook-name>.yml`

`ansible-galaxy collection install community.kubernetes`

N.B: Before running the ansible-playbook command that deploys Prometheus, run

`ansible-galaxy install cloudalchemy.prometheus`
