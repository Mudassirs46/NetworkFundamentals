# Voice VLAN

### Old Phone:

* In older technology desks usually had a PC connected to an Ethernet Switch. Video conferencing kit to a MCU & a Non-IP Phone connected to a Voice Switch called PBX \(Private Branch Exchange\).
* Both PBX & Ethernet Switch sometimes used to sit in the same closet.

  **New Phone:**

* The next generation architecture now provides \(voice,video & data\) Triple play service over  a single infrastructure \(wire\).
* Now in this updated technology desks have PC connected to an Ethernet Switch/Wifi & IP Phone like an end user computer is also connected to an Ethernet Switch/Wifi.
* IP Phones sends & receive voice using IP Packets through their Ethernet ports & the CUCM \( Cisco Unified Communication Manager\) software replaced the PBX management but tagged with an 802.1Q header. 
* One port of the IP Phone is connected to the PC & another to the Ethernet Switch placed in the wiring closet.
* In an IP Phone, PC is in Data [VLAN](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/vlan) & IP Phone is in Voice VLAN & the Switch port with which it is connected to acts sort of like a [Trunk](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/trunking-protocol-802.1q) port carrying traffic from 2 different VLANs.

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 196-197 - Wendell Odom. 

