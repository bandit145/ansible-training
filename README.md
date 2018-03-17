# ansible-training
Repo for the /r/sysadmin Ansible training


To use this you need two things:

1.	Vagrant https://www.vagrantup.com/downloads.html (for linux install the "vagrant" package with your package manager)
2.	VirtualBox https://www.virtualbox.org/

If you are on linux you are going to need to change the folder mapping location for the Ansible server:

```client.vm.synced_folder "C:/Users/"+ENV["user"]+"/Desktop", "/ansible"```

Change that to whatever location you want on your machine.