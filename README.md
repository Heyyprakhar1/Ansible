Firstly, we'll create 1 master server through which all the changes will be pushed to the slave node. cOnce, the creation of the master node gets completed, install the ansible on the master node using the following package commands :-       
sudo apt-get update
sudo apt-get install -y software-properties-common
sudo apt-add-repository ppa:ansible/ansible
sudo apt-get update
sudo apt-get install -y ansible
ansible --version

Ansible hots files are used to store all the information about the existing servers and the variables I want to use in the slave nodes. so, that hostfile exists in the location :- sudo vim /etc/ansible/hosts
<img width="928" height="313" alt="image" src="https://github.com/user-attachments/assets/85cdb064-dc90-4889-b091-67d931c77a27" />
all the details should be filled over the hostfile and then we need to connect all the slave nodes to the private key through ssh. 
I am using windows Laptop, so the process is little bit tougher for me. 
