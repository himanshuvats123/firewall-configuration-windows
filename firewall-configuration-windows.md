## Setup and Use a Firewall (Windows)

## 📌 1. Introduction:

A firewall is a network security mechanism that monitors and controls incoming and outgoing traffic based on predefined security rules.
The purpose of this task was to gain practical experience in configuring firewall rules to block and allow specific network ports using the built-in Windows firewall.



## 🎯 2. Objective:

The main objectives of this task were:

1.To understand the role of a firewall in system security

2.To create inbound rules to block and allow specific ports

3.To verify firewall configuration

4.To learn how to manage and remove firewall rules



## 🛠 3. Tools and Environment:

Operating System: Microsoft Windows

Tool Used: Windows Defender Firewall with Advanced Security

Testing Tool: Command Prompt


## ⚙️ 4. Methodology:

Accessing Firewall Console:
The firewall management console was opened through the Start menu by launching Windows Defender Firewall with Advanced Security. 
This interface provides advanced control over inbound and outbound rules.


## 5.Reviewing Existing Rules:

The existing inbound rules were examined to understand the default configuration and ensure no conflicts with the new rules.


## 6.Creating a Rule to Block Port 23 (Telnet):

A new inbound rule was created with the following configuration:

1.Rule Type: Port

2.Protocol: TCP

3.Port Number: 23

4.Action: Block the connection

5.Profiles Applied: Domain, Private, Public

6.Rule Name: Block Telnet Port 23

This rule prevents Telnet traffic, which is insecure because it transmits data in plain text.


## 7.Creating a Rule to Allow Port 22 (SSH):

Another inbound rule was configured:

1.Rule Type: Port

2.Protocol: TCP

3.Port Number: 22

4.Action: Allow the connection

5.Profiles Applied: Domain, Private, Public

6.Rule Name: Allow SSH Port 22

This ensures secure remote access via SSH is permitted.


## 8.Removing the Test Rule:

After verifying the configuration, the Telnet block rule was removed to restore the system to its original state and demonstrate rule management capability.



## 📊9. Results:

1.The firewall rules were successfully configured and verified:

2.Port 23 traffic was blocked, preventing insecure Telnet communication

3.Port 22 traffic was allowed, enabling secure SSH connections

4.The created rules were visible in the firewall console

The test rule was successfully deleted


## 🧠10. Discussion:

Firewalls are a critical component of a layered security approach.
Blocking unused or insecure ports reduces the attack surface, while allowing only required services ensures controlled access.

Disabling Telnet is considered a best practice because it lacks encryption, whereas SSH provides secure communication.


## 📚11. Key Learnings:

1.Practical understanding of firewall configuration

2.Difference between allowing and blocking traffic

3.Importance of port-based security controls

4.Hands-on experience with Windows security tools

5.Awareness of insecure protocols like Telnet

## 👨‍💻 Author
**Himanshu Vats** 




