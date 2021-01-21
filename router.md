# Router

1\) Router is an Intelligent Device. 2\) As soon as a Router receives a packet on it's port it will read IP Address Refer Routing Table & take the Forwarding decision. 3\) IP Address is a L3 Address, Routing Table is a L3 Table. Hence, Router is a L3 Networking device \[\[202011231827 Types of Networking Devices\]\]. 4\) On receiving a packet on it's port Router will open L3 information, Refer Routing Table & forward the packet only if it has a route to reach that Network or else discard it. 5\) Because Router refers Routing Table to take the forwarding decision hence Routing Table should be populated with Routes.

### Router can be populated in 3 ways:

i\) Directly connected Routes will automatically reflect in Router's Routing Table. ii\) Administrator can make Static Rote Entry in Router's Routing Table iii\) Dynamic Routing Protocols will learn Routes Dynamically in Router's Routing Table. \[\[202012010859 Routing Protocol\]\]

6\) Switch switches within the Subnet & Router routes between the Network. Because Router routes between the Network hence every port of Router must be in the different Network. No two ports of the Router can belong to the same Subnet \[\[202012010809 Subnetting\]\]. 7\) Routers will never never forward a broadcast received on a port to other ports. Router has been created to break the Broadcast Domain. 8\) Every port of a Router is a member of seperate collision domain, similarly every port of a Router is a member of a Seperate Braodcast Domain hence Router is a multiple Collision & Broadcast Domain Device. 9\) Multiple Ports of a Router can have same MAC Address or Multiple MAC Addresses.

* Router/Switch contains 4 different Types of Memory \[\[202012011008 Cisco Memory Types\]\].

## References:

RST Notes

