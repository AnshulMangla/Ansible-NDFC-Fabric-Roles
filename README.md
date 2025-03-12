# Ansible-NDFC-Fabric-Roles

# Pre-requisites

## Install Ansible Roles

 - Download the respective Ansible roles from the repository above and copy the respective role directory under the "roles" folder
 - https://github.com/CiscoDevNet/ansible-dcnm

## Update the Host details
 - Update the ndfc hostname or ip-address in inventory > hosts > hosts file
     ```sh
     aansible_host: 10.106.236.47
     ```

## Update the Log-in Credentials

 - Update the ndfc log-in credentials and the log-in domain  in inventory > group_vars > ndfc > 00_connections.yml file
     ```sh
     ansible_httpapi_login_domain: domain (local/AD)
     ansible_user: user-name
     ansible_password: password
     ``` 


## Executing a Ansible Playbook
 - Once the Ansible Roles have been copied to the "roles" folder above, the Ansible Playbook can be executed as below
   
 - Open **Command Prompt (cmd)** and type:
     ```sh
     ansible-playbook <playbook_name>.yml -i inventory
     ```
