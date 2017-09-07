# Playbooks
once the cloudformation template for Ansible install and setup is deployed. Download this repository for run the playbooks for enabling services to the VMs.
Follow the below steps to run the playbook
cd /etc/ansible/
sudo git init
sudo git clone https://github.com/DXC-DevOps/Playbooks.git


example to run a playbook for linux machines
sudo ansilbe-playbook -i /etc/ansible/inventories.ec2.py /etc/ansible/Playbooks/linux.yml --user=root --ask-pass

example to run a playbook for windows machines
sudo ansilbe-playbook -i /etc/ansible/hosts /etc/ansible/Playbooks/windows.yml --user=root --ask-pass

Note: For windows machines, add the VM's IPs in the /etc/ansible/hosts file for the ansible to identify the target machine.
