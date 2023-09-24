# CS320Week4Lab


This project is for CS320. This is for the Week 4 Lab. Used an ansible playbook to run commands on a remote server.

## Project Requirements
* Install Software
  * Google Chrome
  * Firefox
  * Git
  * Apache 2 (httpd)
  * MariaDB Server
* Task 2 copy files
  * Create a directory on the loacl machine containing 3 sample HTML files.
  * Add a task to the playbook to copy these files from the local machine to /var/www/html on the remote system
* Remove Software
  * Add a task in the playbook to remove google chrome from the remote system
* System restart
    * Add a task in the playbook to restart the remote system after the removal of googl chrome
* System Demon Enablement
    * Add a task to the playbook that enable the HTTPD at startup
    * Add a task to the playbook to restart the HTTPD daemon
 
The playbook will be in the repository. All software was installed utilizing ansible.builtin.dnf for the remote system except for Google Chrome. For Google Chrome the package had to be added utilizing anisible.builting.get_url. I then had to use ansible.builtin.command to install the package. 
