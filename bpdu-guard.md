# BPDU Guard

An Attacker could connect to one of the LAN Switch's Edge port with Low priority & become the RB & can copy Large number of Data Frames or Forward huge traffic in the LAN.

* Or if mistakenly we connect an inexpensive SW to the Edge port of out LAN Switch which does not use/support STP/RSTP \[\[202012071223h STP \(Spanning Tree Protocol\)\]\] \[\[202012071226ab RSTP \(Rapid Spanning Tree\)\]\] then it may cause a Loop.
* Solution is BPDU Guard.
* BPDU Guard disables the port if any BPDU is received on the Port to prevent the Loop & for security.
* BPDU Guard must be enabled where PortFast is configured \(Edge Port\) that connects the end devices & not the other Switch.

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 236 - Wendell Odom.
* RST Notes
* [https://vimeo.com/ondemand/ccna200301/397383597?autoplay=1](https://vimeo.com/ondemand/ccna200301/397383597?autoplay=1)

