

# what is playbook

1. playbooks are one of the core features of ansible
2. playbooks push configuration ansible what to execute
3. its list of todo actions for ansible
4. playbook contains a list of tasks
5. plabook contains the steps which the user wants to execute on a particular machine
6. palybooks are run sequentially
7. all playbooks are written in yml format
8. playbook define set of plays with activities to run on hosts
9. a task is single action perfomr on a hosts
    
## Example:

    name: Play1
    hosts: local host
    tasks:
        - name: "checking date"
            command: date 
        - name: "installing httpd"
            yum:
                name: httpd
                state: present  
        - name: "start httpd server"
            service:
                name: httpd
                state: started


## how to provide multiple playbooks

use the " - " as below for different play books executions or as splits 


    -
        name: Play1
        hosts: local host
        tasks:
          - name: "checking date"
              command: date 
    -  
        name: Play2
        hosts: local hosts
        tasks:

           - name: "installing httpd"
             yum:
                    name: httpd
                    state: present  
           - name: "start httpd server"
                service:
                    name: httpd
                    state: started