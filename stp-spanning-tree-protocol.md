# STP \(Spanning Tree Protocol\)

Hello BPDU are send every 2 seconds which contains Root cost, BID & RB ID.

* RB creates & sends Hello BPDU with root cost as 0 out to all it's working interfaces \(those in forwarding state\)
* Remaining Non-Root Bridges will receive this Hello on their Root Port.

   Non-Root Bridges will then create & forward Hello BPDU including their Root cost, their BID as sender BID & RB ID to all their Designated Ports.

* Step 1 & 2 repeats until something changes.
* STP goes through these following States \[\[202012071226 STP Port States\]\] initially as well as during the convergence.
* RSTP \[\[202012071226ab RSTP \(Rapid Spanning Tree\)\]\] is the enhancement of STP.
* If you don't want your ports to be blocked by STP/RSTP then you may use Ether Channel Protocols \[\[202012071228 Ether Channel\]\]
* You can enable PortFast \[\[202012071226a PortFast\]\] manually on STP running Switch's Edge ports to skip the un-necessary Listening & Learning State.
* Another method of preventing Loop / preventing hackers attack is using BPDU Guard \[\[202012071226aa BPDU Guard\]\]
* There are different types of STP Versions \[\[202012071225 STP Versions\]\]
* Lets take a look at Why STP \[\[202012071223 Why STP\]\] , What STP does \[\[202012071223a What STP Does\]\], How STP does it \[\[202012071223b How STP works\]\] & STP Messages \[\[202012071223c STP Messages \(BPDU\)\]\]
* And finally how an Admin can change the STP Settings Statically \[\[202012071223g Changing the STP Settings\]\]

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 225-226- Wendell Odom.

