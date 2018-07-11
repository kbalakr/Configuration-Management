# HW1:

Objective: Install virtualbox, vagrant, phpvirtualbox and bring a VM operationally up inside another headless VM 
           with the help of ansible
Topology:  There are two VMs initially, one running ansible which is connected to another VM to intall the prerequisites.

![final topology](https://media.github.ncsu.edu/user/6167/files/b17f08f0-94e9-11e7-8414-ddc43b5bb6fa)

The host's private key is added as a key in the Ansible server and the inventory in the ansible server consists of the host details 
including the path were the key is stored. It is made sure that the remote host is reachable from the ansible server through ssh.

Ansible is installed in the ansible server and a .yaml file is written to install virtual box, vagrant and php virtualbox in the remote host.
Also, a new VM is brought up operationally in the remote host vm.

The details of running the yaml script can be understood from the screencast. Also, the yaml file has been uploaded.
 NOTE: Both the remote host VM and the inner VM run instances of trusty. The outer VM is 64 bit and the inner VM is 32 bit.
 
 Ansible server IP: 192.168.33.10
 Remote Host IP: 192.168.33.81
 
# Screencast Link:

https://www.youtube.com/watch?v=unyh5XucfL8&feature=youtu.be

# Reference: 

  Modification to the image from https://github.com/CSC-DevOps/CM/blob/master/Ansible.md was done and attached


