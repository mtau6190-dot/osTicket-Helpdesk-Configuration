<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket: Helpdesk Configuration</h1>
Post-installation setup of osTicket Helpdesk system, demonstrating configuration of roles, departments, teams, SLA policies, and help topics.<br />
<br>
<h2>Skills Demonstrated:</h2>

- Help Desk system deployment
- Role-based access control
- SLA Management
- User & Agent configuration

<h2>Steps:</h2>

- Step 1: How to Access Admin & Agent Panel
- Step 2: Key Configuration Steps



<h2>1. How to access Admin & Agent Panel</h2>

<img width="1033" height="623" alt="image" src="https://github.com/user-attachments/assets/c431dc0e-1618-4d7b-b748-c84341534f6a" />
<p>Logged in as the Admin User</p>
<img width="1342" height="475" alt="image" src="https://github.com/user-attachments/assets/34f53e1f-4448-4f05-83d8-0e5f941b8486" />
<p>The Agent Panel Dashboard</p>
<img width="1305" height="470" alt="image" src="https://github.com/user-attachments/assets/478fa869-5647-4f1a-b21b-67c92261f8f6" />
<p>The Admin Panel Dashboard</p>
<br>

<h3>1.1 Configuring Roles for Grouping Permissions</h3>

<img width="1191" height="426" alt="image" src="https://github.com/user-attachments/assets/dc971721-6ecc-4912-b50b-8ddc4e9d3586" />
<img width="1196" height="480" alt="image" src="https://github.com/user-attachments/assets/fb16b610-3f40-4284-9ce7-e199bdfd795c" />
<img width="836" height="615" alt="image" src="https://github.com/user-attachments/assets/3d3b0c4e-5998-49e6-b0d0-77f97c10c23f" />
<img width="633" height="598" alt="image" src="https://github.com/user-attachments/assets/437b6fa9-3c0b-4102-94eb-1eb49c022fb9" />
<img width="1193" height="553" alt="image" src="https://github.com/user-attachments/assets/b4e0e781-43bc-42ff-8bf9-65f0567894e5" />

<p>Super Admin: Created under *Admin Panel → Agents → Roles → Add New Role to establish a top-level role with unrestricted permissions, ensuring centralized control and clear separation from standard agent access.</p>

<h3>1.2 Configuring Departments</h3>

<img width="1196" height="411" alt="image" src="https://github.com/user-attachments/assets/611a3b5a-a15f-4369-a903-8cfac09b0f36" />
<img width="1191" height="490" alt="image" src="https://github.com/user-attachments/assets/4633a82b-1383-481d-a6bb-a8174b92c98f" />
<p>SysAdmins: Created under *Admin Panel → Agents → Departments* to organize ticket visibility and responsibilities, ensuring issues are routed to the right technical group.</p>


<h3>1.3 Configuring Teams</h3>
<img width="1197" height="371" alt="image" src="https://github.com/user-attachments/assets/1bc02cac-0adf-4a6d-894b-83d224e712a5" />
<img width="1192" height="410" alt="image" src="https://github.com/user-attachments/assets/3a6b8839-f8e2-492e-96bb-72165a13d12d" />

<p>Online Banking: Created under *Admin Panel → Agents → Teams* to bring together agents from different departments into a single working group.
  
  - **What:** A team is a cross‑department collection of agents who collaborate on specific ticket categories.  
  - **Why:** Teams improve flexibility by allowing agents with diverse skills to work jointly on specialized issues (e.g., online banking problems), ensuring faster resolution and better coverage than relying on a single department alone.</p>


<h3>1.4 Configuring Agents</h3>
<img width="1192" height="458" alt="image" src="https://github.com/user-attachments/assets/7e441122-5a13-4cd9-a02e-8f1f483babab" />
<img width="1195" height="497" alt="image" src="https://github.com/user-attachments/assets/24f91e35-1ee0-471d-b265-e256064a7b78" />

- Jane (Dept: SysAdmins)** and John (Dept: Support): Added under *Admin Panel → Agents → Add New* to define the staff responsible for handling tickets.  
  - What: Agents are the helpdesk workers who log in to the system, view assigned tickets, and resolve user issues. Each agent is linked to a department or team to control ticket visibility and responsibilities.  
  - Why:Configuring agents ensures that support requests are routed to the right people. It establishes accountability, organizes workload distribution, and mirrors real-world IT support operations where staff are assigned based on expertise.
 
<h3>1.5 Configuring Users(Customers) in Agent Panel</h3>
<img width="1201" height="535" alt="image" src="https://github.com/user-attachments/assets/d042b5cf-fac1-4c2d-bbef-47d2724e58d3" />
<img width="1192" height="462" alt="image" src="https://github.com/user-attachments/assets/d2f266c0-07d3-4433-8bfa-ab5c36a39451" />

<p>
Karen Colman: Added under Agent Panel → Users → Add New to represent registered customers in the system. 
  
  - What: A “User” in osTicket is a defined customer profile with stored contact details, ticket history, and association to specific issues.  
  - Why: Unlike anonymous ticket creators, registered users provide continuity and accountability. Their tickets can be tracked over time, linked to past requests, and managed more effectively. This improves customer support quality by giving agents context about the user’s history and needs.
</p>

<h3>1.6 Configuring Service-Level Agreements (SLA)</h3>
<img width="1192" height="377" alt="image" src="https://github.com/user-attachments/assets/455faca9-81ee-4b80-858c-51b630045ee9" />
<img width="1191" height="531" alt="image" src="https://github.com/user-attachments/assets/3885936f-1ae8-421d-b7c7-4f483cd6520f" />

<p>
- *ev-A (1 hour, 24/7)**, **Sev-B (4 hours, 24/7)**, **Sev-C (8 hours, Business Hours)**: Configured under *Admin Panel → Manage → SLA* to define response and resolution timelines.  
  - **What:** SLAs set rules for how quickly tickets must be acknowledged and resolved based on severity. Each SLA includes a grace period (time allowed before escalation) and a schedule (24/7 or business hours).  
  - **Why:** SLAs ensure accountability and consistency in support operations. They help prioritize critical issues (e.g., outages) over routine requests, align IT support with business needs, and provide measurable performance standards.  
  - **Value:** By enforcing SLAs, organizations can track compliance, improve customer satisfaction, and demonstrate reliability in handling support requests.
</p>




