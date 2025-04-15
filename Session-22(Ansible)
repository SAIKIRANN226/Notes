To run the file or program in the background
---------------------------------------------
"nohup ansible-playbook -i inventory.ini -e ansible_user=centos -e ansible_password=DevOps321 <file-name> 
with .yaml & >> /dev/null" ---> output will be in nohup.out it will not come in the terminal, if it is a 
small instance we cant everything in background because memory consumption will be high, so you can run 
few scripts. Usage: nohup ansible-playbook -i inventory.ini -e ansible_user=centos -e ansible_password=De
vOps321 mongodb.yaml & >> /dev/null

Ansible roles
--------------
https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_reuse_roles.html
It is a dry principle, dont repeat a proper directory structure to keep our configuration and we can 
share this with other users ---> refer in VS, shipping.service,mongodb.repo,user.service etc. 
we call these as supporting files. So to run the main.yaml in the server "ansible-playbook -i inventory.ini 
-e ansible_user=centos -e ansible_password=DevOps321 -e component=mongodb main.yaml"

How to debug if you are facing any error
-----------------------------------------
"ansible-playbook -vvv -i inventory.ini -e ansible_user=centos -e ansible_password=DevOps321 -e component=mongodb main.yaml" we will get the full information in the terminal which is happening
in the background so that we can see where is the error

Points to remember
*******************
1. To see the background running "tail -f nohup.out"
2. To set the indentation in VS use shift+tab
