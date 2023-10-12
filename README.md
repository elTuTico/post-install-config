# post-install-config
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

- Configure the Roles 
- Configure the Departments
- Configure the Teams
- Allow any User to create tickets
- Configure Agents
- Configure Users
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

<p>
<img src="https://github.com/elTuTico/post-install-config/assets/137955237/a95f1b85-14c8-4357-b076-2c9ef223239f"/>
</p>
<p>
Login into osTicket interface with the credentials created while setting up the ticketing system. Once logged in remember that the initial page that opens up is the “Ticket” screen. From here moving between the “Admin” panel to the “Agent” panel using the options at the top right hand side of the page will be the means of setting up the ticketing team. The admin panel will be utilized as someone who actively sets up the ticketing system and defines the roles, SLA, and general administrative duties. While the agent panel is utilized as an employee at a help desk generally using the platform to solve tickets.
</p>
<br />

<p>
<img src="https://github.com/elTuTico/post-install-config/assets/137955237/a87a532d-88f1-48e5-8e05-bf51dc7645be"/>
</p>
<p>
Roles are permissions granted to Agents per Department that they have access. For this example the role “Supreme Admin” will be created with permissions to create or delete tickets and just about anything else. Within the “Admin” panel click the “Agents” tab, followed by the “Roles” tab, and then click “Add New Role”. 
</p>
<br />

<p>
<img src="https://github.com/elTuTico/post-install-config/assets/137955237/06d31188-80f1-4871-99c2-c70651d09243"/>
</p>
<p>
Name the role “Supreme Admin”. Grant this role all the permissions available under the “Permissions” tab. Click “Add Role” to finazlize the role. 
</p>
<br />

<p>
<img src="https://github.com/elTuTico/post-install-config/assets/137955237/8ae942de-645d-4978-85f4-263b4f94db45"/>
</p>
<p>
Departments are the manner in which tickets are routed to the correct section of the help desk to better suit the issue at hand. Within the “Admin” panel click the “Agents” tab, followed by “Departments”, and then click “Add New Department”. 
</p>
<br />

<p>
<img src="https://github.com/elTuTico/post-install-config/assets/137955237/52ccdc98-48ef-483f-9800-347ef7972c92"/>
</p>
<p>
Create a new top level department named “System Administrators” as a means of giving the Admin Supreme access to all kinds of tickets submitted by the Users. Leave all other settings in default and come back to them later to tinker with SLAs, Emails, and more. Click “Create Department” to save the new department. 
</p>
<br />

<p>
<img src="https://github.com/elTuTico/post-install-config/assets/137955237/713181a9-1bf1-4a97-bf70-bd7841f4d426"/>
</p>
<p>
Teams allows Agents to be utilized from different departments to handle and organize specific issues or users via help topics or tickets filters. To create a “Team” within the “Admin” panel click the “Agents” tab, followed by the “Teams” tab, and then click “Add New Team”. Name the new team “Level II Support”, click “Create Team”, and utilize this new support team as an all-star group of agents that can solve higher level tickets. 
</p>
<br />

<p>
<img src="https://github.com/elTuTico/post-install-config/assets/137955237/2f248d90-0b19-4883-bd65-2896a581ef3e"/>
</p>
<p>
Next, configure the system to allow anyone to create tickets, such as anonymous users. Within the “Admin” panel click the “Settings” tab, followed by the “Users” tab, and then ensure that the “Registration Required” box is unchecked. Save the changes.
</p>
<br />

<p>
<img src="https://github.com/elTuTico/post-install-config/assets/137955237/9fe511d5-4ab2-4a69-a017-71ee15ed80e3"/>
</p>
<p>
Once access to create tickets has been granted to anyone there must be help desk professionals that will be going through and checking/solving tickets through Agents created. Within the “Admin” panel click the “Agents” tab, followed by “Add New Agents”, and then make up to two new agents. Ensuring that the agent's passwords are not required to be reset upon logging in for the first time. Play around with the kind of “Access”, “Permissions”, “Teams”, and “Departments” available.
</p>
<br />

<p>
<img src="https://github.com/elTuTico/post-install-config/assets/137955237/6a35c3ad-15d6-4042-b44f-35b1c3a65c1f"/>
</p>
<p>
Users are essentially the customers or people who the Agents would be providing support to through the kinds of tickets for help they submit through osTicket. Within the “Agent” panel click the “Users” tab, followed by “Add User”, and then create up to two new users. 
</p>
<br />

<p>
<img src="https://github.com/elTuTico/post-install-config/assets/137955237/67fc3ebc-0f4d-4616-914f-9e8285a0cb12"/>
</p>
<p>
In osTicket SLAs are defined as time limit targets for how long the ticket is going to be open before the issue gets resolved by an agent. Within the “Admin” panel click the “Manage” tab, followed by “SLA”, and then click “Add New SLA Plan” to make up to three varying SLAs: Sev-A (1 hour within 24/7), Sev-B (4 hours within 24/), and Sev-C (8 hours within business hours). 
</p>
<br />

<p>
<img src="https://github.com/elTuTico/post-install-config/assets/137955237/447e3e5d-035b-4689-9efc-aa5759f83e06"/>
</p>
<p>
To finish off “Help Topics” that are used to streamline end users experience to ensure that proper assignments and prompt responses to tickets are done as issues arrise must be created. Within the “Admin” panel click the “Manage tab, followed by “Help Topics”, and then click “Add New Help Topic”. Create four common help topics like “Business Critical Outage”, “Personal Computer Issues”, “Equipment Request”, and “Password Reset” that users could use in the following step of this lab. 
</p>
<br />
