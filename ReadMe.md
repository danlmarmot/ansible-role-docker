An Ansible role for installing Docker and Docker Compose on Ubuntu 15.10.

### Default versions

These are set in /defaults directory
Ubuntu is set in the Vagrant file in the /test directory

Ubuntu 15.10
Docker 1.11.1
Docker Compose 1.7.1

Version 2.0 of Ansible is used.

### Testing

A Vagrant/VirtualBox environment is provided in the /test directory.

To get started:

1. Install Vagrant, Virtualbox, and Ansible.
1. Change your directory into templates folder
1. Run 'vagrant up' to bring up the VM.

### Additional notes

- For Vagrant installs, the install packages for are downloaded once and cached locally.
- To speed up re-provisioning, each role in this Ansible playbook will check the version of each application before installing, and will not re-install if the installed version is the desired version.
- To reprovision, use the 'vagrant provision' command.
