# Enterprise Network with DMZ

A secure enterprise network designed and configured in **Cisco Packet Tracer**. Public-facing servers (Web and DNS) are kept in a DMZ, separate from the internal company network.

## What I used

- VLANs, trunking and VTP (HR, Finance, IT, Management, Server Farm)
- EtherChannel (LACP) between the core switches
- Inter-VLAN routing and DHCP on a Layer 3 switch
- OSPF, NAT/PAT and static NAT
- Extended ACLs and port security
- DMZ with Web and DNS servers
- Branch office with local PAT internet access

## Security rules

| Traffic | Result |
|---|---|
| Internet to DMZ Web Server | Allowed |
| Internet to internal LAN | Blocked |
| DMZ to internal LAN | Blocked |
| HR to Finance | Blocked |

## Future improvements

- Site-to-site VPN (GRE or IPsec) between HQ and the branch
- Redundant edge routers (HSRP)

## Author

**W.L. Chathurika Madhuwanthi** | BICT (Hons) in Networking Technology
