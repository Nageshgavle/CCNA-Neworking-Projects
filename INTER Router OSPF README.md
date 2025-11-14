🖧 Inter-Router OSPF Configuration – Cisco Packet Tracer Lab

This project demonstrates the configuration and implementation of OSPF (Open Shortest Path First) dynamic routing across multiple routers using Cisco Packet Tracer.
The goal is to enable efficient route exchange, verify router adjacencies, and ensure full network connectivity across all subnets.

📌 Project Overview

The lab focuses on:

Configuring OSPF on multiple routers

Assigning Router IDs

Advertising networks into OSPF

Understanding OSPF areas (Default: Area 0)

Building neighbour relationships

Verifying OSPF database and routing table

Testing end-to-end communication

🏗️ Network Topology

The topology includes multiple interconnected routers forming an OSPF domain.
Each router shares link-state information with neighbours to build a complete network map.

(Add a screenshot of your Packet Tracer topology here for better presentation.)

⚙️ OSPF Configuration Steps
1️⃣ Enter OSPF Configuration Mode
Router(config)# router ospf <process-id>

2️⃣ Set Router ID (Recommended)
Router(config-router)# router-id <x.x.x.x>

3️⃣ Advertise Networks
Router(config-router)# network <network-address> <wildcard-mask> area 0

4️⃣ Verify OSPF Neighbours
Router# show ip ospf neighbor

5️⃣ Verify OSPF Database
Router# show ip ospf database

6️⃣ Check Routing Table
Router# show ip route ospf

7️⃣ Test Connectivity
Router# ping <destination-IP>

📂 Project Files Included

INTER ROUTER OSPF.pkt – Cisco Packet Tracer file containing the full inter-router OSPF configuration.

📘 Learning Outcomes

By completing this lab, you will understand:

✔ How OSPF operates between routers
✔ How neighbour adjacencies form
✔ How to advertise networks in OSPF
✔ How OSPF builds routing tables
✔ How to verify and troubleshoot OSPF
✔ How link-state protocols differ from distance-vector protocols

🚀 How to Use This Repository

Download the .pkt file

Open it in Cisco Packet Tracer

Observe router interfaces and OSPF configuration

Modify or expand the topology

Practice adding more routers and networks

🧑‍💻 Author

Nagesh Gavale
CCNA Learner | Networking Enthusiast | Linux & IT Support

