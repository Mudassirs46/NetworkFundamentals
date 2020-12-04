# Router

1. A Router is an Intelligent Device.
2. As soon as a Router receives a packet on its port it will read IP Address Refer Routing Table & take the Forwarding decision.
3. IP Address is a L3 Address, Routing Table is a L3 Table. Hence, a Router is a L3 [Networking device](untitled-33.md).
4. On receiving a packet on its port Router will open L3 information, Refer Routing Table & forward the packet only if it has a route to reach that Network or else discard it.
5. Because Router refers Routing Table to take the forwarding decision hence Routing Table should be populated with Routes. 
6. Switch switches within the Subnet & Router routes between the Network. Because Router routes between the Network hence every port of Router must be in the different Network. No two ports of the Router can belong to the same [Subnet](untitled-42.md).  
7. Routers will never forward a broadcast received on a port to other ports. The Router has been created to break the Broadcast Domain. 
8. Every port of a Router is a member of a separate collision domain, similarly, every port of a Router is a member of a Separate Broadcast Domain hence Router is a multiple Collision & Broadcast Domain Device.
9. Multiple Ports of a Router can have the same MAC Address or Multiple MAC Addresses.

### The Route can be populated in 3 ways:

* Directly connected Routes will automatically reflect in the Router's Routing Table. 
* An Administrator can make Static Rote Entry in Router's Routing Table
* [Dynamic Routing Protocols](untitled-43.md) will learn Routes Dynamically in the Router's Routing Table.

## References:

RST Notes

