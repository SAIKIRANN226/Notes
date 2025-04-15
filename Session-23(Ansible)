Ansible.cfg --> It is a configuration file we can control everything from here, if we enter this command 
in the server terminal "ansible --version" we can see from where the configuration file is loading, we have preferences below. Gothrough ansible.conf in VS.
1. ANSIBLE_CONFIG (environment variable if set)
2. ansible.cfg (in the current directory)
3. ~/.ansible.cfg (in the home directory)
4. /etc/ansible/ansible.cfg

Templates is a jinja2 format, it is like ansible variable you can submit variable in catalogue.service 
file moved to the template and given {{MONGODB_HOST}}, so now this has become template, it is same as 
copy module

Handlers, for example if a configuration file is changed then we need to restart the nginx,
but what handlers will do is sometimes you want a task to run only when any changes are done in the machine(config_file), for example you may want to restart a service if a task updates the configuration
of that service, but not if the configuration is unchanged, for this we use "notify", why we use this
handlers because some servers will take 2-3 min other servers like nginx will restart in seconds

Tags.yaml is to run a tag ---> ansible-playbook -t devops 16.tags.yaml ---> dint not given hosts because 
it will test from the local host, if you dint mention the tags in the command it will run all tags, so 
where this tags are useful ? for example a new version is going to release for catalogue, so for that we
need to deploy new version, for that we need to stop the service/remove old code/download latest code/
and then restart, here we no need to run all the catalogue script, so create a deployment.yaml file in 
common in tasks folder. Usage: "ansible-playbook -e component=catalogue -t deployment main.yaml"

Points to remember
*******************
1. After all successful components deployments but still you may get erros like categories are not 
   displaying so in this case first "sudo less /var/log/messages" in this session catalogue is unable 
   to connect mongodb so do this "cat /etc/systemd/system/catalogue.service"
