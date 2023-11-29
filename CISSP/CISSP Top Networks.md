# CISSP Top Networks

## Top 10 IEEE Standards *

| IEEE | Title | Source |
|-|-|-|
| 802.1X | IEEE Standard for Local and Metropolitan Area Networks--Port-Based Network Access Control | https://standards.ieee.org/ieee/802.1X/7345/ |
| 802.3 | IEEE Standard for Ethernet | https://standards.ieee.org/ieee/802.3/7071/ |
| 802.11 | IEEE Standard for Information Technology--Telecommunications and Information Exchange between Systems - Local and Metropolitan Area Networks--Specific Requirements - Part 11: Wireless LAN Medium Access Control (MAC) and Physical Layer (PHY) Specifications | https://standards.ieee.org/ieee/802.11/7028/ |
| 802.11i | IEEE Standard for information technology-Telecommunications and information exchange between systems-Local and metropolitan area networks-Specific requirements-Part 11: Wireless LAN Medium Access Control (MAC) and Physical Layer (PHY) specifications: Amendment 6: Medium Access Control (MAC) Security Enhancements | https://standards.ieee.org/standard/802_11i-2004.html |


## Top 5 Unusual IPv4 ranges

| IPv4 CIDR | IPv4 Range | Number of IPs | Purpose | Source |
|-|-|-|-|-|
| 0.0.0.0/8 | 0.0.0.0–0.255.255.255 | 16,777,216 | This network | RFC791 |
| 10.0.0.0/8 | 10.0.0.0–10.255.255.255 | 16,777,216 | Private-Use | RFC1918 |
| 172.16.0.0/12 | 172.16.0.0–172.31.255.255 | 1,048,576 | Private-Use | RFC1918 |
| 192.168.0.0/16 | 192.168.0.0–192.168.255.255 | 65,536 | Private-Use | RFC1918 |
| 127.0.0.0/8 | 127.0.0.0–127.255.255.255 | 16,777,216 | Loopback | RFC1122 |

- Source: https://www.iana.org/assignments/iana-ipv4-special-registry/iana-ipv4-special-registry.xhtml


## Top Ports

Port numbers range from 0 to 65,535.

| Ports | Assignment |
|-|-|
| 0 - 1,023 | Well-known ports |
| 1,024 - 49,151 | Registered ports |
| 49152 – 65535 | Dynamic, private or ephemeral ports |

| Port | L3 | Protocol |
|-|-|-|
| 20 | TCP | File Transfer Protocol (FTP) - data transfer |
| 21 | TCP | File Transfer Protocol (FTP) - control / command |
| 22 | TCP | Secure Shell (SSH) |
| 22 | TCP | Secure File Transfer Protocol (SFTP) |
| 23 | TCP | Telnet |
| 25 | TCP | Simple Mail Transfer Protocol (SMTP) |
| 53 | TCP, UDP | Domain Name System (DNS) |
| 67 | UDP | DHCP - server |
| 68 | UDP | DHCP - client |
| 80 | TCP, UDP | Hypertext Transfer Protocol (HTTP) |
| 88 | TCP, UDP | Kerberos |
| 110 | TCP | Post Office Protocol version 3 (POP3) |
| 123 | UDP | Network Time Protocol (NTP) |
| 161 | UDP | Simple Network Management Protocol (SNMP) |
| 220 | TCP, UDP | Internet Message Access Protocol (IMAP) |
| 389 | TCP | Lightweight Directory Access Protocol (LDAP) |
| 443 | TCP, UDP | Hypertext Transfer Protocol Secure (HTTPS) |
| 465 | TCP | SMTP over TLS/SSL (SMTPS) |
| 500 | UDP | Internet Security Association and Key Management Protocol (ISAKMP) / Internet Key Exchange (IKE) |
| 636 | TCP | Lightweight Directory Access Protocol over TLS/SSL (LDAPS) |
| 989 | TCP, UDP | FTP over TLS/SSL (FTPS) - data transfer |
| 990 | TCP, UDP | FTP over TLS/SSL (FTPS) - control / command |
| 992 | TCP, UDP | Telnet protocol over TLS/SSL |
| 993 | TCP | Internet Message Access Protocol over TLS/SSL (IMAPS) |
| 995 | TCP, UDP | Post Office Protocol 3 over TLS/SSL (POP3S) |
| 3389 | TCP, UDP | Remote Desktop Protocol (RDP) |

### Source
https://www.iana.org/assignments/service-names-port-numbers/service-names-port-numbers.xhtml
https://wiki.wireshark.org/PortReference
