# Trunk Port

### Why use Trunk Port?

* Initially each VLAN requires a port between the Switch. So 20 VLANs takes up 20 ports just between the 2 Switches.
* Now if we have 20 computers of 20 different VLANs of SW1 to the 20 different VLAN on another 20 different computers then no ports are left as all the ports are taken by switches connecting each other.
* Hence we use Trunk port.

### What is a TRUNK Port?

* Trunk port is a port which is the member of multiple VLANs.
* Trunk port runs [802.1Q](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/trunking-protocol-802.1q) & does VLAN tagging in which they insert the 802.1Q VLAN Header to the Ethernet frame which includes the VLAN ID so that the receiving Switch can then know what [VLAN](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/vlan) this frame belongs & it removes the 802.1Q VLAN header, refer the VLAN ID & forward the frame out to the interface belonging to that particular VLAN. 

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 180-182 - Wendell Odom. 
* RST Notes

