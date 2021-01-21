# Trunking Protocol \(802.1Q\)

Cisco has supported 2 different trunking Protocol.  Inter-Switch Link \(ISL\) and IEEE 802.1Q.

* Both does the same work but differently. ISL encapsulates the frame whereas 802.1Q inserts the frame. ISL is obsolete now on newer Cisco Switches.
* [Trunk port](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/trunk-port) runs 802.1Q & does VLAN Tagging in which they insert the 4 bytes 802.1Q VLAN header in the original Ethernet Frame.
* In that header it includes the 12-bit VLAN ID field.
* This 12 bit field supports a maximum of 2^12 i.e. 4096 VLANs of which VLAN 0 \(hex value: 0x000\), VLAN 1 \(hex value: 0x001\) & 4095 \(hex value: 0xFFF\) VLANs are reserved.

| VLAN RANGE | USE | TYPE |
| :---: | :---: | :---: |
| 0&4095 | Reserved for system use |  |
| 1 | Cisco default \(Management\), \(VTP & CDP Messages\), \(Native VLAN\) |  |
| **2-1001** | **Ethernet VLAN** | **STANDARD VLAN** |
| 1002-1005 | Reserved for FDDI & Token Ring \(Native\) |  |
| **1006-4094** | **Ethernet VLAN** | **EXTENDED VLAN \(VTP ONLY\)** |

### VLAN 0 \(hex value: 0x000\):

* VLAN 0 indicates that the frame does not carry a VLAN ID. Hence, 802.1Q refers this tag as a priority tag.

  **VLAN 1 \(Native VLAN\) \(hex value: 0x001\):**

* VLAN 1 is reserved for management VLAN. 802.1Q does not add the it's own VLAN header to the frames belonging to the Native VLAN just to provide the basic connection to the devices that does not understand 802.1Q Trunking & also to get the Telnet/SSH Access to those Switches.

  **VLAN 4095 \(hex value: 0xFFF\):**

* VLAN 4095 is reserved for the port group of a Virtual Machine \(VM\). This port is connected to a Switch's Trunk port on one end & all the different VM Server on the other. Traffic from all the VLANs are carried from Trunk till this port & then as VM is not a Switch it is then forwarded to 4095 VLAN.
* There are 2 ways to configure a Trunk Port. 1. Statically using \(\#switchport mode trunk\) & another is dynamically using [DTP](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/dtp-dynamic-trunking-protocol).
* In an IP Phone, PC is in Data [VLAN](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/vlan) & IP Phone is in [Voice VLAN](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/voice-vlan) & the Switch port with which it is connected to acts sort of like a Trunk port carrying traffic from 2 different VLANs.
* If the native VLANs differ according to the two neighboring switches, the switches will cause frames sent in the native VLAN to jump from one VLAN to the other.
* \(E.g. If switch SW1 sends a frame using from it's native VLAN 1 on an 802.1Q trunk, SW1 will send it without the VLAN header as it is a Native VLAN. When switch SW2 \(whose Native VLAN is VLAN 2\) receives the frame without the 802.1Q header, will assume it is for native VLAN & forward the frame to VLAN 2 straight away. This is called VLAN Hopping.

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 180-183,205 - Wendell Odom. 
* [https://networkengineering.stackexchange.com/questions/24404/vlan-0-1-and-4095-are-reserved-what-are-they-reserved-for](https://networkengineering.stackexchange.com/questions/24404/vlan-0-1-and-4095-are-reserved-what-are-they-reserved-for)
* [https://youtu.be/N31yloKN0hE](https://youtu.be/N31yloKN0hE)

