# PortFast

It takes 50 seconds to bring a port up from Blocking to Forwarding Mode. It makes sense to use STP/RSTP between the Switches as Loop might occur between Switch to Switch.

* But Loop won't occur between Switch & End devices. So we need a feature to simply disable STP on the Edge ports where no STP enabled devices are connected to bring the port up immediately. 
* Solution is PortFast.
* You can enable PortFast manually on STP \[\[202012071223h STP \(Spanning Tree Protocol\)\]\] running Switch's Edge ports to skip the un-necessary Listening & Learning State.
* RSTP \[\[202012071226ab RSTP \(Rapid Spanning Tree\)\]\] is enabled by default on newer Cisco Switches which skips the Listening & Learning State that means PortFast is also enabled by default on RSTP running Switches on Edge ports.

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 235 - Wendell Odom.
* RST Notes
* [https://vimeo.com/ondemand/ccna200301/397383597?autoplay=1](https://vimeo.com/ondemand/ccna200301/397383597?autoplay=1)

