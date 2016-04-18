# ansible-harstorage
Install harstorage with ansible playbook

# assumptions
mongo role is available

# TODOs
add supervisor changes to support harstorage
add virtualenv to install python packages

# to run the play use playbook like

- name: Deploy Harstorage
  hosts: all
  sudo: True
  gather_facts: True
  roles:
    - mongo
    - harstorage
