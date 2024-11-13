# automate_with_ansible

## Project Summary
In this hands-on project, we'll use Ansible to automate the setup of a simple web application environment on four virtual machines hosted in AWS. All four VMs are configured within the same local VPC (Virtual Private Cloud) network, ensuring secure and efficient communication between the servers.

The setup is as follows: <br>
Ansible Controller: This server is responsible for managing and orchestrating the automation tasks across the environment. <br> 
Two Web Servers: These servers will host the web application using Nginx as the web server software. They serve as the front-end for delivering the web content. <br>
One Database Server: This server will run MySQL, handling all database operations for the application. <br>

## Implementation

### VMs Setup
![image](https://github.com/user-attachments/assets/5cb29c9e-a2d6-48bd-a10a-d2c096acf20a) <br>

### Ansible controller setup
Login(SSH) to the ansible_controller VM and install ansible and python. <br>
```
  sudo apt update
  sudo apt install software-properties-common
  sudo add-apt-repository --yes --update ppa:ansible/ansible
  sudo apt install ansible
```

### Write inventory files
Write the inventroy files in the ansible_controller VM that will provide information (e.g. IP address, username, passwords etc) to ansible about it's targets. <br>
![image](https://github.com/user-attachments/assets/56310afe-578d-4ba5-8e44-05dc0bf94d4d)

