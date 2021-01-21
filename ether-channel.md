# Ether Channel

If we paid hefty amount for each individual links between the 2 Switches & all of those links are in Discarding Mode & only 1 is used due to STP/RSTP \[\[202012071223h STP \(Spanning Tree Protocol\)\]\] then we need a port bundling mechanism to group those ports as 1 single port.

* Ether Channel is the solution to bundle multiple ports/links as a single logical link.
* Ether Channel is the logical aggregation of similar links.
* Ether Channel does Load Balancing between those links.
* Ether Channel provides Redundancy for up to 16 links.
* Ether Channel works only on directly connected Switches.
* In STP/RSTP convergence starts as soon as there is a change in Topology/link fails. But now as we are grouping the links & treating them as 1 single link so even if one of the link goes down from a particular group convergence won't start. Convergence will take place only if the entire group/channel goes down.

  **Guidelines:**

* All interface in an Ether Channel must be configured at the same Speed & Duplex.
* All interface in an Ether Channel must support the same allowed range of VLANs.
* In L2 Ether Channel, Interfaces must be assigned to the same VLAN/Configured as Trunk.
* In L3 Ether Channel, IP Addresses must be assigned to port-channel logical interfaces.

### Ether Channel Protocols:

#### PAGP \(Port Aggregation Protocol\):

* Cisco Proprietary works only on Cisco Switches.
* Has Desirable & Auto modes like 802.1Q modes.

  **LACP \(Link Aggregation Control Protocol\):**

* Open Standard works on all the Switches.
* Has Active & Passive modes like Active & Passive Modes of PAGP.

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 234 - Wendell Odom.
* RST Notes
* [https://vimeo.com/ondemand/ccna200301/397383542?autoplay=1](https://vimeo.com/ondemand/ccna200301/397383542?autoplay=1)

