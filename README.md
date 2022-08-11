# Vagrant Setup
### Prerequisites 
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

### Creating a VM from command line
1. run `vagrant up`
![image](https://user-images.githubusercontent.com/110126036/184164845-04a853e7-57d5-4ff6-b920-ef76c996b4da.png)
2. run `vagrant ssh`
![image](https://user-images.githubusercontent.com/110126036/184165205-62e2ace8-4669-485a-98bf-846eef4eeb18.png)
3. Your command line should now display this (you are inside the virtual machine).
![image](https://user-images.githubusercontent.com/110126036/184165286-324e0646-48f5-411f-a055-8a9c7935ef3c.png)

We will now be automating the update and upgrade of the OS.

1. Create a shell file.
![image](https://user-images.githubusercontent.com/110126036/184166109-5229d987-1769-4fb6-9938-a9a6d97660c8.png)

2. Input the commands into the file
![image](https://user-images.githubusercontent.com/110126036/184166495-fed1345d-f777-4a64-845d-8daa146ad916.png)

3. We can check if the file has any permissions.
![image](https://user-images.githubusercontent.com/110126036/184166826-5999cae8-34ef-417a-9e28-a845007c9c76.png)

4. Give execute permissions to the file.
![image](https://user-images.githubusercontent.com/110126036/184167109-ab470118-4636-4eda-b0e7-c66072ba457f.png)

5. Run the file.
![image](https://user-images.githubusercontent.com/110126036/184167484-71602439-5544-47f3-9cac-bd8c5f086856.png)
![image](https://user-images.githubusercontent.com/110126036/184167574-770175e7-5fd4-4076-9630-224a16d9a877.png)

### Useful Linux commands

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
  
