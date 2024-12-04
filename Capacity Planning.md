
![sysadm pkt![Uploading Capacity Planning.png…]()










](https://github.com/user-attachments/assets/cbfe0d67-ead7-41fe-a6ff-50bb9d668304)


Network Analysis:
Potential Bottlenecks:

•	Congestion is more likely to occur when switches and routers are highly interconnected, particularly in the multilayer switches that make up the core network. If one of the multilayer switches fails, traffic may become heavily concentrated on the remaining switch, causing potential delays.

•	The servers connected to access switches have a single link to each switch, making them points of failure and possible bottlenecks.

Security Risks:

• Network loops could arise from redundant links between devices if protocols such as STP (Spanning Tree Protocol) are not set up correctly. 

•	Absence of obvious security measures, such firewalls, for traffic between core and edge layers and between VLANs.

•	No mention of access control lists (ACLs) or segmentation to limit malicious traffic.

Capacity Limitations:

•	The network appears well-distributed, but high traffic on the VLANs (e.g., from servers to PCs) could cause access-layer switch overload. 


Scalability Planning:

Relevant Solutions:

•	Add more servers: Ensure each VLAN has more than two servers to balance the load better. For instance, VLAN1 might have three servers with active-active configurations.

•	Use stacking or chassis-based switches: To simplify management and increase port availability for future expansions.

•	Implement Virtualization: Use hardware that supports virtual servers to improve resource utilization and scalability.


Potential Drawbacks:

•	Higher cost for new hardware and implementation.

•	Increased complexity in managing virtual servers or additional VLANs.

•	Potentially higher power consumption with additional hardware.

Evaluation of Solutions:

Hardware Upgrades:

•	Added backups in every devices. Two each to ensure redundancy and scalability.

•	Add backup power supplies for core and access-layer devices to ensure uninterrupted operation.

Software Configurations:

•	Configure STP and EtherChannel on all redundant links to prevent loops and optimize traffic distribution.

•	Enable HSRP or VRRP on the routers for high availability of gateway services.

•	Introduce a centralized management system like Cisco DNA Center for monitoring and scaling.

Network Optimizations:

•	Introduce Quality of Service (QoS) configurations to prioritize critical traffic such as server-to-PC communications.

•	Use VLAN pruning to limit unnecessary traffic on trunk links.


Proposed Design: 

•	We added two clouds as well as two routers and 2 multilayer switch. 

-	This is to ensure that if one crashes, it will have a backup and as we can see, there are lots of connection.
  
•	We also added 2 switches in every VLAN in order to have smooth connection even when one switch will crash. We also added two servers each VLAN.


Evaluation and Justification:

Cost:

• High initial costs for additional hardware (e.g., redundant servers, stackable switches, cross-over cables, and straight-through).

•	Ongoing operational costs for power, maintenance, and management.

 Complexity:
 
•	Increased configuration complexity with the introduction of STP, load balancing, and dynamic routing.

•	Requires staff training or external expertise.

Impact:

•	Improved network resilience with reduced downtime risks.

•	Higher bandwidth and optimized traffic handling enhance user experience.

•	The modular approach ensures that future expansions are simpler to implement.
