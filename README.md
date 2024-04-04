<div align="center">
  <img src="https://i.imgur.com/uumfBQn.png" alt="Wireshark logo"/>
</div>

<h1>Networking in Azure VMs</h1>
This tutorial is for beginners to learn Azure networking. You'll create a resource group with Windows 10 and Linux virtual machines, and use Wireshark to watch ICMP, SSH, DHCP, DNS, and RDP traffic. Understand network talks, turn off and on ICMP talk, and explore basic networking ideas. Also, learn to manage resources by deleting the group and confirming its removal.

<h2>Tasks Summary</h2>

- Create a Resource Group.
- Set up a Windows 10 Virtual Machine (VM).
- Create a Linux (Ubuntu) VM.
- Install Wireshark in your Windows 10 VM.
- Watch ICMP Traffic.
- Monitor SSH Traffic.
- Check DHCP Traffic.
- Analyze DNS Traffic.
- Observe RDP Traffic.
- Delete the Resource Groups to avoid costs.
- Confirm the Resource Groups are gone.

<h2>Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computers)
- Remote Desktop
- Command-Line Tools
- Network Protocols (ICMP, SSH, DHCP, DNS, RDP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems</h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>Requirements</h2>

- Active Azure account (Tenant) and Subscription
- Completion of Azure Account and Storage Lab (recommended)

<h2>Installation Steps</h2>

<h3>Create a Resource Group.</h3>
<p>
<img src="https://i.imgur.com/3Qafc6P.png" height="80%" width="80%" alt="RG Creation"/>
</p>
<p>
  To create a resource group in Azure, search for "Resource Group", click 'Create', choose your subscription, name the group (e.g., RG-Lab-2), select a region, and click 'Create'.
</p>

<h3>Set up a Windows 10 Virtual Machine (VM).</h3>
<p>
  To create a Windows 10 Virtual Machine (VM) in Azure, follow these steps:
  <ol>
    <li>Search for "Virtual Machine" in Azure.</li>
    <li>Click on 'Create' and choose "Azure virtual machine".</li>
    <li>Select your subscription and specify the resource group (e.g., RG-Lab-2).</li>
    <li>Name the virtual machine (e.g., VM1) and select a region for its creation.</li>
    <li>Choose the Windows 10 Pro image and select a size for your VM.</li>
    <li>Set up the username, password, licensing, and disk options.</li>
    <li>Configure the network settings and click 'Create'.</li>
  </ol>
</p>

<h3>Create a Linux (Ubuntu) VM.</h3>
<p>
<img src="https://i.imgur.com/GVWotlE.png" height="80%" width="80%" alt="Linux VM Creation"/>
</p>
<p>
  To create a Linux (Ubuntu) VM in Azure, follow similar steps as above but choose the Ubuntu Server 20.04 LTS image and configure the authentication type, username, password, disk options, and network settings accordingly.
</p>

<h3>Install Wireshark in your Windows 10 VM.</h3>
<p>
  To install Wireshark on your Windows 10 VM, you'll need to:
  <ol>
    <li>Access your VM through Remote Desktop.</li>
    <li>Download Wireshark from the official website.</li>
    <li>Install Wireshark following the setup instructions.</li>
  </ol>
</p>

<h3>Watch ICMP Traffic.</h3>
<p>
<img src="https://i.imgur.com/GT0gM6d.png" height="80%" width="80%" alt="ICMP Traffic"/> 
</p>
<p>
  To observe ICMP traffic:
  <ol>
    <li>Launch Wireshark and filter for "icmp".</li>
    <li>Initiate ping commands from PowerShell to observe the traffic.</li>
    <li>Experiment with blocking and unblocking ICMP traffic using Network Security Groups in Azure.</li>
  </ol>
</p>

<!-- Repeat the same pattern for SSH Traffic, DHCP Traffic, DNS Traffic, and RDP Traffic -->

<h3>Monitor SSH Traffic.</h3>
<p>
<img src="https://i.imgur.com/saQJeGN.png" height="80%" width="80%" alt="SSH Traffic"/>
</p>
<p>
  To observe SSH traffic:
  <ol>
    <li>Filter for "ssh" or "tcp.port == 22" in Wireshark.</li>
    <li>Establish an SSH connection from your Windows 10 VM to the Linux VM.</li>
    <li>Execute various commands within the SSH session and monitor the traffic in Wireshark.</li>
  </ol>
</p>

<h3>Check DHCP Traffic.</h3>
<p>
<img src="https://i.imgur.com/GK8tuBs.png" height="80%" width="80%" alt="DHCP Traffic"/>
</p>
<p>
  To analyze DHCP traffic:
  <ol>
    <li>Filter for "dhcp" in Wireshark.</li>
    <li>Trigger a DHCP renewal process in your Windows 10 VM and observe the DHCP messages exchanged.</li>
  </ol>
</p>

<h3>Analyze DNS Traffic.</h3>
<p>
 <img src="https://i.imgur.com/8r7blHa.png" height="80%" width="80%" alt="DNS Traffic"/>
</p>
<p> 
  To observe DNS traffic:
  <ol>
    <li>Filter for "dns" or "udp.port == 53" in Wireshark.</li>
    <li>Perform DNS lookups from PowerShell and monitor the DNS traffic in Wireshark.</li>
  </ol>
</p>

<h3>Observe RDP Traffic.</h3>
<p>
<img src="https://i.imgur.com/5XVzhIV.png" height="80%" width="80%" alt="RDP Traffic"/>
</p>
<p>  
  To monitor RDP traffic:
  <ol>
    <li>Filter for "rdp" or "tcp.port == 3389" in Wireshark.</li>
    <li>Establish an RDP connection to your Windows 10 VM and observe the ongoing RDP traffic.</li>
  </ol>
</p>

<h3>Delete the Resource Groups.</h3>
<p>
  <img src="https://i.imgur.com/wNlmze9.png" height="80%" width="80%" alt="Delete RG"/>
</p>
<p>
  To remove the Resource Groups:
  <ol>
    <li>Search for "Resource Group" in Azure.</li>
    <li>Click on the resource group you want to delete.</li>
    <li>Click 'Delete resource group', confirm the deletion, and repeat for any other relevant resource groups.</li>
  </ol>
</p>

<h3>Verify Deletion.</h3>
<p>
  To confirm the Resource Groups are deleted:
  <ol>
    <li>Search for "Resource Group" in Azure.</li>
    <li>Ensure that the specified resource groups are no longer listed.</li>
  </ol>
</p>

<!-- You can add any concluding remarks or additional tips here -->


