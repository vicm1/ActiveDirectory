Installing Active Directory with Windows Server on a Virtual Machine
Requirements:
Using VMWare Workstation PRO
Windows Server 22

How to install Active Directory w/ Windows Server on a Virtual Machine

Make sure its Workstation pro 17 cause the previous versions don’t contain Window Server 2022 which will be used for this.
Click on Create a new virtual machine to set up a new virtual machine.

Choose Typical configuration
Install the operating system you want to use. We’re
	Using windows. I will install it later to minimize the
	errors.

Select Windows Server 2022, since its the server
We’re going to be using.



Choose how storage is going to be allocated to this specific virtual machine: Depends on how much a user will need. I allocated 20 GB. The recommended is 60 GB.


Shows the settings that are going to be used to create the Virtual Machine




Virtual Machine using Windows Server 2022 is now created. Shows the specifications of the virtual machine. 
Still have to add the Operating System, if not added when creating the virtual machine earlier.

Right click on the newly created virtual machine, called Windows Server 2022, under the My Computer tab located on your library. 

A popup will appear showing the virtual machine settings, here go to CD/DVD (SATA) option and install where the user has the location of the operating system that they’re going to use. Mine is an ISO image file that I got from the windows website, so I choose browse on my downloads and click on the OS ISO file. Click on ok when the proper OS is chosen. 


Click on Power on this virtual machine. When booting up press a key quickly to load the ISO. If user misses the key press they will receive a Timeout showing just EFI Network… Press CTRL + ALT to get out of the Virtual Machine and right click on Windows Server 2022 again but this time power off the machine under power options and restart the machine, it’ll boot up again to press the key quick. 

This will show up, choose Windows Setup [EMS Enabled]

If successful the Microsoft Server OS Setup should show. 

Click Next and then Install now.


Choose the Windows Server 2022 Standard Evaluation (Desktop Experience) because this one comes with a GUI and the other one comes with just the command line.

Click on Next, then Next again but first accept the Microsoft Software License Terms.

Choose Custom Installation. Then next page choose Drive 0 and it should show how much storage (GB) the user allocated earlier. Mines 20 GB since I allocated 20GB. After clicking Next with Drive 0 checked it should start installing the OS.



Window Server 2022 should now be installed. Next we have to do Customizs Settings. 

Make your own credentials for the Administrator.

 Now user has their own Administrator account. Log in with the credentials.



Server Manager will show up for the first time. Only used by Windows Server. 

Go to ActiveDirectorySteps.MD for steps on how to install and use Active Directory.

