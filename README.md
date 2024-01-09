# Azure-AD-Connect
Synchronization methods with Azure AD Connect
Use Sentinel. Run Failed Login Attempt Query. Turn on Fusion Machine Learning.

<h2>Description</h2>
The tool used to configure directory synchronization is called Azure AD Connect. Azure AD Connect consists of, or can leverage, the following components:
1. Synchronization services
2. Active Directory Federation Services (AD FS)
3. Health Monitoring

<p>Azure AD Connect supports multiple AD forests and multiple Exchange organizations to a single Microsoft 365 tenant. It synchronizes users, groups, and contact objects from your
on-premises AD to Microsoft 365.<br />
There are some writeback capabilities that can be leveraged if chosen or required, which will allow attributes from passwords and groups set in Microsoft 365 to be
written back to an on-premises AD.<br />
The principles of Azure AD Connect are shown in the following diagram:<br />
<img src="1.png" height="50%" width="50%" />
<br />
<p> Express Settings: default setting for Azure AD Connect and is designed for use with password hash synchronization from a single AD forest. <br /></p>
<img src="Express.png" height="50%" width="50%" />
<br />
<p>Custom Settings: With the custom settings installation, you are provided with the following options to extend your on-premises identities in the cloud using Azure AD
Connect. </p><br />
<img src="Custom.png" height="50%" width="50%" /> <br />



</p>
<br />


<h2>Environments Used </h2>
- <b>Microsoft Azure Sentinel Portal </b>

<h2>Prerequisites</h2>

-<b> Password Lockout Settings modified by anyone assigned the following roles:
 - Log Analytics Contributor
 - Log Analytics Reader
 - Global Administrator
 </b>
- <b> Licenses:  Azure AD trial or Premium P1 or higher licenses </b>

<h2>Program walk-through:</h2>

<h3>Steps: </h3>
1. Steps:
1.	Go to Azure portal --> Azure Sentinel
2.	Select 	Azure Sentinel Workspace
3.	Select Hunting --> select Query ‘Failed login attempt’ --> Run Query
4.	Go to Analytics section --> select active rule --> edit
5.	Enable status of rule --> Configure it
6.	Review & Save

<h3>Screenshots:</h3>

<p align="center">
Select Log Workspace Analytics:  <br/>
<img src="select log workspace analytics.png" height="50%" width="50%" />
<br />
<br />
Select Query:  <br/>
<img src="query.png" height="50%" width="50%" />
<br />
<br />
Active Rules of Query: <br/>
<img src="active rules.png" height="50%" width="50%"/>
<br />
<br />
Enable Status: <br/>
<img src="enable status of rule.png" height="65%" width="50%"/>
<br />
<br />
Result: <br/>
<img src="result.png" height="65%" width="50%"/>
<br />
<br />


</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
