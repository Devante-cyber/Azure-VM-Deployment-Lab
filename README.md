# Azure-VM-Deployment-Lab
The objective of this lab is to demonstrate how to deploy and manage a Windows Virtual Machine in Microsoft Azure. This includes creating a VM, configuring access, and connecting using Remote Desktop Protocol (RDP).


##  Skills Demonstrated

- Azure Virtual Machine deployment
- Resource Group management
- Virtual networking basics (IP, ports, NSG)
- Remote Desktop Protocol (RDP)
- Cloud resource lifecycle management
- Cost management (stop/deallocate VM)

## 🛠️ Lab Environment

- Microsoft Azure Portal
- Windows 10/11 Virtual Machine image
- Remote Desktop Connection (RDP)
- Internet connection

# Lab Steps

## Step 1: Create a Resource Group

- Sign in to the Azure Portal: https://portal.azure.com  
- Search for **Resource Groups**

<img width="1077" height="793" alt="Screenshot 2026-07-03 181207" src="https://github.com/user-attachments/assets/c0ca9363-c917-4e52-b131-24286aa29409" />
   
- Click **Create**

- Configure:
   - Subscription: Your Azure subscription
   - Resource Group Name: `RG-Azure-VM-Lab`
   - Region: Choose the closest region (e.g., East US)
- Click **Review + Create**
- Click **Create**
  
<img width="783" height="373" alt="Screenshot 2026-07-03 181339" src="https://github.com/user-attachments/assets/d749e81d-052e-4f4e-941c-3050307caa82" />

## Step 2: Create a Virtual Machine

- In Azure Portal, search **Virtual Machines**
  
   <img width="507" height="388" alt="Screenshot 2026-07-03 181848" src="https://github.com/user-attachments/assets/369f9e66-4442-4df5-a695-f4aff649260b" />

- Click **Create → Azure Virtual Machine**

<img width="669" height="540" alt="Screenshot 2026-07-03 181926" src="https://github.com/user-attachments/assets/057c719c-4db1-4aa2-804e-e602b11b8541" />

### Basic Configuration:
- Subscription: Default
- Resource Group: `RG-Azure-VM-Lab`
- Virtual Machine Name: `VM-Lab-01`
- Region: Same as resource group
- Image: Windows 10/11 Pro
  
<img width="928" height="780" alt="image" src="https://github.com/user-attachments/assets/49de9228-956e-4113-b470-4d761ab5c4f0" />

### Administrator Account:
- Username: `azureadmin`
- Password: Create a strong secure password

<img width="891" height="192" alt="image" src="https://github.com/user-attachments/assets/66214b0f-c031-4dbc-82dc-cecc67a3dbc5" />

## Step 3: Configure Networking 

### In the Networking tab:

- Virtual Network: Auto-created (default is fine)
- Subnet: Default
- Public IP: Enabled (required for RDP access)

<img width="846" height="737" alt="image" src="https://github.com/user-attachments/assets/430acac1-29d3-4f54-ae49-d42657c218cd" />

##  Step 4: Review and Deploy VM
