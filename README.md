<h1>Active Directory Home Lab</h1>

<h2>Description</h2>
Built and managed a virtualized Active Directory environment using Windows Server and Windows 10 to develop hands-on experience with domain administration and enterprise IT support. Configured domain services, Organizational Units (OUs), Group Policy Objects (GPOs), user authentication, password policies, and Role-Based Access Control (RBAC). Joined client machines to the domain and troubleshot DNS resolution, domain connectivity, and authentication issues to strengthen Windows administration and troubleshooting skills.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Operating Systems: Windows Server, Windows 10</b> 
- <b>Directory Services: Active Directory Domain Services (AD DS)</b> 
- <b>Administration Tools: Active Directory Users and Computers (ADUC), Group Policy Management Console (GPMC)</b> 
- <b>Networking: DNS, DHCP, TCP/IP</b> 
- <b>Virtualization: Oracle VirtualBox</b> 
- <b>Security: Group Policy Objects (GPOs), Role-Based Access Control (RBAC), password policies, user authentication</b> 

<h2>Program walk-through:</h2>

<p align="center">
Created a Nat server and made sure all of the machines were in that network:  <br/>
<img src="https://imgur.com/e4BrRzS" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Configuring active directory to the windows server 2022 and changing the network to 192.168.10.7: <br/>
<img src="https://i.imgur.com/La1gc60.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Installing Active Directory for Windows server:  <br/>
<img src="https://i.imgur.com/aeBEv5t.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Then we go on to put the server as the Domain Controller for Active Directory:  <br/>
<img src="https://i.imgur.com/DuG4fy6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Upon logging in as the domain controller, we created a new users and a new organizational unit and labeled them to put the  new user in them:  <br/>
<img src="https://i.imgur.com/hKgoXWm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Assigning appropriate permission for user:  <br/>
<img src="https://i.imgur.com/YBad56P.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Moving on to the target machine (Windows 10), we wanted to join the server that had the active directory. To do this we changed our DNS server to 192.168.10.7 to point to the Windows server and then joined by changing the domain on the windows machine to the name we put in the windows server:  <br/>
<img src="https://i.imgur.com/4sywyPw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>
<img src="https://i.imgur.com/5jW93dg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
After we restarted the windows machine, we can now log in to the user that we created. In this case, I logged in to Jsmith which was one of the user I created in the windows server with active directory:  <br/>
<img src="https://i.imgur.com/5uNoO54.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
