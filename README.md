# automate_with_ansible

## Project Summary
In this hands-on project, we'll use Ansible to automate the setup of a simple web application environment on four virtual machines hosted in AWS. All four VMs are configured within the same local VPC (Virtual Private Cloud) network, ensuring secure and efficient communication between the servers.

The setup is as follows: <br>
Ansible Controller: This server is responsible for managing and orchestrating the automation tasks across the environment. <br> 
Two Web Servers: These servers will host the web application using Nginx as the web server software. They serve as the front-end for delivering the web content. <br>
One Database Server: This server will run MySQL, handling all database operations for the application. <br>

## Implementation

### VMs Setup
![image](https://github.com/user-attachments/assets/ef127f12-6056-4b31-a910-5150ba49f4ea) <br>

### Ansible controller setup
Login(SSH) to the ansible_controller VM and install ansible<br>
```
  sudo apt update
  sudo apt install software-properties-common
  sudo add-apt-repository --yes --update ppa:ansible/ansible
  sudo apt install ansible
```
![image](https://github.com/user-attachments/assets/2c0eeef8-a5da-41b9-bbe8-b29af074359d) <br> <br>

Create an Ansible configuration file to specify the inventory <br>
![image](https://github.com/user-attachments/assets/65ef10ae-602d-4307-b61c-4891f47cecb6) <br> <br>


### Write inventory files
Write the inventroy files in the ansible_controller VM that will provide information (e.g. IP address, username, passwords etc) to ansible about it's targets. <br>
![image](https://github.com/user-attachments/assets/29519cd7-f221-4138-bf02-03671c6cdda6) <br> <br>


### Test Connections
![image](https://github.com/user-attachments/assets/e1f3ee0e-3605-4461-a512-2d33b0054357) <br> <br>
![image](https://github.com/user-attachments/assets/c443cde1-51a8-4498-8e6c-802873cc952e) <br> <br>




