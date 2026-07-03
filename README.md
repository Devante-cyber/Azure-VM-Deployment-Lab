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
- Deployment is complete

  <img width="1062" height="508" alt="image" src="https://github.com/user-attachments/assets/8abf5e82-ae15-49f4-9b06-593d22042aa1" />

## Step 5: Connect to the Virtual Machine

- Go to **Virtual Machines**
- Select `VM-Lab-01`

<img width="863" height="544" alt="image" src="https://github.com/user-attachments/assets/915e934d-bc5d-472f-b3c9-058ccc6774c9" />

- Copy the **Public IP Address**
- Open **Remote Desktop Connection (mstsc)** on your PC

  <img width="403" height="215" alt="image" src="https://github.com/user-attachments/assets/f661744d-924c-471d-9cf3-d5b57a8b8920" />

  <img width="414" height="246" alt="image" src="https://github.com/user-attachments/assets/01c00113-0b11-48c9-b2a8-8359d3096f72" />


- Enter credentials:

<img width="451" height="390" alt="image" src="https://github.com/user-attachments/assets/cbf39733-70cd-45a2-9982-3afe9403e3d1" />

## You should now be logged into a Windows desktop environment hosted in Azure

<img width="1893" height="1067" alt="image" src="https://github.com/user-attachments/assets/0b7a2676-1506-426d-9014-48340a83d6ef" />

## Step 6: Validate System Access

- Once logged in:
- Open **Task Manager**

<img width="716" height="400" alt="image" src="https://github.com/user-attachments/assets/9995360b-43e1-4750-9432-fe74b5ac0982" />
 
- Check CPU and memory usage

<img width="716" height="400" alt="image" src="https://github.com/user-attachments/assets/04435cb2-7696-4ddc-81ee-ad44cad5ce16" />
 
- Confirm internet connectivity (open Edge)

  <img width="1512" height="658" alt="image" src="https://github.com/user-attachments/assets/bfb7b8b8-675b-46a4-bfe7-c2b1913c0fe2" />

## Step 7: Stop and Deallocate the VM (Cost Control)

- Return to Azure Portal
- Select the VM
  
<img width="1081" height="779" alt="image" src="https://github.com/user-attachments/assets/b39d9418-07bb-4567-b1da-767ee01f0d4a" />
  
- Click **Stop**

   <img width="1081" height="779" alt="image" src="https://github.com/user-attachments/assets/d008c951-1b59-4816-9891-a52d44916aa0" />

5. Confirm **Deallocate**

<img width="758" height="567" alt="image" src="https://github.com/user-attachments/assets/7de2589e-7253-4b1b-9f65-de406fdf6da8" />

## Cost Control

- The virtual machine was stopped and deallocated after testing to prevent unnecessary Azure charges.

# What I Learned

- How to deploy and configure a virtual machine in Microsoft Azure
- How cloud networking enables secure remote access (RDP over port 3389)
- How resource groups help organize cloud infrastructure
- How to manage cloud costs by stopping/deallocating resources
- How to operate a Windows environment in a cloud-hosted VM

##  Key Takeaways

This lab demonstrates foundational cloud computing and system administration skills used in IT environments, including virtual machine provisioning, remote access configuration, and basic network security concepts.

  

