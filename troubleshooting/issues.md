# Troubleshooting Issues
This section records common issues, errors, and solutions during this project setup
## Issue 1. Web Server NOT Accessible
Unable to access web server from another server using curl

#### Actions Performed
• Checked network connectivity using ping

    ping -c 4 10.190.139.5
    ping -c 4 10.190.139.6
• Verified server ip address

    hostname -I
• Checked nginx status

    systemctl status nginx
#### Solution
• Started nginx

    systemctl start nginx
• Verified service is running - "Active (running)"

• Rechecked connection

    curl http://10.190.139.5
## Issue 2. Firewall Blocking Access
Web server is running but cannot be accessed from another machine

#### Actions Performed
• Checked Nginx status

    systemctl status nginx
• Checked open port

    ss -tulnp
• Checked firewall status

    ufw status
#### Solution
• Allowed HTTP traffic

    ufw allow 80/tcp
• Checked if firewall rules was updated

    ufw status
• Rechecked access

    curl http://10.190.139.5

## Issue 3. Docker Container NOT Responding
Cannot access the web server running on port 8080

#### Actions Performed
• Checked Docker status

    systemctl status docker
• Checked running containers

    docker ps
#### Solution
• Started Docker

    systemctl start docker
• Restarted container

    systemctl restart nginx
• Confirmed containers is running and accessible

    systemctl status nginx

## Issue 4. SSH Connection Refused
Cannot access to remote server via SSH
#### Actions Performed
• Checked SSH status

    systemctl status ssh
    
• Checked network connectivity using ping

    ping -c 4 10.190.139.5
    ping -c 4 10.190.139.6
• Checked firewall rules for port 22

    ufw status
#### Solution
• Started ssh

    systemctl start ssh
• Allow SSH traffic

    ufw allow ssh
• Reconnected

    ssh verra@10.190.139.5
## Issue 5. Incorrect IP Address
Cannot reach server using ping because of wrong IP address
#### Actions Performed
• Checked IP address

    hostname -I
• Compared to the expected IP
#### Solution
• Updated command with correct IP address

• Checked connectivity using ping

    ping -c 4 10.190.139.5
    ping -c 4 10.190.139.6
