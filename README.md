# About this Ansible_Project
Trying to make a basic automation via Ansible to retrive data from new VM's. Along with setup automation and connection with Node.
#Step 1
We need to have VM configured. In this project I am using AWS as it has free tier t2.micro Instances. First make a instane which is going to be out master node (Ubuntu instances) and configure it.
\\\bash
sudo apt update
sudo apt upgrade -y
sudo apt install ansible
\\\