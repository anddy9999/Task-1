# Task-1
Scanning Local Network For Open Ports Using Nmap

Tools & Environment –
o	Tool Used: Nmap (Network Mapper)
o	Operating System: Kali Linux
o	Network Type: Local Area Network (LAN)

Risk analysis –

1.Port 135 – MSRPC
Description:  Used by Windows for Remote Procedure Calls.
Security Risk:   Can be exploited for information gathering Often targeted in Windows-based 
Risk Level:  Medium

2.Port 139 – NetBIOS-SSN
Description:  Used for file and printer sharing in Windows systems.
Security Risk:  Allows enumeration of network shares Can leak system and user information.
Risk Level:  Medium

3.Port 445 – Microsoft-DS (SMB)
Description:  Used for SMB file sharing.
Security Risk:  Common target for ransomware attacks (e.g., WannaCry) Vulnerable if system is unpatched.
Risk Level:  High

4.Port 902 – ISS RealSecure
Description:  Associated with security monitoring or virtualization services.
Security Risk:  If misconfigured, may expose internal services Can be abused for unauthorized access.
Risk Level:  Medium

5.Port 912 – APEX Mesh
Description:  Used by internal communication services.
Security Risk:  Limited public documentation Unknown services increase attack surface.
Risk Level:  Medium

6.Port 2869 – ICSLAP
Description:  Used for device discovery in Windows environments.
Security Risk:  Can be abused for service enumeration Rarely required in secure environments.
Risk Level:  Medium

7.Port 5357 – WSDAPI
Description:  Used for Web Services for Devices (WSD).
Security Risk: Enables device discovery May expose device metadata.
Risk Level:  Medium

Recommendation –
o	Disable Unused Service
o	Restrict SMB Access
o	Enable Host-Based Firewall
o	Apply System Updates
o	Network Segmentation

Limitations –

This assessment was limited to network scanning only. No exploitation or intrusive testing was performed. Firewall and IDS configurations may affect scan results.


Conclusion –

The scan revealed multiple open ports primarily associated with Windows networking services. While most ports are filtered by the firewall, some services such as SMB and NetBIOS pose potential security risks if left exposed. Implementing proper firewall rules, disabling unnecessary services, and maintaining updated systems will significantly reduce the attack surface


Internship Learning Outcome –

•	Practical experience with Nmap
•	Understanding of network reconnaissance
•	Ethical and authorized security testing practices

