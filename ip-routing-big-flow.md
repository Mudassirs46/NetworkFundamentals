# IP Routing \(BIG FLOW\)

The main job of [IP](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/ip-internet-protocol) is Routing of IP Packets from Source to Destination.

* Using BUS Topology, Sender PC1 is connected to SW1 then to a R1. R1 is connected to R2 via a Serial Line using HDLC WAN Link. R2 is further connected to R3 via EoMPLS WAN Link. R3 is then finally connected to SW2 which is connected to the destination PC2.
* R1's Network is in 150.150.1.0 Network & R2's Network is in 150.150.4.0 Network.
* **PC1 sends to packet to its Default Router:**
  * PC1's Network Layer logic builds the IP packet with 150.150.4.10 as a DIP. 
  * Network Layer also analyzes that 150.150.4.0 Network is not in the Local IP Subnet, so PC1 sends it to the Default Router R1 by placing the IP Packet into an Ethernet Data-Link frame with DMAC as R1's MAC.
* **R1 Processes the incoming Frame & Forwards the packet to R2:**
  * R1 receives & accepts the frame with DMAC as his own MAC & processes the Frame.
  * First R1 checks the FCS errors, if none, R1 de-encapsulate the Ethernet Header & Trailer compares the DIP \(150.150.4.10\) referring to its Routing Table & finds the entry for Subnet 150.150.4.0.
  * Because R1 has a Route to reach that Network it forwards the packet to the interfaces listed in that matching Route \(Serial 0\) which leads the packet to next-hop Router R2 \(150.150.2.7\).
  * R1 will Re-encapsulate the packet with HDLC Header & Trailer then pass it on to R2 on the Serial Link.
* **R2 Processes the incoming Frame & Forwards the packet to R3:**
* After receiving the Frame R2 will repeat the general Process, it will check the FCS field for the FCS errors, if none, R2 de-encapsulate the HDLC Header & Trailer compares the DIP \(150.150.4.10\) referring to its Routing Table & finds the entry for Subnet 150.150.4.0.
* Because R2 has a Route to reach that Network it forwards the packet to the interfaces listed in that matching Route \(Fa0/0\) which leads the packet to next-hop Router R3 \(150.150.3.1\).
* R2 will Re-encapsulate the packet with Ethernet Header & Trailer then pass it on to R2 on the Fast Ethernet Link.
* **R3 Processes the incoming Frame & Forwards the packet to PC2:**
* Link R1 & R2, R3 check the FCS field for the FCS errors, if none, R2 de-encapsulate the Ethernet Header & Trailer compares the DIP \(150.150.4.10\) referring to its Routing Table & finds the entry for Subnet 150.150.4.0 mapped to its own Ethernet interface.
* R3 refers to the ARP table to check the mapping of MAC Address with PC2's IP Address 150.150.4.10 & then finally Re-encapsulate the packet with Ethernet Header & Trailer then pass it on to PC2 with Destination Address of PC2's MAC.

## Reference:

CCNA 200-301 OCG, Volume 1, Pg. 71 - Wendell Odom.

