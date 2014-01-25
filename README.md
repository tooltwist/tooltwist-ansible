
The scripts in this project are used to set up one or more servers for ToolTwist deployments.

The servers can be fired up and running in a few minutes, making them ideal for testing:

- Physical servers
- Virtual Box
- VMWare
- Amazon
- Other Cloud-based servers

To do this, we use several products:

* [Virtual Box](https://www.virtualbox.org) and [VMWare](https://www.vmware.com) are used to run virtual machines on your desktop machine.
* [Vagrant](http://www.vagrantup.com) is used to fire up and shutdown virtual machines, on VirtualBox, VMWare or Amazon AWS.
* [Ansible](http://www.ansible.com/home) is a tool used to install software and run configuration scripts on the servers.


If you have an existing server running, Ansible can be used to configure the machine. If you don't have an existing server, Vagrant can create the server(s) and then run Ansible for you.


### Links
[Vagrant documentation](http://docs.vagrantup.com/v2/)  
[Ansible documentation](http://docs.ansible.com/intro.html)  
[Installing Ansible on OSX](http://devopsu.com/guides/ansible-mac-osx.html)  
[Best Practices for Ansible](http://docs.ansible.com/playbooks_best_practices.html#how-to-arrange-inventory-stage-vs-production)  
