# SSH and Telnet Remote Access Lab

## Overview
This lab demonstrates how to configure remote access to a Cisco router using both SSH and Telnet.

## Topology

- 1 Cisco Router (R1)
- 1 Windows PC

## IP Addressing

| Device | Interface | IP Address |
|----------|----------|------------|
| R1 | Fa0/0 | 50.0.0.1/24 |
| PC | NIC | 50.0.0.10/24 |

## Objectives

- Configure basic router settings
- Assign an IP address to the router interface
- Configure Telnet access
- Configure SSH access
- Create a local user account
- Generate RSA keys for SSH encryption
- Verify remote connectivity

## Router Configuration

### Basic Security
- Hostname configured
- Enable secret password configured
- Password encryption enabled
- MOTD banner configured

### Interface Configuration
- FastEthernet0/0 configured with IP address 50.0.0.1/24
- Interface enabled using `no shutdown`

### SSH Configuration
- Local username created
- Domain name configured
- RSA keys generated
- SSH Version 2 enabled

### VTY Configuration
- Local authentication enabled
- SSH and Telnet allowed on VTY lines

## Verification

### Test Connectivity

From the PC:

```text
ping 50.0.0.1