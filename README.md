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

## Practical Exercises

<p align="center">
<img src="https://imgur.com/LwGyPzk.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Set the timeline to match the time of incident.</b>
<br/>

<p align="center">
<img src="https://imgur.com/fxaCAzW.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Check which sources are available.</b>
<br/>

<p align="center">
<img src="https://imgur.com/k70KDWN.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>User machine's IP address.</b>
<br/>

<p align="center">
<img src="https://imgur.com/mjg7xjG.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Destination IP addresses that the user's machine tried to connect to.</b>
<br/>

<p align="center">
<img src="https://imgur.com/nNzYJvu.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/nbWCpTQ.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/zeT5lk3.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>The suspicious destination IP address that the user's machine tried to connect to, along with a suspicious executable in the Temp directory, seems suspicious.</b>
<br/>

<p align="center">
<img src="https://imgur.com/zgETTsb.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>The address from which the suspicious binary was downloaded.</b>
<br/>

<p align="center">
<img src="https://imgur.com/tPGQ0mw.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>The command was executed to configure the suspicious binary to run with elevated privileges.</b>
<br/>

<p align="center">
<img src="https://imgur.com/0oLTNJX.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>The permissions under which the suspicious binary runs, and the command that runs the binary with elevated privileges.</b>
<br/>

<p align="center">
<img src="https://imgur.com/zSJhDWs.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>The remote server to which the suspicious binary connected.</b>
<br/>

<p align="center">
<img src="https://imgur.com/4TqxgSS.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>A PowerShell script was downloaded to the same location as the suspicious binary.</b>
<br/>

<p align="center">
<img src="https://imgur.com/9yUo9DM.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/quvLzAR.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>The actual name of the malicious script after it was flagged as malicious.</b>
<br/>

<p align="center">
<img src="https://imgur.com/MjFLUEC.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>A ransomware note was saved to the user's machine disk.</b>
<br/>

<p align="center">
<img src="https://imgur.com/9JqYLSq.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>The image file was saved to disk to replace the user's desktop wallpaper, similar to how most ransomware replaces the desktop wallpaper</b>
<br/>

## Outcome

- Improved Investigation Skills: Gain hands-on experience with Splunk and other essential tools, enhancing efficiency in identifying and analyzing IOCs.
- IOC Identification: Successful identification of key IOCs, including malicious binaries, PowerShell commands, and ransomware characteristics.
- Enhanced Response Tactics: Learn to respond quickly to incidents, focusing on relevant logs and events within defined timeframes.
- Understanding Ransomware: Comprehensive knowledge of ransomware behavior, including file encryption, ransom notes, and executable interactions.

## Acknowledgements

This project combines ideas and methods from various sources, such as the TryHackMe - PS Eclipse room and my IT experience. These resources provided the fundamental information and techniques, which were then modified in light of practical uses.
 - [TryHackMe - PS Eclipse](https://tryhackme.com/r/room/posheclipse)
 - [Splunk](https://www.splunk.com/)
 - [CyberChef](https://gchq.github.io/CyberChef/)
 - [VirusTotal](https://www.virustotal.com/)
 
## Disclaimer

The sole goals of the projects and activities here are for education and ethical cybersecurity research. All work was conducted in controlled environments, such as paid cloud spaces, private labs, and online cybersecurity education platforms. Online learning and cloud tasks adhered closely to all usage guidelines. Never use these projects for improper or unlawful purposes. It is always prohibited to break into any computer system or network. Any misuse of the provided information or code is not the responsibility of the author or authors.
