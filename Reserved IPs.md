# Reserved IPs

## RFC 1918 - Private Address Space (1996)

> This document describes address allocation for private internets. The allocation permits full network layer connectivity among all hosts inside an enterprise as well as among all public hosts of different enterprises. The cost of using private internet address space is the potentially costly effort to renumber hosts and networks between public and private.
https://tools.ietf.org/html/rfc1918

| Host Min | Host Max | Network CIDR |
| --- | --- | --- |
| 10.0.0.1 | 10.255.255.254 | 10.0.0.0/8 |
| 172.16.0.1 | 172.31.255.254 | 172.16.0.0/12 |
| 192.168.0.1 | 192.168.255.254 | 192.168.0.0/16 |

## RFC 6598 Shared Address Space (2012)

> Shared Address Space is distinct from RFC 1918 private address space because it is intended for use on Service Provider networks. However, it may be used in a manner similar to RFC 1918 private address space on routing equipment that is able to do address translation across router interfaces when the addresses are identical on two different interfaces.
https://tools.ietf.org/html/rfc6598

| Host Min | Host Max | Network CIDR |
| --- | --- | --- |
| 100.64.0.1 | 100.127.255.254 | 100.64.0.0/10 | 

## RFC1122 - Requirements for Internet Hosts - Communication Layers (1989)

> Addresses in this block refer to source hosts on "this" network.  Address 0.0.0.0/32 may be used as a source address for this host on this network; other addresses within 0.0.0.0/8 may be used to refer to specified hosts on this network ([RFC1122], Section 3.2.1.3).
https://tools.ietf.org/html/rfc5735
https://tools.ietf.org/html/rfc1122

| Host Min | Host Max | Network CIDR |
| --- | --- | --- |
| 0.0.0.1 | 0.255.255.254 | 0.0.0.0/8 |

## RFC1122 - Requirements for Internet Hosts - Communication Layers (1989)

This block is assigned for use as the Internet host loopback address.  A datagram sent by a higher-level protocol to an address anywhere within this block loops back inside the host.  This is ordinarily implemented using only 127.0.0.1/32 for loopback.  As described in [RFC1122], Section 3.2.1.3, addresses within the entire 127.0.0.0/8 block do not legitimately appear on any network anywhere.
https://tools.ietf.org/html/rfc5735
https://tools.ietf.org/html/rfc1122

| Host Min | Host Max | Network CIDR |
| --- | --- | --- |
| 127.0.0.1 | 127.255.255.254 | 127.0.0.0/8 |

## RFC3927 - Dynamic Configuration of IPv4 Link-Local Addresses (2005)

This is the "link local" block.  As described in [RFC3927], it is allocated for communication between hosts on a single link.  Hosts obtain these addresses by auto-configuration, such as when a DHCP server cannot be found.
https://tools.ietf.org/html/rfc5735
https://tools.ietf.org/html/rfc3927

| Host Min | Host Max | Network CIDR |
| --- | --- | --- |
| 169.254.0.1 | 169.254.255.254 | 169.254.0.0/16 |

## RFC919 - Broadcasting Internet Datagrams (1984)

The one exception to this is the "limited broadcast" destination address 255.255.255.255.  As described in [RFC0919] and [RFC0922], packets with this destination address are not forwarded at the IP layer.
https://tools.ietf.org/html/rfc5735
https://tools.ietf.org/html/rfc919

| Host |
| --- |
| 255.255.255.255 |
