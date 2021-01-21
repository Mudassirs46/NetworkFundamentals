# SWITCH

* The Switch is a L2 [Networking device](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/types-of-networking-devices) because it uses Data-Link Layer standards. Meaning Switch refers to MAC Addresses \(which is a Layer 2 Address\) & MAC Table \(which is a Layer 2 Table\)
* When a Switch receives a Frame on its port it refers to the Frame \(Header&Trailer\) & forwards the Frame to the relevant Port only \(**forward-versus-filter** decision\) and not to all other ports \(not to filter\). \(Mentioned in [detail](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/ethernet-lan-switching)\)
* The Switch supports Half-Duplex as well as Full-Duplex logic.
* To Avoid/Detect Collisions Switch uses CSMA/CA & CSMA/CD algorithms.
* The Neighbor device connected to a HUB must always set it's Duplex settings to Half-Duplex. Hence if a Switch is connected to a HUB it must always set its port connected to that HUB to a Half-Duplex setting.
* To perform LAN Switching, Switch performs these 3 actions:
  1. Examine the SMAC & make the entry in the MAC Table
  2. Deciding when to forward or not to forward depending on the DMAC Address
  3. To forward only one copy of the frame to avoid creating a loop Using STP logic.
* The Switch is an intelligent device. 

  2\) As soon as a switch receives a frame on its port it will read MAC Address refer MAC Table & take the forwarding decision.

  3\) MAC Address is a L2 Address, MAC Table is a L2 Table, Hence Switch is a L2 Device.

  4\) On receiving a Frame on its port switch will open L2 information, Read DMAC Address, refer MAC Table & forward the frame to the relevant port only & not to all other ports. Whereas HUB will forward it to all other ports.

  5\) Switch segments the Network whereas HUB extends the Network.

  6\) Because Switch refers to the MAC Table hence MAC Table should be populated with MAC Addresses.

  7\) MAC Table can be populated in 2 ways:

  i\) Administrator can make a Static MAC entry in the MAC table.

  ii\) Switch does self-learning of MAC entry in MAC Table when a Frame traverses a Switch.

  8\) Huge MAC Table has 3 issues: High Memory utilization, High CPU utilization & Frame forwarding delay.

  9\) To overcome these issues cisco defined 4096 MAC entries \(old times\) in the MAC Table anything \(newer Switches like Cisco 2960-XR have bigger CAM \(Physical Space\) hence can store 7299/8000 entries\). And any MAC entry in MAC Table that is not sending Frame in 5 mins will be considered as Stale & will be removed from the MAC Table.

* Router/Switch contains 4 different [Types of Memory](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/memory-types).

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 55-56 - Wendell Odom.
* RST Notes

