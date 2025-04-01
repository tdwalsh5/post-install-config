<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Configuration Steps</h2>

<p>
<img src="post-install-shot1.PNG" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now that osTicket is successfully installed and running, we can start system administration tasks. Starting with configuring new roles within the help desk. This will allow effective management of user access and permissions.
</p>
<br />

<p>
<img src="post-install-shot2" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To configure new roles within osTicket for the helpdesk, go to the admin panel in the top right of the page, then click Agents -> Roles -> Add New Role. Enter the name of the new role, in my case I used "Supreme Admin". Now you can grant permissions to this role, since I created a Supreme Admin role, I granted the role to have access to all permissions. This allowed me to have full access to the tickets and any adjustments I wanted to make for learning purposes. 
Admin Panel -> Agents -> Roles
</p>
<br />

<p>
<img src="post-install-shot3" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After configuring the roles desired, we will create departments. In the Agents tab, select Departments -> Add New Department. Create a new department called "SysAdmins" (short for System Administraters) and will serve as the designated department for System Administraters. We will be putting the "Supreme Admin" role into this department. Also make sure to have the Parent of this department be "Top Level Department". Additional settings, such as SLAs, managers, and email configurations, can be customized within the Departments tab to align with your help desk's operational needs. Make sure to click "Create Dept" after finishing configurations.
Admin Panel -> Agents -> Departments
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now we will configure Teams. To do so navigate to Admin Panel -> Agents -> Teams. Creating teams allows us to group agents from different departments to collaborate effectively. Create a team named "Online Banking" and assign agents from different departments as needed.
Admin Panel -> Agents -> Teams
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this simulated case, I wanted to allow anyone to create tickets. Navigate to Admin Panel -> Settings -> User Settings. Uncheck the box "Require registration and login to create tickets" allowing unregistered users to submit tickets without needing an account.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To configure agents (workers), navigate to Admin Panel -> Agents -> Add New. Fill in the necessary details, in my project I created Jane and John Doe. I assigned Jane to the SysAdmins department and John to the Support Department. The support department was a default, and did not need to be created manually. I granted Jane all permissions. (Pics 6 & 7)
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now to create users (customers), navigate to Agent Panel -> Users -> -> Add new. Add users, give them a name and email address, to enable them to submit and manage their tickets.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To configure SLA (Service Level Agreements) navigate to Admin Panel -> Manage -> SLA -> Add New. For the names use, Sev-A, Sev-B, and Sev-C, with Sev-A being the most sever and decreasing until Sev-C. 
My SLA's:
- Sev-A (Grace Period: 1 hour, Schedule: 24/7)
- Sev-B (Grace Period: 4 hours, Schedule: 24/7)
- Sev-C (Grace Period: 8 hours, Schedule: 24/5)
</p>
<br />

<p>
image 10
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To configure help topics for user ticket creation navigate to Admin Panel -> Manage -> Help Topics -> Add New Help Topic. These topics will be presented to users and help them categorize their tickets effectively. There is a permission that can be granted to support to recategorize tickets if done so incorrectly by the customer.
Help topics I created:
Image 11
</p>
<br />
