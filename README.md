## Objective

To equip with the skills and methodologies necessary for investigating ransomware attacks using Splunk, focusing on identifying indicators of compromise (IOCs), analyzing PowerShell commands, and understanding ransomware behavior.

### Skills Learned

- Log Analysis: Efficient use of Splunk to sift through logs and identify malicious activities.
- Incident Response: Understanding the steps for responding to ransomware attacks, including timeline filtering and IOC identification.
- PowerShell Command Decoding: Analyzing PowerShell commands to track malicious activities.
- Malware Analysis: Understanding ransomware behavior, including encryption patterns and ransom notes.
- Critical Thinking: Developing a methodical approach to analyzing evidence and correlating events for a comprehensive investigation.
  
### Tools Used

- Splunk: For log analysis and timeline filtering.
- CyberChef: For decoding and analyzing data.
- VirusTotal: For checking malicious file hashes and binaries.
- Sysmon: Track and record system activity in the Windows event log.

## Practical Exercises

<p align="center">
<img src="https://imgur.com/LwGyPzk.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>Set the timeline to match the time of incident.</b>
<br/>

<p align="center">
<img src="https://imgur.com/fxaCAzW.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>Check which sources are available.</b>
<br/>

<p align="center">
<img src="https://imgur.com/k70KDWN.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>User machine's IP address.</b>
<br/>

<p align="center">
<img src="https://imgur.com/mjg7xjG.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>Destination IP addresses that the user's machine tried to connect to.</b>
<br/>

<p align="center">
<img src="https://imgur.com/nNzYJvu.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/nbWCpTQ.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/zeT5lk3.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>The suspicious destination IP address that the user's machine tried to connect to, along with a suspicious executable in the Temp directory, seems suspicious.</b>
<br/>

<p align="center">
<img src="https://imgur.com/zgETTsb.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>The address from which the suspicious binary was downloaded.</b>
<br/>

<p align="center">
<img src="https://imgur.com/tPGQ0mw.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>The command was executed to configure the suspicious binary to run with elevated privileges.</b>
<br/>

<p align="center">
<img src="https://imgur.com/0oLTNJX.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>The permissions under which the suspicious binary runs, and the command that runs the binary with elevated privileges.</b>
<br/>

<p align="center">
<img src="https://imgur.com/zSJhDWs.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>The remote server to which the suspicious binary connected.</b>
<br/>

<p align="center">
<img src="https://imgur.com/4TqxgSS.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>A PowerShell script was downloaded to the same location as the suspicious binary.</b>
<br/>

<p align="center">
<img src="https://imgur.com/9yUo9DM.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/quvLzAR.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>The actual name of the malicious script after it was flagged as malicious.</b>
<br/>

<p align="center">
<img src="https://imgur.com/MjFLUEC.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>A ransomware note was saved to the user's machine disk.</b>
<br/>

<p align="center">
<img src="https://imgur.com/9JqYLSq.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>The image file was saved to disk to replace the user's desktop wallpaper, similar to how most ransomware replaces the desktop wallpaper</b>
<br/>

## Outcome

- Improved Investigation Skills: Gain hands-on experience with Splunk and other essential tools, enhancing efficiency in identifying and analyzing IOCs.
- IOC Identification: Successful identification of key IOCs, including malicious binaries, PowerShell commands, and ransomware characteristics.
- Enhanced Response Tactics: Learn to respond quickly to incidents, focusing on relevant logs and events within defined timeframes.
- Understanding Ransomware: Comprehensive knowledge of ransomware behavior, including file encryption, ransom notes, and executable interactions.

## Acknowledgements
- Adapted from [TryHackMe - PS Eclipse](https://tryhackme.com/r/room/posheclipse)
- [Splunk](https://www.splunk.com/)
- [VirusTotal](https://www.virustotal.com/)
- [Sysmon](https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon)

## Disclaimer

The projects and activities within this portfolio are for educational and ethical cybersecurity research purposes only. All work was performed in controlled environments, including isolated, personally owned laboratories, subscription-based cloud environments, and through engagement with online cybersecurity learning platforms. Any cloud-based activities and participation in online learning platforms were conducted in full compliance with their respective terms of service and acceptable use policies. These projects should not be used for any illegal or unethical activities. Unauthorized access to any computer system or network is strictly prohibited. The author(s) are not responsible for any misuse of the information or code provided.
