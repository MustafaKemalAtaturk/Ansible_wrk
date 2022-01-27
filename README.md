# Ansible_wrk
This repo contains 2 playbooks
# - playbook_usr.yml

  This playbook runs the following roles and tasks related to these roles. 
  
  # - role: add-account 
    # add-account perform these tasks:
      Creates a user group named optuser
      Creates a user named jamie
      Adds an ssh key file to the authorized key for user jamie
      
  # - role: createfolder
    # createfolder perform these tasks:
      Creates 2 folders named folder1 and folder2 under the opt directory
      Makes jamie user owner for created folders and only gives read and write permissions to jamie user.
      
  # - role: ngnix_install
    # ngnix_install perform these tasks:
      It installs nginx and configrets 
      Adds a index.html file 
      Retarts nginx
      
# - playbook_tcp_fw.yml

  This playbook runs the following roles and tasks related to these roles. 
  
  # - role: systemctl
    # systemctl perform these tasks:
      Interferes with systemctl using the ansible.posix.sysctl plugin. The aim is to perform the following task.
      
                        [Updates the kernel parameter which enables TCP Forwarding]

      
