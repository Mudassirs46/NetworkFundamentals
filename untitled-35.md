# SWITCH

* A Switch is a L2 [Networking device](untitled-33.md) because it uses Data-Link Layer standards. Meaning Switch refers to MAC Addresses \(which is a Layer 2 Address\) & MAC Table \(which is a Layer 2 Table\)
* When a Switch receives a Frame on its port it refers to the Frame \(Header&Trailer\) & forwards the Frame to the relevant Port only and not to all other ports.
* The Switch supports Half-Duplex as well as Full-Duplex logic.
* To Avoid/Detect Collisions Switch uses CSMA/CA & CSMA/CD algorithms.
* The Neighbor device connected to a HUB must always set it's Duplex settings to Half-Duplex. Hence if a Switch is connected to a HUB it must always set its port connected to that HUB to a Half-Duplex setting.

  1\) Switch is an intelligent device. 

  2\) As soon as a switch receives a frame on its port it will read MAC Address refer to MAC Table & take the forwarding decision.

  3\) MAC Address is a L2 Address, MAC Table is a L2 Table, Hence Switch is a L2 Device.

  4\) On receiving a Frame on its port switch will open L2 information, Read DMAC Address, refer MAC Table & forward the frame to the relevant port only & not to all other ports. Whereas the HUB will forward it to all other ports.

  5\) Switch segments the Network whereas HUB extends the Network.

  6\) Because Switch refers to the MAC Table hence MAC Table should be populated with MAC Addresses.

  7\) MAC Table can be populated in 2 ways:

  i\) Administrator can make Static MAC entry in MAC table.

  ii\) Switch does self-learning of MAC entry in MAC Table when a Frame traverses a Switch.

  8\) Huge MAC Table has 3 issues: High Memory utilization, High CPU utilization & Frame forwarding delay.

  9\) To overcome these issues cisco defined 4096 MAC entries in the MAC Table anything. And any MAC entry in MAC Table that is not sending Frame in 5 mins will be considered as Stale & will be removed from the MAC Table.

## Reference:

CCNA 200-301 OCG, Volume 1, Pg. 55-56 - Wendell Odom.

