# RSTP \(Rapid Spanning Tree\)

RSTP \(802.1W\) in the enhancement of STP \[\[202012071223h STP \(Spanning Tree Protocol\)\]\] \(802.1D\)

* RSTP was crated by IEEE to get rid of the slow convergence of STP where it takes 50 seconds to bring the port up from Discarding \(Blocking\) to Forwarding state. \[\[202012071227a RSTP Port States\]\]
* RSTP convergence is in few seconds \(3 Hello Timers\) or withing few milliseconds of a Physical Link failure.
* It does it so quickly because there is no Listening mode in RSTP. Ports can directly move from Discarding mode to Learning & Forwarding Mode.
* RSTP is backwards-compatible with standard STP \(you can run STP & RSTP in the same Network\)
* RSTP has inbuilt Cisco proprietary features like Backbone fast, Uplink fast, Portfast, BPDU Filter.
* In RSTP, Not only RB but all the other Non-Root Bridges will also be sending & receiving the BPDUs to make the convergence faster.
* RSTP Port roles \[\[202012071226b RSTP Port Roles\]\] are slightly different as compared to STP
* RSTP is enabled by default on newer Cisco Switches which skips the Listening & Learning State that means PortFast \[\[202012071226a PortFast\]\] is also enabled by default on RSTP running Switches on Edge ports.
* Another method of preventing Loop / preventing hackers attack is using BPDU Guard \[\[202012071226aa BPDU Guard\]\]

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 229-233 - Wendell Odom.
* RST Notes
* [https://vimeo.com/ondemand/ccna200301/397383697?autoplay=1](https://vimeo.com/ondemand/ccna200301/397383697?autoplay=1)

