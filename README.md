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

1. Access Panels


Log into the Admin/Analyst Panel (/scp/login.php)


Access the End User Portal (/osTicket)


Understand the difference between Agent Panel vs Admin Panel


2. Define Roles & Permissions


Create Roles (e.g., Supreme Admin) to group permissions


Assign appropriate privileges to each role


3. Organize Departments & Teams


Configure Departments for ticket visibility (e.g., SysAdmins, Support)


Create Teams by pulling agents across departments (e.g., Online Banking)


4. Set User Access Rules


Control ticket creation:


Allow anyone to create tickets OR


Require registration/login for ticket creation


5. Add Agents (Helpdesk Staff)


Create new Agents and assign them to departments


Example: Jane (SysAdmins), John (Support)


6. Add Users (Customers)


Create End Users who will submit tickets


Example: Karen, Ken


7. Configure SLA Plans


Define service level agreements (response/resolution times)


Example:


Sev-A: 1 hr, 24/7


Sev-B: 4 hrs, 24/7


Sev-C: 8 hrs, Business Hours


8. Create Help Topics


Define categories for incoming tickets (helps routing & prioritization)


Examples: Business Critical Outage, Password Reset, Equipment Request, Personal Computer Issues, Other

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 1 – Access osTicket Panels

Admin/Analyst Login Page:
http://localhost/osTicket/scp/login.php

End User Portal:
http://localhost/osTicket

Understand the difference:

Agent Panel → Used by helpdesk staff (agents).

Admin Panel → Used for configuring osTicket (settings, permissions, etc.).
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 2 – Configure Access and Organization

Roles (grouping permissions):

Admin Panel → Agents → Roles

Create Supreme Admin.

Departments (ticket visibility):

Admin Panel → Agents → Departments

Create SysAdmins.

Teams (cross-department groups):

Admin Panel → Agents → Teams

Example team: Online Banking.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 3 – User & Agent Setup

Allow or restrict ticket creation:

Admin Panel → Settings → User Settings

Uncheck “Unregistered users can create tickets” → Require login.

Agents (staff):

Admin Panel → Agents → Add New

Example: Jane (Dept: SysAdmins), John (Dept: Support).

Users (customers):

Agent Panel → Users → Add New

Example: Karen, Ken.
</p>
<br />
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 4 – Configure SLAs and Help Topics

SLA Plans:

Admin Panel → Manage → SLA

Examples:

Sev-A: 1 hour, 24/7

Sev-B: 4 hours, 24/7

Sev-C: 8 hours, Business Hours

Help Topics (categories for tickets):

Admin Panel → Manage → Help Topics

Add: Business Critical Outage, Personal Computer Issues, Equipment Request, Password Reset, Other.
</p>
<br />
