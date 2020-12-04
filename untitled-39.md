# Ethernet WAN \(EoMPLS\)

Multiple LANs are connected with the help of a WAN using a device called a Router & One of the Types of [WAN](untitled.md) is a Leased Line WAN.

* In Ethernet WAN instead of using Serial Link between the Two Routers, SP uses Ethernet Link. 
* Even if it is not using HDLC WAN Protocol still it will Re-encapsulate & De-encapsulate IP Packets at every HOP with a new Header & Trailer. Because at every HOP in Ethernet Communication SMAC & DMAC will change. Hence it will also calculate FCS at each HOP. 
* Ethernet WAN is also known as **Ethernet Line Service \(E-Line\), Ethernet emulation, Ethernet over MPLS \(EoMPLS\)**.

  **Ethernet Line Service \(E-Line\):**

* For the Reference of kind of point-to-point Ethernet WAN service.

  **Ethernet emulation:**

* A term emphasizing that the link is not a literal Ethernet link.

  **Ethernet over MPLS \(EoMPLS\):**

  A term that refers to Multi-protocol Label Switching \(MPLS\), a technology that can be used to create the Ethernet service for the customer. 

## Reference:

CCNA 200-301 OCG, Volume 1, Pg. 66-67 - Wendell Odom.

