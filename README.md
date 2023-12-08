<h1>Failed Remote Desktop Protocol(RDP) to IP Geolocation Info</h1>

<h2>Description</h2>
<b>This repository includes a PowerShell that parses Windows Event Log data related to failed RDP attempts. It leverages a third-party API to retrieve attacker geolocation data..</b>
<br/>
<br/>
In this demonstration, we'll explore the power of Azure Sentinel for security monitoring and threat hunting. We'll set up a virtual machine acting as a honeypot specifically designed to attract and capture malicious activity. As live attacks, primarily RDP brute force attempts, hit the honeypot from various corners of the globe, we'll leverage a custom PowerShell script to gather crucial information: the geolocation of the attackers. This valuable data will then be visualized on an interactive Azure Sentinel map, providing a clear and insightful picture of the attack landscape.
<br />
<br />

<p align="center">

  
</p>
<h2>Languages Used</h2>

- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer 

<h2>Utilities Used</h2>

- <b>ipgeolocation.io:</b> IP Address to Geolocation API

Update: We're witnessing increased activity on the honeypot, with attacks originating from China. Our custom script has successfully extracted and logged valuable geolocation data, providing valuable insights into the attack source.

<p align="center">
<img src="https://github.com/Sophi-E/Sentinel-lab/assets/42657684/c674364c-afab-4b1a-8c59-e2983192f8da"  height="85%" width="85%" alt="Image Analysis Dataflow" />
  
</p>


<h2>Custom logs on Log Analytics workspace</h2>

<p align="center">
  
<img src = "https://github.com/Sophi-E/Sentinel-lab/assets/42657684/dbebc63b-a61a-419f-bab9-9b75f7ca7e57" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>World map of incoming attacks after 2 hours (built custom logs including geodata)</h2>

<p align="center">

<img src="https://github.com/Sophi-E/Sentinel-lab/assets/42657684/ea7bf037-4017-4aa3-92da-1c208edf253c" height="85%" width="85%" alt="Image Analysis Dataflow"/>
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
