Active Directory + Azure AD Hybrid Integration Lab

📌 Overview

This project demonstrates a hybrid Active Directory integration with Microsoft Azure.
It simulates a real-world enterprise setup where an on-premises Active Directory Domain Services (ADDS) environment is synchronized with Azure Active Directory using Azure AD Connect.

The goal is to enable single identity for users across on-prem and cloud environments, and provide seamless login to Microsoft 365 services.

🏗️ Lab Architecture

On-Premises (Azure VM acting as DC):

Windows Server (ADDS, DNS installed)

Test users created (e.g., TestUser1, TestUser2)

Cloud:

Azure Active Directory (Free Tier Subscription)

Office 365 tenant (trial licenses)

Azure AD Connect installed on the on-prem server

🔗 Hybrid Connection: ADDS → Azure AD → Office 365

⚙️ Steps Implemented

Provision Azure Resources

Subscribed to Azure Free Tier

Created Windows Server VM with static private IP

Promoted VM to Domain Controller (india.com)

Active Directory Setup

Created 2 test users (TestUser1, TestUser2)

Configured DNS for domain resolution

Azure AD Connect

Installed Azure AD Connect on the VM

Connected on-prem ADDS with Azure AD tenant (*.onmicrosoft.com)

Configured Password Hash Sync for hybrid identity

User Synchronization

Verified TestUser1, TestUser2 synced to Azure AD portal

Assigned Microsoft 365 licenses

Tested cloud login (Office.com)

📊 Outcomes

✅ On-prem AD users synced successfully to Azure AD

✅ Single sign-on working with Office 365 apps

✅ Azure AD portal showing synced identities

✅ Configured hybrid identity management
