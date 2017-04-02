# Ansible Project/Playbook

This play book does the following:

  - Spins up three aws mirco instances in EU
  - Two instances have nginx install on them and started
  - One instance has HAProxy installed and started
  - The playbook updates the haproxy.cfg file to add in the nginx servers as backend nodes
  - The playbook enables haproxy to run.
  
## For ansbile version without vault please see [here](https://github.com/Steve-Walsh/ansible_project)

### Installation

Project requires 
  - [Ansible](https://www.ansible.com/) 
  - [Boto](https://github.com/boto/boto)

 
To run the play book
```sh
$ cd ansible_project
$ ansible-playbook -vvv provision-ec2.yml --ask-vault-pass
```

