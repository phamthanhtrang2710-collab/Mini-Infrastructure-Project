# Networking
This file configures basic networking between VMs

## Configure IP Address
Command:

    ip a
Or

    hostname -I

(Write down the IP address)

• Server 1: 192.168.1.123

• Server 2: 192.168.1.147

• Server 3: 192.168.1.125

## Test Connectivity
From server 1 to server 2

Command:

    ping -c 4 192.168.1.147

Reverse:

    ping -c 4 192.168.1.123

From server 1 to server 3, and reverse

    ping -c 4 192.168.1.125 (on S1)
    ping -c 4 192.168.1.123 (on S3)

## Set Hostname (If Needed)
Command:

    sudo hostnamectl set-hostname server1

## Verification
• Server can ping each other

• Hostname update correctly
