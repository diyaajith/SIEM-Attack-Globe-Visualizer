<h1>SIEM-Sentinel-Map: Failed RDP to IP Geolocation Information</h1>

<h2>Description</h2>
<b>The PowerShell script found in this repository carries out the task of extracting details from the Windows Event Log concerning unsuccessful RDP (Remote Desktop Protocol) attempts. It then employs an external API to gather geographical data related to the location of the attackers.
</b>
<br />
<br />
This script is utilized within a VM where I establish Azure Sentinel, a Security Information and Event Management (SIEM) system, and link it to a virtual machine designed as a decoy for potential attacks. We will actively observe real-time instances of attacks, specifically RDP brute force attacks originating from various locations globally. To enhance this demonstration, a personalized PowerShell script is employed to retrieve geographical information about the attackers, which is subsequently displayed on an Azure Sentinel Map.
<br />
<br />

<p align="center">
<img src="https://i.imgur.com/WbaDCqU.png" height="85%" width="85%" alt="RDP event fail logs to iP Geographic information"/>
</p>
<h2>Languages Used</h2>

- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer 

<h2>Utilities Used</h2>

- <b>ipgeolocation.io:</b> IP Address to Geolocation API

<h2>Attacks from China coming in; Custom logs being output with geodata</h2>

<p align="center">
<img src="https://i.imgur.com/wvXT0ht.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>World map of incoming attacks after an hour (built custom logs including geodata)</h2>

<p align="center">
<img src="https://i.imgur.com/D3iIDmZ.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>
