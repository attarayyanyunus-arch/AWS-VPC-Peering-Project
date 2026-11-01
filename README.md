# AWS VPC Peering – Connecting Two Private Networks

**Internship:** EWB EDU TECH – AWS & DevOps  
**Student:** Ayyan Yunus Attar  
**Programme:** B.Tech Computer Engineering  
**Institute:** Eaglewood Polytechnic Institute  
**AWS Region:** Asia Pacific (Sydney) – `ap-southeast-2`

## Project Overview

This project demonstrates how to connect two separate Amazon Virtual Private Clouds (VPCs) using AWS VPC Peering. It enables private communication between resources in different VPC networks using private IP addresses.

## Project Objectives

- Create two separate VPC networks.
- Establish an active VPC Peering connection.
- Configure private route tables.
- Configure security group rules.
- Test connectivity between private EC2 instances.

## Network Configuration

| Resource | VPC A | VPC B |
|---|---|---|
| VPC Name | ewb-vpc-a | ewb-vpc-b |
| CIDR | 10.10.0.0/16 | 10.20.0.0/16 |
| Private Subnet | 10.10.2.0/24 | 10.20.1.0/24 |
| EC2 Private IP | 10.10.2.10 | 10.20.1.10 |

## VPC Peering Details

- Connection Name: `ewb-a-b-peer`
- Connection ID: `pcx-0f8becfc5a5c6ada4`
- Status: Active

## Connectivity Testing

Command executed from App-A:

`ping -c 4 10.20.1.10`

**Result:**
- 4 packets transmitted
- 4 packets received
- 0% packet loss
- Average RTT: 0.172 ms

The ICMP connectivity test was successful.

**Note:** SSH port 22 was checked but returned CLOSED. SSH connectivity is not claimed as successful.

## Project Evidence

Project screenshots and the final project report are included in this repository.

## Conclusion

The VPC Peering connection was successfully established between two separate VPC networks. Private route tables were configured, and ICMP connectivity between App-A and App-B was successfully verified.

**Prepared by:** Ayyan Yunus Attar
