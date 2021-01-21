# Elect One/Multiple Designated Ports on each Non RB:

### Criteria:

* **Port with the lowest cost to reach RB**

  **Tie Breaker:**

* **Lowest Local BID**
* **Lowest Local Port Priority**
* **Lowest Local port Number**
* **If however it is connected through a HUB then election goes to the lowest interface STP/RSTP priority and, if that ties, the lowest internal interface number \(this scenario is very unlikely\)**
* As mentioned [earlier ](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/how-stp-works)that to prevent loop STP puts an interface either in Forwarding or Blocking mode. To do that it elects a RB first then Elect Root Port on each Non RB & then finally Elect One/Multiple Designated Ports on each Non RB.
* RB will send it's cost as 0 in BPDU, & the receiving Switches will add their port's cost to it then calculate accordingly.
* The Designated port of each LAN segment is the port that advertises the lowest-cost Hello onto a LAN segment to reach the RB.
* One or Multiple ports of a Non-Root Bridge will be marked as Designated Ports & hence will be put in the forwarding state to keep the links between each Switch up for forwarding traffic onto a network segment & the remaining ports will be blocked by default.
* E.g. SW1 is a RB \(with the lowest MAC 001\). Hence the opposite ports of SW1 will automatically become Root Port \(gig0/2 of SW2 & gig 0/1 of SW3\). Now for Designated port election between gig 0/2 of SW3 & gig0/1 of SW2 both will send their cost in Hellos & the Switch which utilizes least cost to reach the RB it's port will be marked as Designated Port \(Gig0/1 of SW2\) & neighbor Switch's port will be marked as Non-Designated \(Gig0/2 of SW1\) & hence will be blocked.

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 222- Wendell Odom.

