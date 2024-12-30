
## [Ansible Getting started]( https://docs.ansible.com/ansible/latest/getting_started_ee/index.html) 

# youtube links
[1. Ansible UI](https://www.youtube.com/watch?v=NyOSoLn5T5U)    
[2. Automate everything with Ansible ! Ansible for beginners](https://www.youtube.com/watch?v=w9eCU4bGgjQ)

# Ansible
# Parameters: 

    web         ansible_host = myserver1.test.com
    api         ansible_host = myserver2.test.com
    cache       ansible_host = myserver3.test.com
    db          ansible_host = myserver4.test.com

# localhost 
    
    ansible_connection = localhost

# Parameters:

    Ansible_connection: ssh/winrm/localhost
    Ansible_port: 22/8080
    Amsible_user: root/admin
    Ansible_ssh_pass: Password

# install Ansible 
1. macbook: run followin cmds in terminal
   1. brew update 
   2. brew install ansible
   3. ansible --version # to check the ansibel version
2. Linux: 
   1. 


# syntax to execute playbook execute

syntex:
    ansible-playbook <playbook name> -i <inventory file>
    ansible-playboot httpd.yml - i inventory.txt

# Ansible Modules

Ansible covered varioues number of modules in documentation
modules are reusable, standalone scripts that can be used by the Ansible API, or by the ansible or ansible playbook

1. Cloud
2. Clustering
3. Command
4. File
5. Database
6. System
7. Windowns
8. Monitoring

