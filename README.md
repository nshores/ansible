#Ansible Playbooks


#Install Anisble:

sudo pip install --ignore-installed --ugprade ansible

#Example Commands:


**Run Commands against module**

ansible -i myhosts lab -m ios_command -a "commands="sh ver" host={{ inventory_hostname }} username=user password=password"

**Run commands raw against SSH hosts**

ansible -i myhosts lab -m raw -a "show cdp neighbor


**Example Inventory File**

[lab]
192.168.1.3
10.1.1.240
10.1.1.241
10.1.1.242
10.1.1.243
10.1.1.244
10.1.1.245 

[lab:vars]
ansible_user=ansible
ansible_password=ansible"
