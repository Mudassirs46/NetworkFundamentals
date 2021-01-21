# VLAN

### What is VLAN?

* VLAN is nothing but a single Broadcast Domain or a Single Subnet.
* To understand VLAN we must first understand LAN. [LAN](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/lan) is nothing but a single Broadcast Domain in which if any of the device [sends any frame](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/ethernet-lan-switching), all the other devices gets the copy of that frame.

  **Why VLAN?**

* And as we know Switch is a single Broadcast domain device. When received a Broadcast/Multicast frame on it's port it forwards it to all the other ports.
* If we have a large LAN where there are 50,000 computers & to connect them we have to use 2500 Switches of 20 port each. On such a large Network if any mistake happens then it's impact will be on the whole campus because all the computers are initially the member of same VLAN \(VLAN1\).
* But if we divide this large LAN into smaller virtual LANs we not only break the Broadcast domain but we also get the 
* **Broadcast Control, Segmentation, Flexibility & Security for our LAN.**
  * **Broadcast Control & less Memory, CPU & Bandwidth utilization:**
    * By default if a broadcast frame from one VLAN will never be forwarded to the other VLAN. Hence we get a good broadcast control which reduces the Memory, CPU, Bandwidth utilization by getting rid of unnecessary Broadcast frames.
  * **Segmentation:**
    * If we roll out any changes in a particular VLAN & if any mistake happens then the impact will be this VLAN \(segment\) only & will not be faced by the other VLANs.
  * **Flexibility:**
    * Managing a LAN Network with 50,000 computers is a not only Strenuous \(demanding or requiring vigorous exertion\) but troublesome. Hence, managing small VLANS are more smooth and uncomplicated than one large LAN.
  * **Security:**
    * Because the Broadcast sent in one VLAN will not be forwarded to the other VLANs hence it also improves the security as frames are seen by lesser hosts.
* Switch does VLAN tagging in which they add [802.1Q Header ](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/trunk-port)to the frame  include VLAN ID so that the receiving Switch can then know what VLAN this frame belongs. 
* If you want to forward a packet from one VLAN to another VLAN on a different Switch \(SW1's VLAN 10 to SW2's VLAN 20\)  then you need to Route those frames between the Switches.
* VLAN can be [configured ](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/configuring-vlan)in 2 Ways: Full Method & Short Method
* [VTP](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/vtp-vlan-trunking-protocol) is a Cisco proprietary tool on Cisco switches that advertises each VLAN configured in one switch \(with the vlan number command\) so that all the other switches in the campus learn about that VLAN. 
* In an IP Phone, PC is in Data VLAN & IP Phone is in [Voice VLAN](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/voice-vlan) & the Switch port with which it is connected to acts sort of like a [Trunk](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/trunking-protocol-802.1q) port carrying traffic from 2 different VLANs.

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 176,179-180 - Wendell Odom. 
* RST Notes

