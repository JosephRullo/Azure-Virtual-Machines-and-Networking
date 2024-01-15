<p align="center">
<img src="https://i.imgur.com/zVU5h9m.png" height=100% width=100% alt="Microsoft Active Directory Logo"/>
</p>

<h1> <p align="center"> Virtual Machine Creation in Microsoft's Cloud Platform Azure</h1>
<p align="center"> This tutorial outlines the basics of implementing and deploying a Virtual Machine and gaining access to it with a remote client.<br />
<br />
<br />
<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remmina Remote Desktop Client
- RDP Protocol

<h2>Operating Systems Used </h2>

- Linux (Ubuntu)
- Windows 10 (21H2)

<h2>What is a Virtual Machine?</h2>
A virtual machine (VM) is a virtual environment that functions as a virtual computer system with its own CPU, memory, network interface, and storage, created on a physical hardware system (located off- or on-premises). This digital version of a physical computer can run programs and operating systems, store data, connect to networks, and do other computing functions, and requires maintenance such as updates and system monitoring. 
<br>
<h2>Deployment and Configuration Steps</h2>
<p>
<p>
<h2>Step 1.</h2> 
  
**Microsoft Azure.** 
<p>
To begin visit (www.portal.azure.com) -> create an account -> sign in. 
<p>
<p> 
<img src="https://i.imgur.com/N0pZPVG.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
<h2>Step 2.</h2> 
  
**Create Virtual Machine.** 
<p>
Once signed in, you will be brought to the Azure homepage. From here, click on the "Virtual Machines" tab at the top of the screen -> click "Create" -> select "Azure virtual machine".
<p>
<p> 
<img src="https://i.imgur.com/GpxuA3K.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/SeP4Jqo.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/LMYpPnc.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
<h2>Step 3.</h2> 
  
**Virtual Machine Configuration Basics.** 
<p>
Now we will setup what type of VM we want to create. We'll begin in the "Basics" tab and choose a few key components, leaving the others default. We must begin first by creating a "Resource Group" to store the VM and it's resources inside of. Under "Resource Group" click "Create New" and assign it a name. Next, give your VM a name and select the "Region" you would like it to be located and function in.
<p>
<p> 
<img src="https://i.imgur.com/5EG11W2.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/6nKu7mf.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
<h2>Step 4.</h2> 

**Virtual Machine Configuration Basics (continued).** 
<p>
Next scroll down to select the "Image" or Operating System that the VM will run, in this case Windows 10 is being selected. Now go down to "Size", this determine how many virtual CPU's (Central Processing Unit) it will run and the amount of RAM (Random Access Memory) for the VM. Note you'll want to choose the appropriate "Size" for what tasks you'll be performing on the VM. Too slow of a choice and you will have a hard time getting work done with resource demanding applications; too fast a choice and you'll be wasting resources and money since this comes at a premium price. Next, scroll down and assign a "Username" and "Password" (be sure to store them in a secure place in case you forget them). Finally check the box under "Licensing" and click "Next" on the bottom.
<p>
<p> 
<img src="https://i.imgur.com/4GlNFoN.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/xAJXroj.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/uohlSle.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
<h2>Step 5.</h2> 

**Virtual Machine Configuration Disks.** 
<p>
On the "Disks" settings tab, you will choose the size of the "Disk Drive" which will determine the amount of storage on the VM. You can also choose what type of disk drive which will determine the speed at which it accesses the data stored on it. In this case the defaults are set with 127Gb of storage on a SSD (Solid State Drive) disk (a faster option compared to a HDD or Hard Disk Drive). After selecting click "Next".
<p>
<p> 
<img src="https://i.imgur.com/IWOvzWr.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
<h2>Step 6.</h2> 

**Virtual Machine Configuration Networking.** 
<p>
On the "Networking" settings tab we will leave the default settings. Take note that a "Virtual Network", "Subnet" and "Public IP" are automatically created for you here. The rest of the configuration settings will be left on default for this basic tutorial as we have what we need to get the VM up and running. Click "Review + Create" on the bottom left to proceed.
<p>
<p> 
<img src="https://i.imgur.com/JLDKGGk.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
<h2>Step 7.</h2> 

**Validation and Deployment.** 
<p>
Now the VM is in the "Validation Process". If there is something incompatible with your selections, then an error message will pop up saying that "Validation failed. Required information is missing or not valid." and will point you towards the problematic section(s). Once Validation has passed, you can review the setup you've created and will be able to preview the price for your virtual machine. You can now finalize the creation of the VM and "Deploy" it by clicking the "Create" button on the bottom left of the screen. You can see on the next screen the "Resources" being built as the Deployment is in progress. Once finished click on "Go to resource"
<p>
<p> 
<img src="https://i.imgur.com/pLINIK7.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/mfbEspq.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/RCT5kGI.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
<h2>Step 8.</h2> 

**Virtual Machine Overview.** 
<p>
You will now be brought to the VM Overview page where you can view all the specs of the system as well as make further configuration changes. For now all we will copy is the "Public IP Address" so we can log on to the VM for the first time.
<p>
<p> 
<img src="https://i.imgur.com/Pqm3MrV.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
<h2>Step 9.</h2> 

**Remote Client.** 
<p>
In order to logon to the VM (which is located in Microsoft's cloud sever), we will need to use a "Remote Client". Since I'm using a Linux operating system, I will download and install "Remmenia Remote Desktop Client" to connect. However, if you are using a Window's or Apple host computer, you would use Microsoft's "Remote Desktop" which is built into Windows and can be downloaded on Mac. After opening your "Remote Client" type the "Public IP Address" for the VM that you copied on the Overview page. Enter the "Username" and "Password" you assigned to it and connect.
<p>
<p> 
<img src="https://i.imgur.com/YirLGAc.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/9dfLhjl.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/N7Cmz45.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
<h2>Step 10.</h2> 

**Test VM.** 
<p>
A new window will open on your host computer, inside of which is your fully functional Virtual Machine running it's own operating system you setup for it. Explore inside of it. Open up the file explorer and note the Drives and Network are just as you set up. If you go on the web browser you can visit (www.whatsmyipaddress.com) where you'll see not your host's IP but the location and IP of the VM. Feel free to use the VM as you would any PC for work or other projects. **Note** you can minimize the "Remote Client" window at any time to return to your "Host" computer. 
<p>
<p> 
<img src="https://i.imgur.com/pYLuFgR.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/tCVNNDz.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/HXFW2d5.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
<h2>Step 11.</h2> 

**Delete Resource Group (optional).** 
<p>
You must keep in mind you are being charged money for using Microsoft Azure's resources. You will continue to be charged while the "Resource Group" you created contains the VM and it's resources inside it. You can choose to delete it at any time to stop these charges from increasing. This is an important step if you are just using the Virtual Machine for a simple project and will not be needing it or it's resources on a long term basis. However, if you are using it as a necessity for business or work, you can leave it and access it remotely at any time. To delete the "Resource Group" and all of it's components, go to the Azure homepage -> select the "Resource Groups" tab -> click on the resource group highlighted in blue (you will notice two groups were created for the VM, delete them both one at a time) -> click on "Delete resource group" -> copy the resource group name -> paste at the bottom -> click on "Delete" -> repeat this for the other group created. All done.
<p>
<p> 
<img src="https://i.imgur.com/0DF3Ddz.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/O5vzKUt.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/hLWWEWO.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/xwZIbu3.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
<h2> <p align="center"> Congratulations!!! All Steps Are Now Complete. Enjoy Using Your Virtual Machine.</h2>
