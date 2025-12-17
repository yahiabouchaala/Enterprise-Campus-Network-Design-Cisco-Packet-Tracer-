\# IP Addressing Plan (VLSM)



Base network: 172.16.1.0/16  

Subnetting was performed using VLSM to efficiently allocate IP addresses based on departmental size and function.



\# VLAN \& Subnet Allocation



| VLAN | Department | Subnet | Mask | Default Gateway (HSRP VIP) |

|-----|-----------|--------|------|-----------------------------|

| 10 | Sales \& Marketing | 172.16.1.0 | /25 | 172.16.1.1 |

| 20 | HR \& Logistics | 172.16.1.128 | /25 | 172.16.1.129 |

| 30 | Finance \& Accounts | 172.16.2.0 | /25 | 172.16.2.1 |

| 40 | Admin \& Public Relations | 172.16.2.128 | /25 | 172.16.2.129 |

| 50 | ICT | 172.16.3.0 | /25 | 172.16.3.1 |

| 60 | Server Room | 172.16.3.128 | /28 | 172.16.3.129 |



##### \## Notes ##

\- User VLANs are sized to support ~120 devices each.

\- Server VLAN uses a /28 subnet as devices are statically assigned.

\- First-hop redundancy is provided via HSRP on multilayer switches.

\- The HSRP virtual IP is used as the default gateway in DHCP pools.



