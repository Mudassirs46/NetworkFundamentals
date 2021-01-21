# HDLC Encapsulating and Re-encapsulating

Suppose LAN1's PC1 is connected to a distanced LAN2's PC2 through a WAN link with a Router in each LAN connecting these two LANs running HDLC [WAN Data-Link Protocol](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/wan-data-link-layer-protocols) in between.

* Topology is like a BUS Topology where PC1 is connected to a Switch1 then to Router R1. Router R1 is then connected to Router R2 both running HDLC WAN Protocol between each other providing P2P Communication. Router R2 is then connected to Switch2 which is further connected to PC2.
* PC1 will create an Encapsulated Data with Ethernet Header & Trailer & DIP as PC2's IP but DMAC will be Gateway's MAC which will be R1 Router in this case. Similarly, PC2's Gateway will be a R2 Router.
* Ethernet Frame \(with Ethernet Header+Trailer\) will travel from PC1 then at R1 it will be De-encapsulated & Re-encapsulated with HDLC Header & Trailer will travel from R1 to R2 then again De-encapsulated & Re-encapsulated with an Ethernet Header&Trailer then reached to PC2.

## Reference:

CCNA 200-301 OCG, Volume 1, Pg. 65 - Wendell Odom.

