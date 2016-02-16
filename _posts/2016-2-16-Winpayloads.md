---
layout: post
title: WinPayloads - Undetectable Windows Payload Generation
published: true
---

![WinPayloads Menu](/images/2016-02-16 10_12_29-Kali2 - VMware Workstation.png)

*Winpaylods is a payload generator tool that uses metasploits meterpreter shellcode, injects the users ip and port into the shellcode and writes a python file that executes the shellcode using ctypes. This is then aes encrypted and compiled to an Windows Executable using pyinstaller.*
<br />

#Features:
* Undetectable Windows Payload Generation
* Easy to Use Gui
* Upload Payload to Local WebServer
* Psexec Payload to Target Machine
* Automatically Runs Metasploit Listener with Correct Settings after Payload Generated
* Shellter Intergration

<br />
Winpayloads also comes with a few features such as **uac bypass** and **payload persistence**. These are powershell files that execute on the system when the meterpreter gets a reverse shell. The uac bypass is written by **PowerShellEmpire** and uses an exploit to bypass uac on local administrator accounts and creates a reverse meterpreter running as local administrator back to the attackers machine.

Winpayloads can also setup a **SimpleHTTPServer** to put the payload on the network to allow downloading on the target machine and also has a **psexec** feature that will execute the payload on the target machine if supplied with usernames,domain,passwords or hashes. **psexec.py is writted by imacket**
