# AWS VPC Peering Project

## Overview
This project connects two Amazon VPCs securely using VPC Peering in the AWS Mumbai region (`ap-south-1`).

## Architecture
- **VPC A:** `10.10.0.0/16`
- **VPC B:** `10.20.0.0/16`
- **EC2 Instances:** Bastion, App-A, and App-B
- **Networking:** Custom route tables, security groups, and VPC Peering

## Implementation
1. Created two separate VPCs with different CIDR ranges.
2. Configured subnets, an Internet Gateway, and route tables.
3. Established an active VPC Peering connection.
4. Configured security groups for SSH and ICMP traffic.
5. Connected to private instances through the bastion host.
6. Tested connectivity between App-A and App-B.

## Test Result
**Successful:** App-A pinged App-B (`10.20.1.76`) with 4 packets received and 0% packet loss.

## Technologies Used
- Amazon Web Services (AWS)
- Amazon VPC and VPC Peering
- Amazon EC2
- Security Groups and Route Tables
- SSH and ICMP

## Screenshots
Screenshots of the VPC peering connection, route tables, VPCs, EC2 instances, and connectivity tests are included in this repository.

## Author
Ziya Shaikh
