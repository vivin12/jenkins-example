### Ansible Playbook example 

#### Manually running the playbook 

1. Change to the directory containing the ansible playbook. 

2. Run the following command to check before running the playbook ```ansible-playbook -i hosts simple-devops-image.yml --check``` 

3. To run the playbook ```ansible-playbook -i hosts simple-devops-image.yml```

### Ansible on Jenkins 

1. Got to manage Jenkins -> configure system -> configure over ssh. This is to enable jenkins to ssh into ansible system. Provide the ip, username and password of Ansible system. 

2. Once you have integrated Ansible server on Jenkins you will see an option in post build actions to send files over ssh. You can drop your war file to ansible server and in exec command section you can provide ansible run command ```ansible-playbook -i hosts simple-devops-image.yml```. 
  
