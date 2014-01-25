## Fast Configuration of ToolTwist servers

The scripts in this project are used to set up one or more servers for ToolTwist deployments. Various types of servers can be fired up and running in a few minutes, making them ideal for testing.

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


## Creating a server on Virtualbox
If you already have _Virtual Box_, _Vagrant_ and _Ansible_ installed on your machine, the following commands will create a Virtual Machine ready to run ToolTwist servers.

    $ git clone https://github.com/tooltwist/tooltwist-ansible.git
    Cloning into 'tooltwist-ansible'...
    remote: Counting objects: 49, done.
    remote: Compressing objects: 100% (30/30), done.
    remote: Total 49 (delta 3), reused 46 (delta 3)
    Unpacking objects: 100% (49/49), done.
    
    $ cd tooltwist-ansible/virtualbox
    $ vagrant up
    ...
    
The first time this command is executed it takes a while to run, as the base virtual machine is downloaded, and then Ansible is used to configure the machine. Once the server is running you can log in.

    $ vagrant ssh
    
## Further Information

See the [wiki](https://github.com/tooltwist/tooltwist-ansible/wiki) for more information.

--
