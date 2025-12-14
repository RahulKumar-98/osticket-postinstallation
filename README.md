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

- Windows 10</b> (22H2)

<h2>Configuration Steps</h2>

<p>
<img width="1244" height="517" alt="1" src="https://github.com/user-attachments/assets/9fc6b581-0626-4bff-97ba-b4605acdc72b" />
</p>
<p>
Now that OsTicket has been installed, we can proceed with our post-installation setup and configuration. First, we will log in as Admin and assign roles across various departments/ teams, managing each user's access respectively.

-  To Log in as Admin/ Agent: http://localhost/osTicket/scp/login.php
-  To Log in as an End User: http://localhost/osTicket
</p>
<br />

<p>
<img width="956" height="216" alt="2" src="https://github.com/user-attachments/assets/6f0b0b58-c8e8-4ba8-81e9-92b441d82f80" />
<img width="951" height="708" alt="3" src="https://github.com/user-attachments/assets/02ef776c-fbf8-4f0a-b3bc-087fba66f382" />
</p>
<p>
click on "Admin Panel" on the top right after logging in as the Admin. This will allow us to configure and assign user permissions and roles as the Admin, whereas the Agent will be the Helpdesk worker. We will proceed by setting up a "Supreme Admin" role on our help desk. First we will navigate to the Agent tab -> Roles -> Click on "Add New Role". Here we will name the role "Supreme Admin" and grant all permissions in the Permissions Tab located next to the "Definition Tab".
</p>
<br />

<img width="964" height="1108" alt="image" src="https://github.com/user-attachments/assets/e9aff945-2f67-44a6-8f72-4e7ea1f9525c" />
<p>
Next we will configure departments in our Helpdesk. This is significant for providing various levels of access for departments, i.e SysAdmin ticket visibility or department specific inquiries (Dependant upon company structure and delegation of responsibilities). First, we will click on the "Departments" tab under Agent -> Add New Department -> Name Department and configure department settings/ access based on your preferences. Then we will create the department.
</p>
<br />

<img width="977" height="675" alt="5" src="https://github.com/user-attachments/assets/9e83495f-f822-4e3e-833e-e51ea04c19d3" />
<p>
Now we will create a new Team, under the Agents tab we will click on Teams -> "Add new Teams" -> Then we will create the Team. Here we may create teams dependant upon a specific task or responsibility, i.e Online Banking Team or Maintenance Team.
</p>
<br />
<img width="965" height="685" alt="7" src="https://github.com/user-attachments/assets/b9fcfd60-a3c0-42b6-a0c5-ff6ebe47d349" />

<p>
Now that we've created our relevant teams, we can proceed with the ticket creation process and configure access settings to allow any User to create a ticket without registration, on our Helpdesk server. To do this, we will click on Settings tab within the Admin Panel -> Click on Users -> Uncheck where it says "Require registration and login to create tickets".
</p>
<br />

<img width="964" height="956" alt="8" src="https://github.com/user-attachments/assets/beec8fdb-9fa9-4ea2-9cb8-cd6f52bc5e35" />

<p>
Next we will configure agents in our Helpdesk. click on Agents within the Admin Panel still -> Click on Agent (next to Teams)  -> Click Add New Agent. Here we can add the Agent's contact information, set up their username or password, and lock/ unlock their account.
</p>
<br />

<img width="964" height="1108" alt="image" src="https://github.com/user-attachments/assets/e9aff945-2f67-44a6-8f72-4e7ea1f9525c" />
<p>
Next we will configure agents in our Helpdesk. click on Agents within the Admin Panel still -> Click on Agent (next to Teams)  -> Click Add New Agent. Here we can add the Agent's contact information, set up their username or password, assign a department or permissions, add them to a team, and lock/ unlock their account.
</p>
<br />

<img width="963" height="234" alt="9" src="https://github.com/user-attachments/assets/a46d8418-c44a-4fa4-ac2b-18587a617583" />

<p>
Next we will configure end-users on our Helpdesk. This will allow us to create end-users (Customers) who will be able to utilize our Helpdesk platform. Click on Users (under the Agent Panel) -> Click on "Add Users" -> Enter User credentials.
</p>
<br />

<img width="962" height="384" alt="10" src="https://github.com/user-attachments/assets/730d7f8d-40b4-4bfe-ab32-4f89fd7407ee" />

<p>
Now we will congifure SLAs. Setting the appropriate SLA based on ticket severity is extremely important in the delegation of tasks within a Helpdesk platform like OsTicket. To get started, first we will go back to the Admin Panel -> Click on the Manage Tab -> Click on SLA ->  "Add New SLA Plan".
</p>
<br />

<img width="959" height="666" alt="11" src="https://github.com/user-attachments/assets/27a8b2ef-1a69-4cb3-8607-310674feee56" />

<p>
Here we can set various Service Level Agreements (SLA) dependant upon the ticket's severity and priority level. In the above, Sev-A would be considered a top-priority ticket. Ex: CEO's laptop has been hacked or the sales team is unable to access their laptops. We can set a grace period of how many hours we would expect to be needed for the ticket to be resolved. We can also set the schedule for this type of SLA, having it run on a 24/7 schedule, 24/5 schedule, or an 8-5pm Business hours including business holidays schedule.
</p>
<br />
<img width="958" height="632" alt="12" src="https://github.com/user-attachments/assets/13496848-2f27-4b1d-8dab-aaa5f2a7de29" />

<p>
Lastly, we can incorporate "Help Topics" onto our ticketing platform. To do this. We will click on "Manage" (in the Admin Panel) -> click on "Help Topics" -> then click on "Add New Help Topic". Here we can create help topics such as Internet Connectivity Issues, Password Outages, or General Inquiry topics for users to reference. You can also set a "Parent Topic" for the Help Topic being created. That being said, this concludes the OsTicket post-installation configuration guide.
</p>
<br />

<p>
Next we will configure departments in our Helpdesk. This is significant for providing various levels of access for users, depending on the department they are assigned, i.e SysAdmin ticket visibility or Bank Group (Dependant upon company structure and SLA responsibility). First, we will click on the "Departments" tab under Agent -> Add New Department -> Name Department and configure department settings/ access based on your preferences. Then we will create the department.
</p>
<br />
