RIP Version 2 Demo — CCNA Practical Lab
📘 Overview

This project demonstrates the configuration and operation of Routing Information Protocol (RIP) Version 2 on Cisco routers using Cisco Packet Tracer.
It is part of my CCNA practical labs collection and focuses on understanding how RIP dynamically exchanges routing information between routers.

🎯 Objectives

Configure RIP v2 routing between multiple routers.

Understand distance-vector routing behavior.

Verify routing tables, updates, and network reachability.

Practice basic troubleshooting using Cisco IOS commands.

🧩 Topology

The lab includes two or more routers connected in series, each with a local LAN.

    PC1 ---- R1 ---- R2 ---- R3 ---- PC2


Each router advertises its directly connected networks using RIP version 2.

⚙️ Configuration Example
Router 1
enable
configure terminal
hostname R1
!
interface GigabitEthernet0/0
 ip address 10.0.1.1 255.255.255.0
 no shutdown
!
interface GigabitEthernet0/1
 ip address 192.168.1.1 255.255.255.0
 no shutdown
!
router rip
 version 2
 no auto-summary
 network 10.0.1.0
 network 192.168.1.0
end
write memory


Repeat similar configurations on R2 and R3, adjusting IP addresses and network statements.

🔍 Verification Commands

Use the following commands to confirm proper RIP operation:

show ip protocols — displays routing protocol and timers.

show ip route — shows learned RIP routes.

debug ip rip — monitors RIP updates (use carefully).

show ip interface brief — verify interfaces and IPs.

🧠 Key Learnings

RIP is a distance-vector protocol using hop count as its metric.

Maximum hop count is 15 — routes beyond that are unreachable.

RIP sends periodic updates every 30 seconds.

Version 2 supports VLSM and authentication.

🚀 Files Included

RIP version 2 Demo.pkt → Cisco Packet Tracer lab file

README.md → This documentation

(Optional)

configs/ → Saved router configurations

notes/ → Screenshots or observations

🧰 Tools Used

Cisco Packet Tracer

Cisco IOS Commands

CCNA Lab Environment
