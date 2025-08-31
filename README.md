# About this Ansible_Project
Trying to make a basic automation via Ansible to retrive data from new VM's. Along with setup automation and connection with Node.

# Step 1
We need to have VM configured. In this project I am using AWS as it has free tier t2.micro Instances. First make a Instane which is going to be out master node (Ubuntu instances) and configure it. We will now SSH into the VM using Console connect or SSH via Public IP address. 

![alt text](1.PNG)

Once inside VM run the below command.

```bash
sudo apt update
sudo apt upgrade -y
sudo apt install ansible -y
```
![alt text](2.PNG)

# Step 2
The above command will install the important packages and also install Ansible. 
Once done run the below command.

```bash
ssh-keygen
```
![alt text](3.PNG)
![alt text](4.PNG)

This will generate key and keep clicking enter until files are created. You can make chnages but default settings are ok. The command created 3 files id_ed25519, id_ed25519.pub and authorized_keys.
Now run the below command.

```bash
cd /.ssh
cat id_ed25519.pub
```
COPY the output we will need it in User_Data.yml

