# Active Directory Home Lab

## Project Overview

This project documents the deployment and configuration of a Windows Server 2022 Active Directory Home Lab built in Oracle VirtualBox. The lab demonstrates common Help Desk and System Administrator tasks performed in an enterprise environment.

## Technologies Used

- Windows Server 2022
- Active Directory Domain Services (AD DS)
- DNS
- Oracle VirtualBox
- Windows 11 Client
- GitHub

## Skills Demonstrated

- Installing Windows Server 2022
- Promoting a Domain Controller
- Configuring Active Directory
- Creating Organizational Units (OUs)
- Creating User Accounts
- Managing Security Groups
- Password Resets
- User Account Unlocks
- Group Membership Management
- Basic Help Desk Administration

## Project Goals

- Build a functioning Active Directory environment
- Simulate real-world Help Desk tasks
- Gain hands-on Windows Server experience
- Document the project for employers

## Lab Screenshots
# Phase 1 – Windows Server 2022 Installation

## Step 1 – Create the Windows Server Virtual Machine

![Step 1](server-1.png)

Downloaded the official Windows Server 2022 Evaluation ISO from Microsoft. This ISO will be used to create the D01 domain controller virtual machine for the Active Directory home lab
.

---

## Step 2 – Install Windows Server 2022

![Step 2](server-2.png)

Created the D01 virtual machine and attached the official Windows Server 2022 Evaluation ISO in Oracle VirtualBox


---

## Step 3 – Initial Server Setup

![Step 3](server-3.png)

Configured the virtual hardware for the DC01 Windows Server virtual machine (4 GB RAM, 2 CPUs, 80 GB virtual disk)



---

## Step 4 – Configure the Server

![Step 4](server-4.png)

Configured the Microsoft OS setup

---

## Step 5 – Prepare the Server

![Step 5](server-5.png)

After completing the installation, created a password under the administrator.

---

## Step 6 – Server Manager

![Step 6](server-6.png)

administrator login screen

---

## Step 7 – Windows Server Ready

![Step 7](server-7.png)

Successfully logged into the newly installed Windows Server 2022 virtual machine for the first time.

---

## Step 8 – Final Configuration

![Step 8](server-8.png)

Renamed the Windows Server host from its automatically generated name to DC01

---

## Step 9 – Windows Server Complete

![Step 9](server-9.png)

Windows Server 2022 installation successfully completed and ready for Active Directory deployment.


# Phase 2 – Active Directory Domain Services Installation

## Step 1 – Launch Add Roles and Features Wizard

![AD 1](ad-1.png)

Opened **Server Manager** and started the **Add Roles and Features Wizard** to begin installing Active Directory Domain Services.

---

## Step 2 – Select Installation Type

![AD 2](ad-2.png)

Selected the **Role-based or feature-based installation** option.

---

## Step 3 – Select Destination Server

![AD 3](ad-3.png)

Selected the local Windows Server 2022 machine (**DC01**) as the destination server.

---

## Step 4 – Select Active Directory Domain Services

![AD 4](ad-4.png)

Selected the **Active Directory Domain Services (AD DS)** server role.

---

## Step 5 – Review Required Features

![AD 5](ad-5.png)

Reviewed and accepted the required Windows features needed for Active Directory.

---

## Step 6 – Active Directory Domain Services Information

![AD 6](ad-6.png)

Reviewed Microsoft's overview of Active Directory Domain Services before continuing.

---

## Step 7 – Confirm Installation

![AD 7](ad-7.png)

Verified the installation selections before beginning the AD DS installation.

---

## Step 8 – Installation Complete

![AD 8](ad-8.png)

Successfully installed the Active Directory Domain Services role.

---

## Step 9 – Begin Domain Controller Promotion

![AD 9](ad-9.png)

Selected **Promote this server to a domain controller** to begin configuring the server as the first domain controller.

---

## Step 10 – Create a New Forest

![AD 10](ad-10.png)

Created a new Active Directory forest for the lab environment.

---

## Step 11 – Configure Domain Controller Options

![AD 11](ad-11.png)

Configured the Directory Services Restore Mode (DSRM) password and domain controller settings.

---

## Step 12 – Review Installation Options

![AD 12](ad-12.png)

Reviewed all Active Directory configuration settings before deployment.

---

## Step 13 – Prerequisite Checks

![AD 13](ad-13.png)

Verified that all prerequisite checks passed successfully before installing the Active Directory forest and promoting the server to a Domain Controller.


# Phase 3 – Active Directory Administration

This phase demonstrates  Help Desk and System Administration tasks performed in an Active Directory environment. These exercises simulate real-world user account management, Organizational Unit (OU) administration, security group management, and Role-Based Access Control (RBAC).

---

## Step 1 – Log On to the Domain Controller

![AD Admin 1](admin-1.png)

After promoting the Windows Server to a Domain Controller, I logged into the new Active Directory environment using the built-in domain Administrator account.

---

## Step 2 – Open Active Directory Users and Computers

![AD Admin 2](admin-2.png)

I opened the Active Directory Users and Computers (ADUC) management console from Server Manager → Tools.

---

## Step 3 – Create the Corporate Organizational Unit

![AD Admin 3](admin-3.png)

I created the Corporate Organizational Unit (OU) within homelab.localdomain

---

## Step 4 – Create the IT Organizational Unit

![AD Admin 4](admin-4.png)

I created the IT Organizational Unit (OU) inside the Corporate OU to represent the Information Technology department. 

---

## Step 5 – Complete the Organizational Unit Structure

![AD Admin 5](admin-5.png)

Created an Active Directory Organizational Unit to organize company resources by department

---

## Step 6 – Create the First Active Directory User

![AD Admin 6](admin-6.png)

Created the first Active Directory user account within the IT Organizational Unit.

---

## Step 7 – Create Department User Accounts

![AD Admin 7](admin-7.png)

Created and organized multiple departmental user accounts to simulate onboarding employees into different business units.

---

## Step 8 – Create Active Directory Security Groups

![AD Admin 8](admin-8.png)

Created departmental security groups to implement Role based access control (RABC)

---

## Step 9 – Add User to the Help Desk Security Group

![AD Admin 9](admin-9.png)

Added the user account Steven R. Pedlar to the Help Desk security group, demonstrating how access is managed using security group membership rather than assigning permissions directly to users.

---

## Step 10 – Reset a User Password

![AD Admin 10](admin-10.png)

Performed a password reset for an Active Directory user account. 

---

## Step 11 – Disable a User Account

![AD Admin 11](admin-11.png)

Disabled a user account to simulate employee offboarding and security procedures.

---

# Skills Demonstrated

- Windows Server 2022 Administration
- Active Directory Domain Services (AD DS)
- Domain Controller Deployment
- Active Directory Forest Creation
- DNS Configuration
- Organizational Unit (OU) Administration
- User Account Management
- Security Group Administration
- Role-Based Access Control (RBAC)
- Password Reset Procedures
- User Account Disablement
- Help Desk Administration
- Windows Server Manager
- Oracle VirtualBox
- GitHub Documentation
