# Vagrant Setup
1. Install Ruby
2. Install Vagrant
3. Install VirtualBox
4. (WINDOWS USERS) Control Panel --> Network and Internet --> Network and Sharing Center --> Change adapter settings --> VirtualBox Host-Only Network (Properties) --> Install --> Service --> Manufacturer: Oracle Corporation, Network Service: VirtualBox NDIS6 Bridged Networking Driver --> Click OK
5. Create a directory and then a file. Input the following into the file.
```
Vagrant.configure("2") do |config|

 config.vm.box = "ubuntu/xenial64" # Linux - ubuntu 16.04

# creating a virtual machine ubuntu 

end
```
6. `vagrant up` to start up the VM
7. Check the status using `vagrant status`
8. Use `vagrant ssh`

You are now inside the virtual machine.

You can use `exit` to leave the VM.

- How can we find out the name of OS `uname` or `uname -a` 
- How to create a file in linux, `touch filename` or `nano filename` 
- How to check existing file/folders `ls` or `ls -a`
- How to create a folder `mkdir foldername`
- How to navigate to the folder `cd foldername`
- How to come out of folder (1 step back) `cd ..`
- How to check our current location `pwd`
- `whoami`
- how to copy file `cp filename_with_absolute_path destination_with_absolute_path` 
- how to remove file/folder `rm -rf filename/foldername`
- how to cut paste the file/move the test file `mv filename_with_absolute path destination_with_absolute_path`
- how to present processes `top` exit with `ctrl c`. Can also use `ps aux`
- can remove/delete/kill processes in linux 
- how to use `|` pipe
- can act as admin/root user with `sudo su` or `sudo i`
- how to check file permissions `ll`
- how to change file permission `chmod permission filename`
- to make executable `chmod +x filename`, `all`, `r`, `w`, `rw` also numbers `400` or `600` for all `700`
- linux commands to communicate with world wide web
- update our ubuntu OS `sudo apt-get update`
- upgrade our ubuntu os `sudo apt-get upgrade` or `sudo apt-get upgrade -y`
- how to create automate tasks with provisioning scripts
- automate update and upgrade
- make .sh folder and make it executable. call the filename with ./filename to run it
- contents of a file `cat filename`
  