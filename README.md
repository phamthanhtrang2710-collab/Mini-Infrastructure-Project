# MiniLab Infrastructure Project
## Overview
Hello, welcome to my small project on system infrastructure. In this project, I will set up connections between 03 servers using virtual machines (UTM) on macOS, deploy and run a web server, work with Docker containers, and perform checks and troubleshooting on IP addresses, ports, services, and firewall configurations.

## Architecture
### Server Role
Server 1: Main management server configured with SSh and Docker

Server 2: Web server configured with Nginx

Server 3: Testing server for network diagnostics, SSH connectivity, and troubleshooting

### IP Address
Server 1: 10.190.139.4

Server 2: 10.190.139.5

Server 3: 10.190.139.6
### Ports and Services
	Service			|	Port	|	Server
	----------------|-----------|---------------
	SSH				|	22		|	All servers
	HTTP (Nginx)	|	80		|	server 2
	Docker container|	8080	|	server 1
	
## Project Highlights
•	Built a 3-node Ubuntu server lab using UTM on macOS

•	Configured SSH for remote administration between nodes

•	Deployed Docker containers and published services over custom ports

•	Installed and managed Nginx web server

•	Practiced Linux user management, file permissions, service control, and troubleshooting

•	Configured UFW firewall rules

•	Tested connectivity between nodes using ping, curl, SSH, and port inspection tools

## Screenshots
#### Virtual Machine Set Up
View here: [Open Folder](https://github.com/phamthanhtrang2710-collab/Mini-Infrastructure-Project/tree/dec969b0d7d627ef21fa7d5ebe4881bd2c37e1e1/Screenshots/Virtual%20Machine%20Set%20Up)

#### Network Set Up
View here: [Open Folder](https://github.com/phamthanhtrang2710-collab/Mini-Infrastructure-Project/tree/2eed9cd77672ed4eb6720063dcb1b0813429c65b/Screenshots/Network%20Set%20Up)

#### SSH Set Up
View here: [Open Folder](https://github.com/phamthanhtrang2710-collab/Mini-Infrastructure-Project/tree/d845594dac14c068109c56f8a6ac2175eaa07392/Screenshots/SSH%20Set%20Up)

#### Docker Set Up
View here: [Open Folder](https://github.com/phamthanhtrang2710-collab/Mini-Infrastructure-Project/tree/8767d7424c4dac8dd0838a975b8c919fab593ec9/Screenshots/Docker%20Set%20Up)

#### Nginx Set Up
View here: [Open Folder](https://github.com/phamthanhtrang2710-collab/Mini-Infrastructure-Project/tree/4a259f8be85e2780445109522780ec9feae1ee12/Screenshots/Nginx%20Set%20Up)

#### Firewall Set Up
View here: [Open Folder](https://github.com/phamthanhtrang2710-collab/Mini-Infrastructure-Project/tree/dbf38b8ff1b0c6de26172417dc387755d5e95e4b/Screenshots/Firewall%20Set%20Up)

## Skills Gained
My project shows skills relevant to
### IT Support

	•	Troubleshooting connectivity issues
	•	Using CLI tool (ping, curl, systemctl)
### System Administration
	•	Linux user and service management
	•	Firewall configuration (UFW)
	•	SSH set up and remote access
	•	Container deployment with Docker
### Networking
	•	Networking basic troubleshooting (ping, curl, ports)
	•	IP addressing and connectivity testing
	•	Port and service verification
