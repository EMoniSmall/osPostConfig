# Post Installation Setup for osTicket 🦘

> [!Important]
> This is a continuation for the installation of osTicket. In this guide we'll be configuring roles, departments, teams as well as the settings for tickets. In order to continue with this guide, you must have a basic installation of osTicket on your system. For assistance in setting this up, please refer to my guide for [osTicket Installation](https://github.com/EMoniSmall/osInstall).
>
> Once your osTicket system is installed and ready to go, log into osTicket via the [Login Page](http://localhost/osTicket/scp/login.php) using the credentials you've chosen in the previous guide.

> [!Note]
> You'll notice on the top right, there is a link called the "Admin Panel." You're currently on the "Agent Panel." By clicking this, you'll swap to the the admin panel and the link will change to "Agent Panel."
> 
>![mstsc_yxyocaMdmg](https://github.com/EMoniSmall/osPostConfig/assets/166156618/c3d721af-602f-4be6-89c1-b9a4eb25f4fc)
> 
> ![mstsc_HCQhU8HLEg](https://github.com/EMoniSmall/osPostConfig/assets/166156618/2c3cca63-e975-4b03-8bdd-3642843ffc4f)
>
> The Admin Panel will allow you to configure everything within osTicket while the Agent Panel is where you will handle live tickets as a normal user. 

<h2>Configuring Roles</h2>

> [!Note]
> As noted by osTicket:
> "Roles are the permissions granted to Agents per Department that they have access to. Each Role has a set of permissions that can be checked/unchecked for agents given that role in association with a department thay have access to. An unlimited number of roles can be created and assigned to agents with access to various departments." 

> [!Tip]
> Make sure you're on the Admin Panel for this portion. We'll be making a Super Admin with all of the permissions

Step 1: Click Agents 

Step 2: Click Roles

Step 3: Click Add New Role and name your role

Step 4: Add all permissions + Add Role

![mstsc_eMTRHC0gsr](https://github.com/EMoniSmall/osPostConfig/assets/166156618/bb58e31d-d463-43e4-8f4b-dc1b3a9805fe)

<h2>Configuring Departments</h2>

> [!Note]
>  Tickets are routed to different departments depending on their Type, SLA or Service Level Agreement, schedule and more. This keeps the Ticketing system more organized and routes the tickets to the most relevant agents.

Step 1: Click Agents 

Step 2: Click Departments

Step 3: Click Add New Department and Name the Department what you wish. In this example we'll be naming it System Admins. 
Default settings are fine until you're ready to play with the other settings.

![mstsc_4BWAlrYgUp](https://github.com/EMoniSmall/osPostConfig/assets/166156618/640ab849-f4f5-4aff-8b55-9f3a90d63596)

<h2> Configuring Teams</h2>

> [!Note]
> As Noted by osTicket:
> "Teams allow you to pull agents from different Departments and organize them to handle a specific issue or user via a Help or Ticket Filter."
>
> "Having Agents from different Departments assigned to a Team will supersede the parameters of the Agents' Department Rules For Example, you can create a Help Topic Associated with a particular product you produce, and assign it to a Team of specialist Agents from different Departments."

Step 1: Click Agents

Step 2: Click Teams

Step 3: Click Add New Team and name the team whatever you wish. 

Step 4 (Optional): Add yourself as a member under Members. 

![mstsc_yIpRVzEfdz](https://github.com/EMoniSmall/osPostConfig/assets/166156618/2a40d348-e03d-4704-8923-d5f0fa77a94b)

<h2>Allowing Everyone to Create Tickets</h2>

Step 1: Click Settings 

Step 2: Click Users

Step 3: Under Authentication Settings, make sure Registration Required is Unchecked. 

![mstsc_rKwN2BAr97](https://github.com/EMoniSmall/osPostConfig/assets/166156618/a282a695-1d1c-4d11-8d98-cc79272ad6c2)

<h2>Configuring Agents</h2>

> [!Note]
> Agents are the actual Help Desk people that go through the tickets and solve the issues.
> 
> As Noted by osTicket:
> "Agents are given access to the help desk with the intent to respond and resolves the tickets. When adding an Agent to the help desk, they will need to be assigned to a Primary Department and given a Primary Role for the Tickets/Tasks routed to that department. Agents can be given Extended Access to additional departments of the help desk as well as assigned different Roles to those departments; this can be configured in the Access tab of the Agent's Profile." 

Step 1: Click Agents 

Step 2: Add New Agent. You'll be creating a few new Agents. In this example, they will be Jane and John. 

Step 3: Add Some credentials for both Agents.

> [!Tip]
> When setting the the Agent's Password, be sure to <b>uncheck</b> "Send the agent a password reset email" and "Require password change at next login." It will not be needed at this time. 

Step 3: Click Set

Step 4: Click Access

Step 5: Make one agent part of the Admins Department you created earlier as well as the team you've created. 

Step 6: Create Account.

> [!Important]
> We'll be making the 2nd agent a normal agent and not an Admin. Place them in the Support Department/View Only rather than the Admin Department.


<h2> Configuring Users</h2>

> [!Note]
> As Noted by osTicket:
> "Users are the owners of the tickets in the help desk. When a ticket is created in the help desk, the user is associated with their email address in the User Directory of the help desk, Users can be added or deleted from the User directory of the help desk at any time. Please note , if the user is deleted the tickets of the user must also be deleted." 

> [!Tip]
> Be sure that you're in the Agent Panel this time. We'll be creating two users, Karen Karen and Ken Ken.

Step 1: Click Users

Step 2: Add User and enter their email and Full name. 

Step 3: Click Add.

![mstsc_viJNvpXlz3](https://github.com/EMoniSmall/osPostConfig/assets/166156618/22bffd4e-607b-47c4-9c7a-939f01cd8f09)

<h2>Configuring SLAs </h2>

> [!Note]
> As noted by osSticket:
>
> "SLA Plans or Service Level Adreements, are unlimited in osTicket. The purpose of the SLA Plan is to provide a length of time in which the help desk Administrator expects tickets to be closed."
>
> It is essentially a time limit of how long a ticket can be left open.

> [!Tip]
> Be sure you're back on the Admin Panel for this. We'll be creating 3 different SLAs:
> 
> Sev-A (1 hour, 24/7)
> 
> Sev-B (4 hours , 24/7)
>
> Sev-C (8 hours, business hours)


Step 1: Click Manage > SLA

Step 2: Add New SLA Plan

Step 3: Name the SLA Plan and set the Grace period and Schedule to match the above Tip.

Step 4: Repeat til all 3 SLA Plans are created. 

![mstsc_LRJUqviXdV](https://github.com/EMoniSmall/osPostConfig/assets/166156618/8460267d-783e-44fb-b0d9-7674c04ac59b)

<h2>Configuring Help Topics</h2>

> [!Note]
> As Noted by osTicket:
>
> Help Topics will help streamline your end-user's help desk experience to ensure proper assignment and prompt response to the ticket. Create as many Help Topics as needed and can even nest Help Topics within each other for futher breakdown (For example, Human Resourves and Human Resouces/Payroll.)
>
> This basically allows users to add more detail to their tickets to ensure it reaches the correct agents for solving.

> [!Tip]
> We'll be creating 4 Different Help Topics.

Step 1: Click Manage. You'll notice there are already some default Help Topics.

Step 2: Add New Help Topic. Create a Business Critical Outage topic. Add Topic.

Step 3: Add New Help Topic. Create a Personal Computer Issues topic. Add Topic.

Step 4: Add New Help Topic. Create an Equiment Request topic. Add Topic.

Step 5: Add New Help Topic. Creat a Password Reset topic. Add Topic.

> [!Note]
> It is possible for users to fill out forms and/or send emails and tickets will automatically be created for them

![mstsc_MFsB03UfRY](https://github.com/EMoniSmall/osPostConfig/assets/166156618/a12cca09-4d84-45b3-8bc1-7accc637d7a4)

<b> This concludes the basic configuration for osTicket! </b>
