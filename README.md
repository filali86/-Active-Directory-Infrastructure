# -Active-Directory-Infrastructure

Enterprise Active Directory Infrastructure Setup

## Overview
This project involves building a complete Windows Server domain infrastructure from the ground up, including Domain Controller promotion, DNS integration, organizational unit design, and comprehensive Group Policy implementation.

## Environment & Technologies
- Windows Server 2022
- Active Directory Domain Services
- DNS Server
- Group Policy Objects
- Organizational Units
- Windows 10/11 Client
- Oracle VirtualBox

## Step-by-Step Implementation

### 1. Server Preparation
- Installed Windows Server 2022
- Configured static IP address (192.168.11.106/24)
- Set DNS server to loopback (127.0.0.1) for self-resolution

### 2. Role Installation
- Installed Active Directory Domain Services role
- Automatically installed DNS Server as required feature
- Prepared server for domain controller promotion

### 3. Domain Controller Promotion
- Created new forest with root domain `Marwan.local`
- Configured Directory Services Restore Mode password
- Set functional levels and additional options
- Passed prerequisites check successfully

### 4. DNS Configuration
- Verified DNS zones created automatically
- Confirmed SRV records for domain services
- Tested name resolution internally and externally

### 5. Organizational Unit Structure
- Designed hierarchical OU structure by geography (USA, Europe, Asia)
- Created sub-OUs for Computers, Servers, and Users
- Implemented logical grouping for efficient management

### 6. User & Computer Management
- Created user accounts with detailed attributes
- Organized computer objects by location and function
- Implemented security and distribution groups

### 7. Group Policy Implementation
- Configured password policies with complexity requirements
- Implemented desktop management policies
- Set security restrictions and access controls
- Applied GPOs to appropriate OUs

### 8. Client Integration
- Configured client DNS to point to Domain Controller
- Joined client computers to the domain
- Verified policy application and functionality

## Challenges & Solutions
- **Challenge**: Building enterprise infrastructure from scratch
- **Solution**: Methodical approach following Microsoft best practices
- **Challenge**: Ensuring reliable name resolution and service discovery
- **Solution**: Proper DNS configuration and client settings

## Key Learnings
- Active Directory forest and domain architecture
- DNS integration with AD DS
- Organizational Unit design principles
- Group Policy hierarchy and processing
- Enterprise-scale user and computer management
- Domain joining and trust relationships

## Screenshots
![Server Manager](/screenshots/1.png)
![Static IP Configuration](/screenshots/2.png)
![AD DS Installation](/screenshots/3.png)
![DC Promotion](/screenshots/4.png)
![Prerequisites Check](/screenshots/5.png)
![OU Structure](/screenshots/6.png)
![User Accounts](/screenshots/7.png)
![GPO Configuration](/screenshots/8.png)
![GPO Configuration](/screenshots/9.png)
![GPO Configuration](/screenshots/x.png)
