# ARP \(Address Resolution Protocol\)

Some other [Network Layer](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/network-layer) features which are related to IP Routing are DNS , ARP & PING.

* Address Resolution Protocol \(ARP\) is a network protocol used to find the MAC address from an IP address of a particular device within the LAN.
* ARP request are broadcast Address sent within the LAN by a Router/Switch simply asking for the MAC Address of an IP Address. And in return an ARP reply is sent by the requested host simply mentioning it's own MAC Address.
* If it is sent by a Router within the LAN then it is sent to the Broadcast Address 255.255.255.255
* If it is sent by a Switch within the LAN then it is sent to the Broadcast Address ff:ff:ff:ff:ff:ff.
* As it is a Broadcast Message so all the devices within the LAN will receive this Address but only the device who's IP's MAC is requested will send the ARP reply containing its own MAC address.
* The mapping of an IP Address & MAC Address is then finally stored in an ARP Table so as to not ask the MAC Address of hosts repeatedly & unnecessarily but the table is flushed occasionally to keep the ARP Table's Mapping updated.

## Reference:

CCNA 200-301 OCG, Volume 1, Pg. 77 - Wendell Odom.

