# VTP \(Vlan Trunking Protocol\)

VTP is a Cisco proprietary tool on Cisco switches that advertises each [VLAN](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/vlan) \[\[202012050661 VLAN\]\] configured in one switch \(with the vlan number command\) so that all the other switches in the campus learn about that VLAN. 

### Why cisco removed VTP?

* Over the course of decades VTP caused unusual behavior in the VLAN Database. As Server Switches can configure Standard VLAN only & Client Switches cannot configure any VLANs.
* Changing any VTP settings was a hazardous task & any wrong change like deleting a VLAN accidentally may cause the outage in the entire Production LAN.
* Even if we have older Switches, Cisco recommends us to turn off the VTP mode by using \(\#vtp mode transparent\) / \(\#vtp mode off\) command.

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 190 - Wendell Odom. 

