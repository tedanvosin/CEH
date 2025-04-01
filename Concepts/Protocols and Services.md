# Protocols & Services: Ports and Context

This document provides an overview of important network protocols and services along with their default ports and a brief description of their purpose and relevance in cybersecurity (CEH). This table can serve as a quick reference during network assessments, penetration testing, and vulnerability analysis.

| Service/Protocol         | Port(s)                                  | Description/Context                                                                                                              |
| ------------------------ | ---------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| **HTTP**                 | 80                                       | Unencrypted web traffic. Often targeted for web exploits and vulnerabilities.                                                    |
| **HTTPS**                | 443                                      | Secure web traffic using SSL/TLS. Critical for protecting data in transit.                                                       |
| **FTP**                  | 20/21                                    | File Transfer Protocol; used for file transfers. Insecure by default; susceptible to brute-force and data interception attacks.  |
| **FTPS**                 | 990 (implicit)<br>21 (explicit)          | FTP Secure; FTP over SSL/TLS providing encrypted file transfers to mitigate FTP's inherent vulnerabilities.                      |
| **SSH**                  | 22                                       | Secure Shell for encrypted remote access and file transfers.                                                                     |
| **Telnet**               | 23                                       | Unencrypted remote login. Rarely used due to security concerns.                                                                  |
| **SMTP**                 | 25                                       | Email delivery protocol; often exploited for spam or relaying attacks.                                                           |
| **SMTPS**                | 465                                      | Secure SMTP; SMTP over SSL/TLS for secure email transmission.                                                                    |
| **DNS**                  | 53                                       | Domain Name System; essential for translating domain names to IP addresses.                                                      |
| **DNS over HTTPS (DoH)** | 443                                      | Secure DNS queries tunneled over HTTPS to prevent eavesdropping and manipulation.                                                |
| **DHCP**                 | 67/68                                    | Dynamic Host Configuration Protocol; automatically assigns IP addresses in a network.                                            |
| **TFTP**                 | 69                                       | Trivial File Transfer Protocol; simple and insecure file transfers, often used in network booting.                               |
| **POP3**                 | 110                                      | Post Office Protocol; used for retrieving email from a server.                                                                   |
| **POP3S**                | 995                                      | Secure POP3; POP3 over SSL/TLS providing encrypted email retrieval.                                                              |
| **IMAP**                 | 143                                      | Internet Message Access Protocol; allows remote email management and retrieval.                                                  |
| **IMAPS**                | 993                                      | Secure IMAP; IMAP over SSL/TLS for secure email communication.                                                                   |
| **SNMP**                 | 161                                      | Simple Network Management Protocol; used for network monitoring and management.                                                  |
| **SNMP Trap**            | 162                                      | Used for sending SNMP alerts or notifications from network devices.                                                              |
| **LDAP**                 | 389                                      | Lightweight Directory Access Protocol; used for directory services and authentication.                                           |
| **LDAPS**                | 636                                      | Secure LDAP; encrypted version of LDAP for protecting directory queries and data.                                                |
| **NetBIOS/SMB**          | 137-139, 445                             | Used for Windows file sharing and printer services. Legacy NetBIOS ports (137-139) are often targeted by network attacks.        |
| **RDP**                  | 3389                                     | Remote Desktop Protocol; used for remote graphical access to Windows systems.                                                    |
| **NTP**                  | 123                                      | Network Time Protocol; synchronizes clocks across devices, which is crucial for logging and incident response.                   |
| **Kerberos**             | 88                                       | Authentication protocol used in Windows and Unix environments for secure ticket-based authentication.                            |
| **SIP**                  | 5060 (unencrypted)<br>5061 (encrypted)   | Session Initiation Protocol; used in VoIP communications, both in cleartext and secure variants.                                 |
| **RADIUS**               | 1812/1813                                | Remote Authentication Dial-In User Service; used for centralized authentication and accounting.                                  |
| **MySQL**                | 3306                                     | Database service for MySQL; a common target for database exploits and SQL injection attacks.                                     |
| **MSSQL**                | 1433                                     | Microsoft SQL Server; often targeted for SQL injection and credential theft.                                                     |
| **VNC**                  | 5900                                     | Virtual Network Computing; used for remote desktop sharing and often targeted for unauthorized access.                           |
| **Redis**                | 6379                                     | In-memory data store; misconfigurations can lead to data exfiltration or remote code execution.                                  |
| **Modbus**               | 502                                      | Protocol used in industrial control systems; vulnerabilities can have critical impacts on infrastructure.                        |
| **MQTT**                 | 1883                                     | Lightweight messaging protocol, primarily used in IoT; misconfigurations can expose devices to remote attacks.                   |
| **PPTP**                 | 1723                                     | Point-to-Point Tunneling Protocol; used for VPNs but considered insecure and vulnerable to various attacks.                      |
| **L2TP/IPSec**           | 1701 (L2TP)<br>500 (IKE)<br>4500 (NAT-T) | Combination used for secure VPN connections; L2TP paired with IPSec offers enhanced security for remote access.                  |
| **OpenVPN**              | 1194                                     | Open-source VPN protocol (typically UDP, sometimes TCP); widely used for secure remote access.                                   |
| **Syslog**               | 514                                      | Protocol for forwarding log messages in an IP network; essential for centralized logging and monitoring.                         |
| **XMPP**                 | 5222 (client), 5269 (server)             | Extensible Messaging and Presence Protocol; used for instant messaging and presence information, sometimes leveraged by botnets. |
| **ICMP**                 | N/A                                      | Internet Control Message Protocol; used for network diagnostics (e.g., ping, traceroute) and error reporting.                    |

---
