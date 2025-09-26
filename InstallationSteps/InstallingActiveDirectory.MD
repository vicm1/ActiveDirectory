Use Active Directory with Windows Server 2022 using VMWare.

Go to the top right, where it says manage and click on add Roles and Features
Make sure in Installation type tab you choose Role-based or feature-based installation. Click next. It’ll take you to Server Selection and click on the only computer found. Then next.


It’ll take the user to the next tab about Server Roles to add Roles. Check Active Directory Domain Services and Remote Access. The ones we’re going to need for now. Click Next.
In the Features tab, make sure to have Group Policy Management is checked, only one we need for this tutorial.
Click next until you reach Role Services, and then check Direct Access and VPN, Routing, and Web Application Proxy.

After just keep on clicking next, it’ll just show you tabs of what Roles you’re choosing to install until you get to Confirmation

Confirmation shows you everything that will be installed, Roles, and Features on the selected server. Click install.

Important step. Click on promote this server to a domain controller since we don’t have a domain controller yet; this will become it.


Make sure to click on Add a new forest (since it’s the main domain), then add the Root Domain name as you wish, but make sure it has .local at the end of it, or AD won’t allow it.
Add the most recent Forest and Domain functional level, should be Windows Server 2016. Add a password.

Just keep on clicking on next until user reaches the Prerequisite Check, which should show that everything is ok, and when passed user can click on install. When the installation finishes, it has to reboot the server/computer because new changes were made to the Windows Server. Just wait a moment for the reboot to commence.


If Active Directory is installed correctly, then when reboote,d the user will be prompted to this signin showing it as Administrator with the forest domain name that was chosen


This is how the dashboard should look now. Notice that the Roles and Server Groups section added the roles we checked.

Now the user should have a Windows Server Active Directory running on the Virtual Machines.
