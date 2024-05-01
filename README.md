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
