# Observability-stack
This stack will setup the Node-Exporter, Prometheus and Grafana on centos system.
the main.yaml is located in parent folder of the repository.
This Observability stack is consist of 3 tasks.
1. Install
2. Uninstall
3. Upgrade

Below are the commands to perform tasks.

Install:
ansible-playbook main.yaml --tags install

Prerequsities
Make sure to write a required version and correct hostname in the vars file which located at:
roles/observability_stack/defaults.main.yml

Uninstall:
ansible-playbook main.yaml --tags uninstall

Upgrade:
ansible-playbook main.yaml --tags upgrade

Prerequsities
Make sure to write a updated/latest version in the vars file which located at:
roles/observability_stack/defaults.main.yml
