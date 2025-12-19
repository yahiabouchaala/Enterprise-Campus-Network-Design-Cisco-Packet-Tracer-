# Enterprise Campus Network Design (Cisco Packet Tracer)

This project demonstrates the design and implementation of a scalable and redundant enterprise campus network using Cisco Packet Tracer.

📌 Scenario
A 600-user organization relocated to a new 3-floor building.  
Each floor hosts multiple departments, each requiring:
- Separate VLANs
- Wireless access
- Secure and reliable connectivity
- Centralized services

🏗 Network Architecture
- Hierarchical design (Core, Distribution, Access)
- Dual multilayer switches for redundancy
- Dual routers connected to two ISPs
- Centralized server room
⛔⛔⛔The password for every switch/Router is :cisco 
🔧 Technologies Used
- VLAN & VLSM subnetting
- Inter-VLAN routing (SVIs)
- HSRP for first-hop redundancy
- OSPF for dynamic routing
- DHCP with relay agents
- NAT/PAT for Internet access
- SSH for device management
- Port security (sticky MAC)

🌐 IP Addressing
Base network: 172.16.1.0/16  
Each department allocated its own subnet using VLSM.

🧪 Validation
- End devices obtain IP addresses via DHCP
- Inter-VLAN communication verified
- Internet connectivity tested
- HSRP failover tested by shutting down active MLS

📷 Screenshots
See the `/screenshots` directory.

🚀 Future Improvements
- DHCP redundancy
- SNMP monitoring
- STP root optimization
