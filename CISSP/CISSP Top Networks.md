# CISSP Top Networks

## Top 10 IEEE Standards *

| IEEE | Title | Source |
|-|-|-|
| 802.1X | IEEE Standard for Local and Metropolitan Area Networks--Port-Based Network Access Control | https://standards.ieee.org/ieee/802.1X/7345/ |
| 802.3 | IEEE Standard for Ethernet | https://standards.ieee.org/ieee/802.3/7071/ |
| 802.11 | IEEE Standard for Information Technology--Telecommunications and Information Exchange between Systems - Local and Metropolitan Area Networks--Specific Requirements - Part 11: Wireless LAN Medium Access Control (MAC) and Physical Layer (PHY) Specifications | https://standards.ieee.org/ieee/802.11/7028/ |
| 802.11i | IEEE Standard for information technology-Telecommunications and information exchange between systems-Local and metropolitan area networks-Specific requirements-Part 11: Wireless LAN Medium Access Control (MAC) and Physical Layer (PHY) specifications: Amendment 6: Medium Access Control (MAC) Security Enhancements | https://standards.ieee.org/standard/802_11i-2004.html |
| 802.15 | IEEE Standard for Low-Rate Wireless Networks | https://standards.ieee.org/ieee/802.15.4/7029/ |

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
| 49 | TCP, UDP | Cisco Terminal Access Controller Access-Control System (TACACS+) |
| 53 | TCP, UDP | Domain Name System (DNS) |
| 67 | UDP | DHCP - server |
| 68 | UDP | DHCP - client |
| 80 | TCP, UDP | Hypertext Transfer Protocol (HTTP) |
| 88 | TCP, UDP | Kerberos |
| 110 | TCP | Post Office Protocol version 3 (POP3) |
| 123 | UDP | Network Time Protocol (NTP) |
| 161 | UDP | Simple Network Management Protocol (SNMP) protocol |
| 162 | TCP, UDP | Simple Network Management Protocol (SNMP) trap |
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
| 1812 | UDP | RADIUS authentication protocol |
| 1813 | UDP | RADIUS accounting protocol |
| 3389 | TCP, UDP | Microsoft Remote Desktop Protocol (RDP) |
| 3868 | TCP | Diameter base protocol |

- Source: https://www.iana.org/assignments/service-names-port-numbers/service-names-port-numbers.xhtml
- Source: https://wiki.wireshark.org/PortReference


## Top 5 Unusual IPv4 ranges

| IPv4 CIDR | IPv4 Range | Number of IPs | Purpose | Source |
|-|-|-|-|-|
| 0.0.0.0/8 | 0.0.0.0–0.255.255.255 | 16,777,216 | This network | RFC791 |
| 10.0.0.0/8 | 10.0.0.0–10.255.255.255 | 16,777,216 | Private-Use | RFC1918 |
| 172.16.0.0/12 | 172.16.0.0–172.31.255.255 | 1,048,576 | Private-Use | RFC1918 |
| 192.168.0.0/16 | 192.168.0.0–192.168.255.255 | 65,536 | Private-Use | RFC1918 |
| 127.0.0.0/8 | 127.0.0.0–127.255.255.255 | 16,777,216 | Loopback | RFC1122 |

- Source: https://www.iana.org/assignments/iana-ipv4-special-registry/iana-ipv4-special-registry.xhtml

# Top 3 CIDR classes

CIDR refers to Classless Inter-Domain Routing. 

| Class | Description | Hosts |
|-|-|-|
| A | A Class A IPv4 address has 8 network prefix bits. For example, consider 44.0.0.1, where 44 is the network address and 0.0.1 is the host address. | 16,777,214 hosts |
| B | A Class B IPv4 address has 16 network prefix bits. For example, consider 128.16.0.2, where 128.16 is the network address and 0.2 is the host address. | 65,534 hosts |
| C | A Class C IPv4 address has 24 network prefix bits. For instance, consider 192.168.1.100, where 192.168.1 is the network address and 100 is the host address. | 254 hosts |

- Source: https://aws.amazon.com/what-is/cidr/

# CIDR 

| Address format | Addresses | Typical use |
|-|-|-|
| a.b.c.d/32 | 1 | Host route |
| a.b.c.d/31 | 2 | Point-to-point links (RFC 3021) |
| a.b.c.d/30 | 4 | Point-to-point links (glue network) |
| a.b.c.d/29 | 8 | Smallest multi-host network |
| a.b.c.d/28 | 16 | Small LAN |
| a.b.c.d/27 | 32 | |
| a.b.c.d/26 | 64 | |
| a.b.c.d/25 | 128 | Large LAN |
| a.b.c.x/24 | 256 | A Class C IPv4 address. |
| a.b.c.x/23 | 512 | |
| a.b.c.x/22 | 1,024 | Small business |
| a.b.c.x/21 | 2,048 | Small ISP/ large business |
| a.b.c.x/20 | 4,096 | |
| a.b.c.x/19 | 8,192 | ISP/ large business |
| a.b.c.x/18 | 16,384 | |
| a.b.c.x/17 | 32,768 | |
| a.b.x.x/16 | 65,536 | A Class B IPv4 address. |
| a.b.x.x/15 | 131,072 | |
| a.b.x.x/14 | 262,144 | |
| a.b.x.x/13 | 524,288 | |
| a.b.x.x/12 | 1,048,576 | |
| a.b.x.x/11 | 2,097,152 | |
| a.b.x.x/10 | 4,194,304 | |
| a.b.x.x/9 | 8,388,608 | |
| a.x.x.x/8 | 16,777,216 | A Class A IPv4 address. |
| a.x.x.x/7 | 33,554,432 | |
| a.x.x.x/6 | 67,108,864 | |
| a.x.x.x/5 | 134,217,728 | |
| a.x.x.x/4 | 268,435,456 | |
| a.x.x.x/3 | 536,870,912 | |
| a.x.x.x/2 | 1,073,741,824 | |
| a.x.x.x/1 | 2,147,483,648 | |
| x.x.x.x/0 | 4,294,967,296 | Entire IPv4 Internet, default route. |

- Source: https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing

