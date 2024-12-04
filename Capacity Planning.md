
![Screenshot 2024-12-04 101952](https://github.com/user-attachments/assets/69336825-d404-4201-a507-cf0881414b11)


![Screenshot 2024-12-04 102044](https://github.com/user-attachments/assets/0aab9feb-b61b-4b18-a2e9-abb6e6b00f86)



![Screenshot 2024-12-04 102153](https://github.com/user-attachments/assets/ae857251-c2ba-4c83-bac7-de6fe22a1ab0)




Page **2** of **6**

+-----------------------------------+-----------------------------------+
| > Network Analysis               | > ![](vertopal_d8b4bf63451241     |
|                                   | f999c111fc04bf1480/media/image4.p |
|                                   | ng){width="0.22777777777777777in" |
|                                   | > height="0.16944444444444445in"} |
|                                   | > Potential Bottlenecks:          |
|                                   | >                                 |
|                                   | > • Congestion is more likely to  |
|                                   | > occur when switches and routers |
|                                   | > are highly\                     |
|                                   | > interconnected, particularly in |
|                                   | > the\                            |
|                                   | > multilayer switches that make   |
|                                   | > up the core network. If one of  |
|                                   | > the multilayer switches fails,  |
|                                   | > traffic may become heavily\     |
|                                   | > concentrated on the remaining   |
|                                   | > switch, causing potential       |
|                                   | > delays.                         |
|                                   | >                                 |
|                                   | > • The servers connected to      |
|                                   | > access\                         |
|                                   | > switches have a single link to  |
|                                   | > each switch, making them points |
|                                   | > of failure and possible         |
|                                   | > bottlenecks.                   |
|                                   | >                                 |
|                                   | > ![](vertopal_d8b4bf63451241     |
|                                   | f999c111fc04bf1480/media/image4.p |
|                                   | ng){width="0.22777777777777777in" |
|                                   | > height="0.16944335083114612in"} |
|                                   | > Security Risks:                 |
|                                   | >                                 |
|                                   | > • Redundant links between       |
|                                   | > devices might result in network |
|                                   | > loops if protocols like STP     |
|                                   | > (Spanning Tree Protocol) are    |
|                                   | > not properly configured.        |
|                                   | >                                 |
|                                   | > • Lack of visible security      |
|                                   | > mechanisms such as firewalls    |
|                                   | > for inter-VLAN traffic and\     |
|                                   | > between core and edge layers.   |
|                                   | >                                 |
|                                   | > • No mention of access control  |
|                                   | > lists (ACLs) or segmentation to |
|                                   | > limit malicious traffic.       |
|                                   | >                                 |
|                                   | > ![](vertopal_d8b4bf63451241     |
|                                   | f999c111fc04bf1480/media/image5.p |
|                                   | ng){width="0.22777777777777777in" |
|                                   | > height="0.16944335083114612in"} |
|                                   | > Capacity Limitations:           |
|                                   | >                                 |
|                                   | > • The network appears           |
|                                   | > well-distributed, but high      |
|                                   | > traffic on the VLANs (e.g.,     |
|                                   | > from\                           |
|                                   | > servers to PCs) could cause     |
|                                   | > access-layer switch overload.   |
+===================================+===================================+
| > Scalability Planning           | > ![](vertopal_d8b4bf63451241     |
|                                   | f999c111fc04bf1480/media/image4.p |
|                                   | ng){width="0.22777777777777777in" |
|                                   | > height="0.170832239720035in"}   |
|                                   | > Relevant Solutions:             |
|                                   | >                                 |
|                                   | > • Add more servers: Ensure each |
|                                   | > VLAN has more than two servers  |
|                                   | > to balance the load better. For |
|                                   | > instance, VLAN1 might have      |
|                                   | > three servers with              |
|                                   | > active-active\                  |
|                                   | > configurations.                 |
|                                   | >                                 |
|                                   | > • Use stacking or chassis-based |
|                                   | > switches: To simplify           |
|                                   | > management and increase port    |
|                                   | > availability for future         |
|                                   | > expansions.                     |
|                                   | >                                 |
|                                   | > • Implement Virtualization: Use |
|                                   | > hardware that supports virtual  |
|                                   | > servers to improve resource     |
|                                   | > utilization and scalability.    |
+-----------------------------------+-----------------------------------+

Page **3** of **6**

+-----------------------------------+-----------------------------------+
|                                   | > ![](vertopal_d8b4bf63451241     |
|                                   | f999c111fc04bf1480/media/image6.p |
|                                   | ng){width="0.22777777777777777in" |
|                                   | > height="0.16944444444444445in"} |
|                                   | > Potential Drawbacks:            |
|                                   | >                                 |
|                                   | > • Higher cost for new hardware  |
|                                   | > and                             |
|                                   | >                                 |
|                                   | > implementation.                 |
|                                   | >                                 |
|                                   | > • Increased complexity in       |
|                                   | > managing virtual                |
|                                   | >                                 |
|                                   | > servers or additional VLANs.    |
|                                   | >                                 |
|                                   | > • Potentially higher power      |
|                                   | > consumption with                |
|                                   | >                                 |
|                                   | > additional hardware.            |
+===================================+===================================+
| > Evaluation of Solutions\        | > ![](vertopal_d8b4bf63451241     |
| >                                | f999c111fc04bf1480/media/image6.p |
|                                   | ng){width="0.22777777777777777in" |
|                                   | > height="0.16944444444444445in"} |
|                                   | > Hardware Upgrades:              |
|                                   | >                                 |
|                                   | > • Added backups in every        |
|                                   | > devices. Two                    |
|                                   | >                                 |
|                                   | > each to ensure redundancy and   |
|                                   | >                                 |
|                                   | > scalability.                    |
|                                   | >                                 |
|                                   | > • Add backup power supplies for |
|                                   | > core and                        |
|                                   | >                                 |
|                                   | > access-layer devices to ensure  |
|                                   | >                                 |
|                                   | > uninterrupted operation.       |
|                                   | >                                 |
|                                   | > ![](vertopal_d8b4bf63451241     |
|                                   | f999c111fc04bf1480/media/image6.p |
|                                   | ng){width="0.22777777777777777in" |
|                                   | > height="0.16944444444444445in"} |
|                                   | > Software Configurations:        |
|                                   | >                                 |
|                                   | > • Configure STP and             |
|                                   | > EtherChannel on all             |
|                                   | >                                 |
|                                   | > redundant links to prevent      |
|                                   | > loops and                       |
|                                   | >                                 |
|                                   | > optimize traffic distribution.  |
|                                   | >                                 |
|                                   | > • Enable HSRP or VRRP on the    |
|                                   | > routers for                     |
|                                   | >                                 |
|                                   | > high availability of gateway    |
|                                   | > services.                       |
|                                   | >                                 |
|                                   | > • Introduce a centralized       |
|                                   | > management                      |
|                                   |                                   |
|                                   | system like Cisco DNA Center for  |
|                                   |                                   |
|                                   | > monitoring and scaling.        |
|                                   | >                                 |
|                                   | > ![](vertopal_d8b4bf63451241     |
|                                   | f999c111fc04bf1480/media/image6.p |
|                                   | ng){width="0.22777777777777777in" |
|                                   | > height="0.17083333333333334in"} |
|                                   | > Network Optimizations:          |
|                                   | >                                 |
|                                   | > • Introduce Quality of Service  |
|                                   | > (QoS)                           |
|                                   | >                                 |
|                                   | > configurations to prioritize    |
|                                   | > critical traffic                |
|                                   | >                                 |
|                                   | > such as server-to-PC            |
|                                   | > communications.                 |
|                                   | >                                 |
|                                   | > • Use VLAN pruning to limit     |
|                                   | > unnecessary                     |
|                                   | >                                 |
|                                   | > traffic on trunk links.         |
+-----------------------------------+-----------------------------------+
| > Proposed Design                 | +---------+---------+---------+   |
|                                   | | •       | > We    |         |   |
|                                   | |         | > added |         |   |
|                                   | | •       | > two   |         |   |
|                                   | |         | >       |         |   |
|                                   | |         |  clouds |         |   |
|                                   | |         | > as    |         |   |
|                                   | |         | > well  |         |   |
|                                   | |         | > as    |         |   |
|                                   | |         | > two   |         |   |
|                                   | |         | >       |         |   |
|                                   | |         | routers |         |   |
|                                   | |         | > and 2 |         |   |
|                                   | |         | > mul   |         |   |
|                                   | |         | tilayer |         |   |
|                                   | |         | >       |         |   |
|                                   | |         | switch. |         |   |
|                                   | +=========+=========+=========+   |
|                                   | |         | \-      | > This  |   |
|                                   | |         |         | > is to |   |
|                                   | |         |         | >       |   |
|                                   | |         |         |  ensure |   |
|                                   | |         |         | > that  |   |
|                                   | |         |         | > if    |   |
|                                   | |         |         | > one   |   |
|                                   | +---------+---------+---------+   |
|                                   | |         | > c     |         |   |
|                                   | |         | rashes, |         |   |
|                                   | |         | > it    |         |   |
|                                   | |         | > will  |         |   |
|                                   | |         | > have  |         |   |
|                                   | |         | > a     |         |   |
|                                   | |         | >       |         |   |
|                                   | |         |  backup |         |   |
|                                   | |         | > and   |         |   |
|                                   | |         | > as we |         |   |
|                                   | |         | > can   |         |   |
|                                   | |         | > see,  |         |   |
|                                   | |         | > there |         |   |
|                                   | |         | > are   |         |   |
|                                   | |         | > lots  |         |   |
|                                   | |         | > of    |         |   |
|                                   | |         | > conn  |         |   |
|                                   | |         | ection. |         |   |
|                                   | |         | >       |         |   |
|                                   | |         | > We    |         |   |
|                                   | |         | > also  |         |   |
|                                   | |         | > added |         |   |
|                                   | |         | > 2     |         |   |
|                                   | |         | > s     |         |   |
|                                   | |         | witches |         |   |
|                                   | |         | > in    |         |   |
|                                   | |         | > every |         |   |
|                                   | |         | > VLAN  |         |   |
|                                   | |         | > in    |         |   |
|                                   | |         | > order |         |   |
|                                   | |         | > to    |         |   |
|                                   | |         | > have  |         |   |
|                                   | |         | >       |         |   |
|                                   | |         |  smooth |         |   |
|                                   | |         | > con   |         |   |
|                                   | |         | nection |         |   |
|                                   | |         | > even  |         |   |
|                                   | |         | > when  |         |   |
|                                   | |         | > one   |         |   |
|                                   | |         | >       |         |   |
|                                   | |         |  switch |         |   |
|                                   | |         | > will  |         |   |
|                                   | |         | >       |         |   |
|                                   | |         |  crash. |         |   |
|                                   | |         | > We    |         |   |
|                                   | |         | > also\ |         |   |
|                                   | |         | > added |         |   |
|                                   | |         | > two   |         |   |
|                                   | |         | >       |         |   |
|                                   | |         | servers |         |   |
|                                   | |         | > each  |         |   |
|                                   | |         | > VLAN. |         |   |
|                                   | +---------+---------+---------+   |
+-----------------------------------+-----------------------------------+

> Page **4** of **6** 

+-----------------------------------+-----------------------------------+
| > Evaluation and Justification   | > ![](vertopal_d8b4bf63451241     |
|                                   | f999c111fc04bf1480/media/image6.p |
|                                   | ng){width="0.22777777777777777in" |
|                                   | > height="0.16944444444444445in"} |
|                                   | > Cost:                           |
|                                   | >                                 |
|                                   | > • High initial costs for        |
|                                   | > additional hardware (e.g.,      |
|                                   | > redundant servers, stackable\   |
|                                   | > switches, cross-over cables,    |
|                                   | > and straight- through).         |
|                                   | >                                 |
|                                   | > • Ongoing operational costs for |
|                                   | > power, maintenance, and         |
|                                   | > management.                    |
|                                   | >                                 |
|                                   | > ![](vertopal_d8b4bf63451241     |
|                                   | f999c111fc04bf1480/media/image6.p |
|                                   | ng){width="0.22777777777777777in" |
|                                   | > height="0.16944335083114612in"} |
|                                   | > Complexity:                     |
|                                   | >                                 |
|                                   | > • Increased configuration       |
|                                   | > complexity with the             |
|                                   | > introduction of STP, load       |
|                                   | > balancing, and dynamic routing. |
|                                   | >                                 |
|                                   | > • Requires staff training or    |
|                                   | > external expertise.            |
|                                   | >                                 |
|                                   | > ![](vertopal_d8b4bf63451241     |
|                                   | f999c111fc04bf1480/media/image6.p |
|                                   | ng){width="0.22777777777777777in" |
|                                   | > height="0.16944335083114612in"} |
|                                   | > Impact:                         |
|                                   | >                                 |
|                                   | > • Improved network resilience   |
|                                   | > with reduced downtime risks.    |
|                                   | >                                 |
|                                   | > • Higher bandwidth and          |
|                                   | > optimized traffic handling      |
|                                   | > enhance user experience.        |
|                                   | >                                 |
|                                   | > • The modular approach ensures  |
|                                   | > that future expansions are      |
|                                   | > simpler to implement.           |
+===================================+===================================+
+-----------------------------------+-----------------------------------+

+-----------------+-----------------+-----------------+-----------------+
| > Criteria      | > Excellent \|  | > Good \| 7pts  | > Needs         |
|                 | > 10pts         |                 | > Improvement   |
|                 |                 |                 | > \| 4pts       |
+=================+=================+=================+=================+
| **Network       | > Accurately    | > Identifies    | > Identifies    |
| Analysis**      | > identifies    | > key network   | > some basic    |
|                 | > potential     | > components    | > network       |
|                 | > bottlenecks,  | > and some      | > components    |
|                 | > security      | > potential     | > but lacks a\  |
|                 | > risks, and\   | > bottlenecks.  | > comprehensive |
|                 | > capacity      |                 | > analysis.     |
|                 | > limitations.  |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| > **Scalability | > Proposes      | > Proposes some | > Proposes      |
| > Planning**    | > multiple\     | > relevant      | > limited       |
|                 | > relevant      | > scalability   | > scalability   |
|                 | > solutions and | > strategies    | > strategies.   |
|                 | > provides      | > but lacks     |                 |
|                 | > detailed\     | > detail.       |                 |
|                 | > explanations, |                 |                 |
|                 | > including     |                 |                 |
|                 | > potential     |                 |                 |
|                 | > drawbacks and |                 |                 |
|                 | > benefits.     |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| >               | > Proposes      | > Provides a    | > Does not      |
| **Evaluation**\ | > comprehensive | > basic\        | > evaluate the  |
| > **of          | > scalability   | > evaluation of | > proposed      |
| > Solutions**   | > strategies,\  | > the\          | > solutions or  |
|                 | > including     | > proposed      | > provides a    |
|                 | > specific\     | > solutions,    | > superficial   |
|                 | >               | > but lacks     | > evaluation.   |
|                 | recommendations | > depth.        |                 |
|                 | > for\          |                 |                 |
|                 | > hardware      |                 |                 |
|                 | > upgrades,\    |                 |                 |
|                 | > software      |                 |                 |
|                 | >               |                 |                 |
|                 | configurations, |                 |                 |
|                 | > and network\  |                 |                 |
|                 | >               |                 |                 |
|                 |  optimizations. |                 |                 |
+-----------------+-----------------+-----------------+-----------------+

Page **5** of **6**

+-----------------+-----------------+-----------------+-----------------+
| > **Proposed    | > Provides a    | > Provides a    | > Does not      |
| > Design**      | > detailed and  | > basic design  | > provide a     |
|                 | >               | > but lacks     | > clear and     |
|                 |  well-justified | > specific      | > detailed      |
|                 | > design,\      | > details and   | > design.       |
|                 | > including     | >               |                 |
|                 | > network\      | justifications. |                 |
|                 | > diagrams,     |                 |                 |
|                 | > configuration |                 |                 |
|                 | > details, and\ |                 |                 |
|                 | >               |                 |                 |
|                 |  implementation |                 |                 |
|                 | > plans.        |                 |                 |
+=================+=================+=================+=================+
| > **Evaluation  | > Provides a    | > Provides a    | > Does not      |
| > and**\        | > thorough\     | > basic\        | > evaluate the  |
| > **            | > evaluation of | > evaluation of | > proposed      |
| Justification** | > the\          | > the\          | > solutions or  |
|                 | > proposed      | > proposed      | > provides a    |
|                 | > solutions,\   | > solutions,    | > superficial   |
|                 | > considering   | > but lacks     | > evaluation    |
|                 | > factors like  | > depth.        |                 |
|                 | > cost,         |                 |                 |
|                 | > complexity,   |                 |                 |
|                 | > and potential |                 |                 |
|                 | > impact.       |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Score:          |                 |                 | > /50           |
+-----------------+-----------------+-----------------+-----------------+

Page **6** of **6**
