<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>

Following the successful installation of osTicket on your Windows 10 Azure Virtual Machine, this guide will walk you through the post-installation setup, focusing on configuring roles, departments, teams, user settings, agents, customers, SLAs, and help topics.
After this tutorial all accounts will be setup to create a simulated help desk environment!<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

<h3>Configure</h3>

- [Roles](https://docs.osticket.com/en/latest/Admin/Agents/Roles.html)
- [Departments](https://docs.osticket.com/en/latest/Admin/Agents/Departments.html)
- [Teams](https://docs.osticket.com/en/latest/Admin/Agents/Teams.html)
- [Agents(workers)](https://docs.osticket.com/en/latest/Admin/Agents/Agents.html)
- [Users (customers)](https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html)
- [SLA](https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html)
- [Help Topics](https://docs.osticket.com/en/latest/Admin/Manage/Help%20Topic.html)

<h2>Configuration Steps</h2>

#### **Configure Roles**

1. **Navigate to Admin Panel -> Agents -> Roles**
   - Create a new role named `Supreme Admin`.
   - Assign all possible permissions to ensure full control over the osTicket system.

#### **Configure Departments**

1. **Go to Admin Panel -> Agents -> Departments**
   - Add a new department named `System Administrators`.
   - Assign the `Supreme Admin` role to this department, ensuring they have the necessary permissions to manage the system effectively.

#### **Configure Teams**

1. **Access Admin Panel -> Agents -> Teams**
   - Create two teams: `Level I Support` and `Level II Support`.

#### **User Settings**

1. **Visit Admin Panel -> Settings -> User Settings**
   - Enable the option `Registration Required` to require registration and login for creating tickets.
   - This helps in tracking and managing tickets more effectively by associating them with specific users.

#### **Configure Agents (Workers)**

1. **Navigate to Admin Panel -> Agents -> Add New**
   - Create agents with the names `Richard` and `Dinesh`.
   - Assign them to the `System Administrators` department and the appropriate support level teams, depending on their expertise and role within the organization.

#### **Configure Users (Customers)**

1. **Head to Agent Panel -> Users -> Add New**
   - Add users `Monica` and `Gavin` as customers who will be creating tickets.
   - Input their contact information accurately to ensure they can be reached for any follow-ups or clarifications.

#### **Configure SLA**

1. **Proceed to Admin Panel -> Manage -> SLA**
   - Set up three SLA plans: `Sev-A`, `Sev-B`, and `Sev-C` with response times of 1 hour (24/7), 4 hours (24/7), and 8 hours (business hours), respectively.
   - These SLAs will help prioritize tickets and manage expectations regarding response times.

#### **Configure Help Topics**

1. **Go to Admin Panel -> Manage -> Help Topics**
   - Create help topics for common issues such as `Business Critical Outage`, `Personal Computer Issues`, `Equipment Request`, and `Password Reset`.
   - Assign these help topics to the relevant departments and SLAs to streamline the ticketing process and ensure that tickets are directed to the correct teams promptly.

### **Conclusion**

Congratulations! You have setup a simulated help desk environment. By following these steps, you will have configured the essential components of your osTicket system to align with your organization's support structure and workflow. This setup ensures that tickets are handled efficiently, with clear roles, responsibilities, and escalation paths. Remember, osTicket offers extensive customization options, so feel free to explore and adjust settings as necessary to best meet your needs.

I'll guide you through the next steps to [create common help desk tickets](https://github.com/d-lowes/osticket-ticket-lifecycle)!
