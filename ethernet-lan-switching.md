# Ethernet LAN Switching

As mentioned earlier, When a [Switch](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/switch) receives the frame on it's port it Open the Frame, refer the MAC Table & forward the frame to the relevant port only & not to all the other ports \(not to filter\). This decision is called "**Forward-Versus-Filter**" decision. \(Note: Switch won't refer the MAC Table if it receives the Broadcast Frame FF:FF:FF:FF:FF:FF. It will simply Broadcast it further\).

* **To perform LAN Switching, Switch performs these 3 actions:**
  1. Examine the SMAC & make the entry in the MAC Table
  2. Deciding when to forward or not to forward depending on the DMAC Address
  3. To forward only one copy of the frame to avoid creating loop Using [STP](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/stp-spanning-tree-protocol) logic.

1. Switch creates multiple copies of the Frame in 3 Scenarios:
   1. If it receives a Broadcast Frame
   2. If it receives a Multicast Frame
   3. If DMAC Address is not known in the MAC Address Table. \(unknown-destination uni-

      cast frames\)
2. If sender & receiver are on the same port then Switch will discard the Frame. As Switch switches between the port & not within the ports.
3. If sender & receiver are on the different ports, Switch will bridge the information on the relevant port only & not to all the other ports.
4. Switch works exactly as per the [CSMA/CD](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/csma-cd-carrier-sense-multiple-access-collision-detection) rules, it will sense the port before putting the frame on the wire, will check the CRC code & so on. But with the help of the hardware it overcomes the flaw of CSMA/CD that says only one computer can talk at a time & everybody else will listen.
5. Switch allows simultaneous communications between multiple communicating pairs connected on the different ports.
6. Every port of Switch has it's own dedicated bandwidth, Hence Switch is a Dedicated bandwidth device. 
7. And Every port of Switch is a member of the Separate Collision domain, hence Switch is a Multiple collision domain device but every port of a Switch is a member of the same broadcast Domain hence Switch is a Single Broadcast domain device.
8. You can configure IP Address on a PC & a Router but you cannot configure IP Address on a Switch as it is a L2 device. To configure IP Address on a Switch we use SVI \(Switched Virtual Interface\) \(Software Interface\) \([VLAN ](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/vlan)Interface\) which is configured on a VLAN \(Virtual Local Area Network\) to get an access to the [Switch](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/switch).

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 109-114 - Wendell Odom.
* RST Notes

