<h1>Azure Virtual Network / VM Creation and Network Monitoring</h1>
![408780434-d7f130f8-0204-4b0a-afd7-9b599cbf88ff](https://github.com/user-attachments/assets/7ece0a68-e4ad-4685-97b1-4380860b0c4a)


<h2>Description</h2>
In Microsoft Azure You have to create 2 new Virtuals Machines that run on the same Virtual Network. Through Wireshark we are able to monitor the Network Traffic between the 2 Virtual Machines or any website you would like, Note this only monitors the Traffic between your Computer and the target IP address like a website or other Virtual Machine 
<br />


<h2>Environments and Utilities Used</h2>

- <b>Microsoft Azure</b>
- <b>Remote Desktop Connection</b> 
- <b>Wireshark</b>
- <b>PowerShell</b>

<h2>Operating Systems Used </h2>

- <b>Windows 10 Professional</b>
- <b>Ubuntu 24.04</b>

<h2> Resource Group Creation </h2>

![Screenshot (14)](https://github.com/user-attachments/assets/64fc4a85-b446-443a-adc2-cebd4ad2c408)

- <b>The first step is Resource Group Creation, To create a resource group you must be signed into the Azure portal. Then you can use the search bar in the portal to search for the resource group tab. Then you press the Blue Create button in the middle of the screen. You can name this resource group anything you want but rememeber what you name the resource group.</b>

![Screenshot (16)](https://github.com/user-attachments/assets/43f70539-1f0f-4fdf-8282-09188f2f00da)

- <b>Once you Name the resource group what you want it to be called then you can press finalize and create, It might take up to 60 seconds for the resource group to be created.</b>

![Screenshot (15)](https://github.com/user-attachments/assets/a61aae6a-806d-4787-bd0c-da32b8f89394)

- <b>This is what it will look like when you create your first resource group! You can create as many as you need for any projects.</b>

<h2> Virtual Network (VN) Creation </h2>

![Screenshot (32)](https://github.com/user-attachments/assets/246d8973-7429-4d39-aeb8-d39bc9bc526b)

- <b>Now we are going to create a Virtual Network (VN), First use the Azure search bar and type in Virtual Network. Then when you are on the VN portal you can press the create button in the center, As shown in the picture you can leave most of the settings default unless you want something more advanced / specific. When you add Virtual Machines to the Network they need to be in the same time zone, so make sure you remember what timezone you created your Virtual Network in. Then Make a name for your Virtual Network, As shown above i named mine VNET. Then you can press review + create on the bottom right corner, once complete give Azure up to 2 minutes to create your virtual network.</b>

<h2> Virtual Machine (VM) Creation/Connection </h2>

![Screenshot (33)](https://github.com/user-attachments/assets/64485b6e-66f6-45db-abbc-66087fb3388f)

- <b>We are almost at Network Observation but first we need to create a Virtual Machine (VM). First use the Azure search bar and type in Virtual Machine, once located you can press the create button in the center. In the picture shown above i am going to create a Linux Virtual Machine, I put this Virtual Machine in the same timezone as my Virtual Network so that in the next picture i can add my Virtual Machine to my Network. If you want more processing power than you can go down to size on the bottom as shown in the picture above, the amount of VCPU's and RAM determine how fast or slow the Machine will run, I kept mine with the recommended size of 2 VCPU's and 8 GB's of RAM.</b>

![Screenshot (34)](https://github.com/user-attachments/assets/55ca5a8c-65fa-423e-9fea-332d2ce7a3ce)

- <b>In the picture shown above we are going to add our Virtual Machine to our Virtual Network, you don't need to touch the disk settings unless you want more storage than already allocated. You are going to press on the Virtual Network drop down menu and you should see your Virtual Network as an option to click. Now that you have selected your Virtual Network now you can press review + create, when creating a Virtual Machine with Azure please give up to 2 minutes for the Machine to be created.</b>

![Screenshot (35)](https://github.com/user-attachments/assets/3de820ae-d330-403b-8f68-5694ac21db6c)

- <b>In this picture shown above i am showing what it would look like once the computer is created in the Azure Portal, i am showing a Windows 10 Virtual Machine in the picture that is on the same network as the Linux Virtual Machine we just created. Both Linux and Windows Machines look the same on the Portal, But when you press on the 2 different machines they have different IP's and Operating Systems. I created both Windows and Linux Virtual Machines on the same Virtual Network for the commands we are going to be running in the Pictures below.</b>

- <b>To Connect to your Virtual Machine you want to click on the Virtual Machine in your Azure Portal, Then as shown above you should have a private IP address for you Virtual Machine. This is the IP address you are going to copy and paste into your remote connection tool to connect to your newly created Virtual Machine.</b>

<h2> Network Observation </h2>

![Screenshot (36)](https://github.com/user-attachments/assets/0b54a7dd-9cdb-4c15-9328-64d2c66d01a9)

![Screenshot (37)](https://github.com/user-attachments/assets/578f9562-0d4f-4e01-a791-835f7904e63d)

![Screenshot (38)](https://github.com/user-attachments/assets/16f612ee-b8c4-434e-8b82-e3bc772c82f6)

![Screenshot (39)](https://github.com/user-attachments/assets/78f63411-abf3-4862-86ba-2f12ba153856)

![Screenshot (40)](https://github.com/user-attachments/assets/bc58b358-1d8e-49fc-b98d-21dfa94c19dd)

![Screenshot (41)](https://github.com/user-attachments/assets/fb113d00-25f2-4473-bb4f-32b1d89cb325)

![Screenshot (42)](https://github.com/user-attachments/assets/0c07d3d9-fd11-4cc0-870b-4d79450b02cd)

![Screenshot (43)](https://github.com/user-attachments/assets/97bbbbb6-a433-4102-ba1d-0f48bcc34ca4)

![Screenshot (44)](https://github.com/user-attachments/assets/36fc46a6-b99a-4005-9ca2-6a0f056b198c)
