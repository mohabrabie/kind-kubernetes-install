# installing kubernetes cluster using Kind on Ubuntu 🚀
in this documentation I will show you the steps of creating a cluster using kind locally and allowing access for a specific IP to the APIServer and run commands on the Master

### Prerequisites
- 2 VMs ubuntu 22.04 installed on them
- Docker installed on the server
- kubectl installed on both

## Installation 💻
1- go to the web site for kind https://kind.sigs.k8s.io/
![Screenshot](1.png)

2- go to installation part and use the link to you're system 
![Screenshot](2.png)

3- create a configuration file as shown but add the VM IP as apiServerAddress under networking in the config file
![Screenshot](3.png)

4- then run the kind create command to create the cluster [1 master,2 nodes]
![Screenshot](4.png)

5- install kubectl to check if the nodes are up and running
![Screenshot](5.png)

6- create a ufw rols to allow only access from the client VM IP address to allow the connection between the client to the server
![Screenshot](6.png)

7- check the ufw status to check the roles created
![Screenshot](8.png)

8- copy the configuration file from the $HOME/.kube/config on the server to the $HOME/.kube/config to be able to connect 
![Screenshot](7.png)
