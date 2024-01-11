<p align="center">
<img src="https://i.imgur.com/zVU5h9m.png" alt="Microsoft Active Directory Logo"/>
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
Now we will setup what type of VM we want to create. We'll begin in the "Basics" tab and choose a few key components leaving the others default. We must begin first by creating a "Resource Group" to store the VM and it's resources inside of. Under "Resource Group" click "Create New" and assign it a name. Next, give your VM a name and select the "Region" you would like it to located and function in.
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
Next scroll down to select the "Image" of Operating System that the VM will run, in this case Windows 10 is being selected. Now go down to "Size", this choose the speed for the CPU (Central Processing Unit) and the RAM (Random Access Memory) of the VM. Note you'll want to choose the appropriate "Size" for what tasks you'll be performing on the VM. Too slow of a choice and you will have a hard time getting work done with resource demanding applications; too fast a choice and you'll be wasting resources and money since this comes at a premium price.  After selecting, scroll down and assign a "Username" and "Password" (be sure to store them in a secure place in case you forget them). Finally check the box under "Licensing" and click "Next" on the bottom.
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

**Virtual Machine Configuration (continued).** 
<p>
Next we will need to select the "Image" of Operating System that the VM will run, in this case Windows 10 is being selected. Now go down to "Size", this choose the speed for the CPU (Central Processing Unit) and the RAM (Random Access Memory) of the VM. Note you'll want to choose the appropriate "Size" for what tasks you'll be performing on the VM. Too slow of a choice and you will have a hard time getting work done with resource demanding applications; too fast a choice and you'll be wasting resources and money since this comes at a premium price.
<p>
<p> 
<img src="https://i.imgur.com/XyGF2Ho.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/xAJXroj.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/uohlSle.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
