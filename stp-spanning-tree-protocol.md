# STP \(Spanning Tree Protocol\)

Hello BPDU are send every 2 seconds which contains Root cost, BID & RB ID.

* RB creates & sends Hello BPDU with root cost as 0 out to all it's working interfaces \(those in forwarding state\)
* Remaining Non-Root Bridges will receive this Hello on their Root Port.

   Non-Root Bridges will then create & forward Hello BPDU including their Root cost, their BID as sender BID & RB ID to all their Designated Ports.

* Step 1 & 2 repeats until something changes.
* STP goes through these following [States ](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/stp-rstp-states)initially as well as during the convergence.
* [RSTP ](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/rstp-rapid-spanning-tree)is the enhancement of STP.
* If you don't want your ports to be blocked by STP/RSTP then you may use [Ether Channel](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/ether-channel) Protocols
* You can enable [PortFast ](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/portfast)manually on STP running Switch's Edge ports to skip the un-necessary Listening & Learning State.
* Another method of preventing Loop / preventing hackers attack is using [BPDU Guard](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/bpdu-guard)
* There are different types of [STP Versions](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/stp-spanning-tree-protocol-versions) 
* Lets take a look at [Why STP](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/why-stp) , [What STP does](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/what-stp-does), [How STP does it](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/how-stp-works) & [STP Messages](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/stp-messages-bpdu)
* And finally how an Admin can change the [STP Settings ](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/changing-the-stp-settings)Statically
* STP uses [STP TImers](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/stp-convergence-if-something-changes-link-fails) after the convergence.

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 225-226- Wendell Odom.

