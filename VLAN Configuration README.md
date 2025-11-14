🖧 VLAN Configuration – Cisco Packet Tracer Lab

This project demonstrates how to configure VLANs (Virtual Local Area Networks) and inter-VLAN communication in Cisco Packet Tracer.
The goal is to logically segment a network, improve security, and control broadcast domains.

📌 Project Overview

In this lab, VLANs are created and assigned to switch ports to separate devices into different logical networks.
Key objectives include:

Creating VLANs on switches

Assigning ports to VLANs

Configuring trunk ports

Setting the native VLAN

Verifying VLAN membership

Testing communication within and across VLANs

🏗️ Network Topology

The topology includes:

Multiple switches

PCs assigned to different VLANs

A trunk link between switches

Optional inter-VLAN communication via a router or Layer 3 switch

(You can insert a screenshot of your topology here.)

⚙️ VLAN Configuration Steps
1️⃣ Create VLANs
Switch(config)# vlan <vlan-id>
Switch(config-vlan)# name <vlan-name>

2️⃣ Assign Interfaces to VLANs
Switch(config)# interface fastEthernet 0/1
Switch(config-if)# switchport mode access
Switch(config-if)# switchport access vlan <vlan-id>

3️⃣ Configure Trunk Port
Switch(config)# interface fastEthernet 0/24
Switch(config-if)# switchport mode trunk
Switch(config-if)# switchport trunk allowed vlan all

4️⃣ Verify VLANs
Switch# show vlan brief

5️⃣ Verify Trunk Port
Switch# show interfaces trunk

📂 Project Files

VLAN.pkt — Cisco Packet Tracer project file containing the complete VLAN configuration.

📘 Learning Outcomes

By completing this lab, you will learn:

✔ How VLANs work
✔ How to segment networks logically
✔ How trunking enables VLAN traffic across switches
✔ How to verify and troubleshoot VLAN issues
✔ How VLANs improve security and broadcast control

🚀 How to Use This Project

Download the .pkt file

Open it in Cisco Packet Tracer

Explore the VLAN configuration on each switch

Modify or add more VLANs for practice

🧑‍💻 Author

Nagesh Gavale
Networking Learner | CCNA Student | IT Support | Linux Enthusiast
