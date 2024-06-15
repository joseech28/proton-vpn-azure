<p align="center">
<img src="https://i.imgur.com/48bnieh.png" alt="Traffic Examination"/>
</p>

<h1>Creating and Using an Azure VM with VPN for IP and Location Testing</h1>
In this tutorial,  involves identifying your public IP address and its associated location using an online IP lookup service. This information will be used as a reference point for later exercises. <br />






<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Web Browsers
- Windows 10
- Proton VPN
- Localization Features

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)

<h2>High-Level Steps</h2>



<h2>Actions and Observations</h2>

<p>
<img src="https://imgur.com/fymZz54.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
1. I opened my web browser on my personal computer.
I navigated to whatismyipaddress.com.
I noted down the public IP address and the city that was displayed.
I recorded this information in a notepad file.
</p>
<br />

<p>
<img src="https://imgur.com/c3qNDfQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
2. I went to the Microsoft Azure portal and logged in with my Azure account.
In the Azure portal, I clicked on Create a resource.
I searched for Virtual Machine and selected Create.
I chose a region outside of my current location (e.g., East US since I'm in West US).
Under the Image section, I selected Windows 10.
I set the Username to "lab user" and created a strong password.
I completed the setup and clicked Review + create. Once validated, I clicked Create.
</p>
<br />


<p>
<img src="https://imgur.com/qunkdIj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
3. Once the VM was created, I navigated to the Virtual Machine section in the Azure portal.
</p>
<br />


<p>
<img src="https://imgur.com/tkL7bXu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
4. I found the public IP address of the VM.
</p>
<br />

<p>
<img src="https://imgur.com/U2jLgfN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
5. I opened Microsoft Remote Desktop (or on a PC, I would open Remote Desktop Connection).
I entered the public IP address of my VM and clicked Connect.
I used the username "lab user" and the password I created to log in.
</p>
<br />

<p>
<img src="https://imgur.com/o7lXmMn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
6. Within the VM, I opened a web browser and went to whatismyipaddress.com.
I noted down the public IP address and the location, which matched the region I selected for the VM.
</p>
<br />


<p>
<img src="https://imgur.com/YDZhnYJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
7. On my local computer, I went to Proton VPN and created a free account.
</p>
<br />

<p>
<img src="https://imgur.com/ZWvMPix.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
8. In my Azure VM, I opened a web browser and went to Proton VPN's download page.
I downloaded and installed the Windows Proton VPN client.
</p>
<br />

<p>
<img src="https://imgur.com/Ika7sSL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
9. I opened the Proton VPN app within my VM.
I logged in with my Proton VPN account credentials.
</p>
<br />

<p>
<img src="https://imgur.com/yu7eZnx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
10. With the VPN connected, I refreshed the whatismyipaddress.com page within my VM.
I noted that the IP address and location now reflected the VPN endpoint in Tokyo, Japan.
</p>
<br />


<p>
<img src="https://imgur.com/5o0lrH2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
11. With the VPN connected, I refreshed the whatismyipaddress.com page within my VM.
I noted that the IP address and location now reflected the VPN endpoint in Tokyo, Japan.
</p>
<br />








