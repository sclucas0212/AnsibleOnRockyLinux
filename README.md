# Ansible Install - Rocky Linux

My notes last update 20 August 2021

Install EPEL

    $ sudo dnf install epel-release
    
Install python3-pip

    $ sudo dnf install python38 python38-pip python38-wheel python3-argcomplete rust cargo curl
    
 
Set Python to python 3.8

    $ sudo alternatives --set python /usr/bin/python3.8
    
Update pip (I ran to an error here and found this command on the web)

    $ sudo pip3 install --upgrade pip
    
Install Ansible

    $ sudo pip3 install ansible
    $ sudo activate-global-python-argcomplete
    
Check Ansible version

    $ ansible --version
    
If you receive a message about not being on python 3.8 use the following command line utility to point python to python 3.8

    $ update-alternatives --config python
    
  


### References
[Installation on the management server](https://docs.rockylinux.org/books/learning_ansible/01-bases)
