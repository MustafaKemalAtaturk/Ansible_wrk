# Ansible_wrk
<strong>First of all, an ip address entry for ansible_host must be provided in the inventory file.</strong>

This repo contains 2 playbooks
<ul>
  <li>playbook_usr.yml</li>
  <li>playbook_tcp_fw.yml</li>
  </ul>

  This playbook runs the following roles and tasks related to these roles. 
  
<h2>Roles:</h2> 
<h3>add-account</h3>
perform these tasks:
<ul>
  <li>Creates a user group named "optuser"</li>
  <li>Creates a user named jamie</li>
  <li>Adds an ssh key file to the authorized key for user "jamie"</li>
  </lu><br

<h3>createfolder</h3>
<ul>
  <li>Createfolder perform these tasks:</li>
  <li>Creates 2 folders named folder1 and folder2 under the opt directory</li>
  <li>Makes jamie user owner for created folders and only gives read and write permissions to jamie user.</li>
  </lu>
  
      
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

      
