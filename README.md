<p align="center">
<img src="https://github.com/user-attachments/assets/43223766-5f00-47f6-bd49-4026ba2644a6"/>
</p>

<h1>Troubleshooting Account Lockouts in Microsoft Azure Virtual Machine with HeidiSQL</h1>
This article describes how to implement an on-premises issue on Azure Virtual Machines and includes a real-world debugging example using HeidiSQL.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- osTicket
- HeidiSQL

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Open HeidiSQL
- Create a Script to Change Admin's passwords
- Manually change Agent's passwords

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://github.com/user-attachments/assets/9cc56003-0803-47c8-958b-7b5991f7109f"/>
</p>
<p>
During the osTicket Project, I had an issue in which I was fully locked out of all of my accounts, including the admin account. To resolve this, I had to enter MySQL and run code under "Query" to change my admin password.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/fbd73c85-dfbf-4adc-b746-dd76819d70c3"/>
</p>
<p>
Lastly, I went into the "ost_staff" table to update the Agent's passwords' manually. This can be done by double clicking the "passwd" field. The password entered is encrypted and translates to "welcome".
</p>
<br />

