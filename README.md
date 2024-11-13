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
