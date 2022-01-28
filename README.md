<h1>Ansible_wrk</h1>
<strong>First of all, an ip address entry for ansible_host must be provided in the inventory file.</strong>

This repository contains 2 playbooks and the roles associated with these playbooks

<ul>
  <li>playbook_usr.yml</li>
  <li>playbook_tcp_fw.yml</li>
  </ul>

<h2>playbook_usr.yml</h2>
  
  This playbook runs the following roles and tasks related to these roles. 
  
<h2>Roles:</h2> 
<h3>add-account</h3>
<strong>perform these tasks:</strong>

<ul>
  <li>Creates a user group named "optuser"</li>
  <li>Creates a user named jamie</li>
  <li>Adds an ssh key file to the authorized key for user "jamie"</li>
</ul>

<h3>createfolder</h3>
<strong>perform these tasks:</strong>

<ul>
  <li>Createfolder perform these tasks:</li>
  <li>Creates 2 folders named folder1 and folder2 under the opt directory</li>
  <li>Makes jamie user owner for created folders and only gives read and write permissions to jamie user.</li>
  </ul>
  
<h3>ngnix_install</h3>
<strong>perform these tasks:</strong>      
<ul>
  <li>It installs nginx and configrets</li>
  <li>Adds a index.html file</li>
  <li>Retarts nginx</li>
  </ul>

<h2>playbook_tcp_fw.yml</h2>

  This playbook runs the following roles and tasks related to these roles. 
  
<h3>systemctl</h3>
<strong>perform these tasks:</strong> 
Interferes with systemctl using the ansible.posix.sysctl plugin. The aim is to perform the following task.
      
<ul>
  <li>Updates the kernel parameter which enables TCP Forwarding</li>
  </ul>

      
