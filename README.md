#Ansible Playbooks


#Install Anisble:

sudo pip install --ignore-installed --ugprade ansible

#Example Commands:


#Run Commands against module

ansible -i myhosts lab -m ios_command -a "commands="sh ver" host={{ inventory_hostname }} username=user password=password"

#Run commands raw against SSH hosts

ansible -i myhosts lab -m raw -a "show cdp neighbor"
