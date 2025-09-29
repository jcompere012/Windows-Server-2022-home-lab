# Windows Server 2022 With Active Directory Home Lab

Set up Windows Server environment to practice Active Directory management and network configuration.

## Prerequisites

- VirtualBox installed on host machine
- Window Server 2022 ISO
- Windows 11 Pro ISO (for domain-join testing)
- Minimum 4GB RAM and 32 GB disk space
  
## Key Tasks
- Installed Windows Server 2022
- Configured AD DS and promoted server to domain controller
- Create Organization Units and user accounts
- Set up Group Policies (e.g., password policy, desktop wallpaper)
- Create and file share

### 1. Install Active Directory Domain Services
- Open Server Manager → Add Roles and Features
- Select **Active Directory Domain Services**
- Promote server to domain controller
  - Domain name: `Server.local`
  - Restart after configuration
<img width="1470" height="956" alt="1step" src="https://github.com/user-attachments/assets/26d80fa7-7625-4b46-bceb-eebdd6f40be7" />


<img width="1470" height="956" alt="2nd step" src="https://github.com/user-attachments/assets/7993b87a-7853-4ece-a506-a73917f915db" />


<img width="1470" height="956" alt="3 ste" src="https://github.com/user-attachments/assets/42b60110-afbd-487c-b163-77b9b6734158" />

<img width="1470" height="956" alt="Screenshot 2025-09-28 at 4 30 31 PM" src="https://github.com/user-attachments/assets/5122658c-1774-46fd-a809-ee1a4b8f6701" />

<img width="1470" height="956" alt="Screenshot 2025-09-28 at 5 02 33 PM" src="https://github.com/user-attachments/assets/b1abc89a-18d9-45ea-b9f0-b5f5a010cb7c" />


    

### 2. Create Organizational Units and Users
- Open **Active Directory Users and Computers**
- Create OU: `Europe, USA,`
-   Create nested OU inside the locations 'USA > Computers, Users, Server'
-   Create Users inside the nested OU

  <img width="1470" height="956" alt="OU" src="https://github.com/user-attachments/assets/27447854-8f8c-4d65-a755-9c5cde287d9a" />

  <img width="1470" height="956" alt="user profile" src="https://github.com/user-attachments/assets/8969f662-d53f-4d76-bc98-0a93175ad3ec" />

  



### 3. Configure Group Policy
- Create Group Policy Management
- Create GPO: `Password policies, `
  - Set password policy
  - Configure desktop wallpaper


<img width="1470" height="956" alt="GPO creation" src="https://github.com/user-attachments/assets/05feb3f2-bcbe-4f8c-822c-50f474d49541" />

<img width="1470" height="956" alt="password policy gpo" src="https://github.com/user-attachments/assets/f2cdd819-5f60-45d3-8452-e511cbe8c228" />


<img width="1470" height="956" alt="GPO" src="https://github.com/user-attachments/assets/2348d4a0-064f-43a8-b48b-983153f00181" />

















