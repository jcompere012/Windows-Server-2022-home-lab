# Windows Server 2022 With Active Directory Home Lab

Set up Windows Server environment to practice Active Directory management and network configuration.



# Youtube Video Link
-  ### [Cloud Azure Active Directory Set UP](https://youtu.be/9QCERCaoIW0)

## Prerequisites

- VirtualBox installed on host machine
- Window Server 2022 ISO
- Windows Server act as Client 
  
## Key Tasks
- Installed Windows Server 2022
- Configured AD DS and promoted server to domain controller
- Create Organization Units and user accounts
- Join local domain

### 1. Install Active Directory Domain Services
- Open Server Manager → Add Roles and Features
- Select **Active Directory Domain Services**
- Promote server to domain controller
  - Domain name: `Lab.local`
  - Restart after configuration
<img width="1470" height="956" alt="1step" src="https://github.com/user-attachments/assets/26d80fa7-7625-4b46-bceb-eebdd6f40be7" />


<img width="1470" height="956" alt="2nd step" src="https://github.com/user-attachments/assets/7993b87a-7853-4ece-a506-a73917f915db" />


<img width="1470" height="956" alt="3 ste" src="https://github.com/user-attachments/assets/42b60110-afbd-487c-b163-77b9b6734158" />

<img width="1470" height="956" alt="Screenshot 2025-09-28 at 4 30 31 PM" src="https://github.com/user-attachments/assets/5122658c-1774-46fd-a809-ee1a4b8f6701" />



    

### 2. Create Organizational Units and Users
- Open **Active Directory Users and Computers**
- Create OU: `Training, HR`
-   Create nested OU inside the locations 'Training > Users , Computers'
-   Create Users inside the nested OU

 <img width="879" height="612" alt="Screenshot 2025-12-10 at 2 44 25 PM" src="https://github.com/user-attachments/assets/d79448cd-b44f-4dba-a51c-72653a43011c" />

 <img width="885" height="700" alt="Screenshot 2025-12-10 at 2 53 20 PM" src="https://github.com/user-attachments/assets/15c2aa9b-b186-43a8-98c8-50c989364a9d" />





### 3. Join Local Domain
- Spin another Datacenter VM and act as a client machine 
- Machine `Client1`
  - Configure network to connect both machine and join the domain
  - Join the `Lab.local`
  - ping the `lab.local` to confirm the machine is connected
 
<img width="1544" height="921" alt="Screenshot 2025-12-10 at 3 24 09 PM" src="https://github.com/user-attachments/assets/b053c38e-423b-43cb-8743-2b11a13660f2" />

<img width="1193" height="636" alt="Screenshot 2025-12-10 at 4 06 26 PM" src="https://github.com/user-attachments/assets/825aca1c-f2ac-4d63-a2d7-1eb6e4ebc6c4" />

<img width="1144" height="636" alt="Screenshot 2025-12-10 at 3 29 09 PM" src="https://github.com/user-attachments/assets/4feee0bb-ed95-4fd8-9018-3e1d540d5073" />

<img width="1144" height="872" alt="Screenshot 2025-12-10 at 3 28 44 PM" src="https://github.com/user-attachments/assets/eeb498e7-1029-4313-8745-0712df770e8f" />



















