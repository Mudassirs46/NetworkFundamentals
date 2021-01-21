# Electing a RB \(Root Bridge/Switch\)

### Criteria: Switch wit the Least Priority

### Tie Breaker: MAC Address

* As mentioned [earlier](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/how-stp-works) that to prevent loop STP puts an interface either in Forwarding or Blocking mode. To do that it elects a RB first.
* Initially when all the Switches come up they start exchanging BPDU \(Bridge Priority + MAC Address\) & all the switches will put their own BID as a Root Bridge ID.
* If a Switch hears a Hello that lists a lower BID, then that Switch stops advertising it's own BID as RB ID & starts forwarding their own BID as well as the Superior Bridge's Hellos as a Root Bridge ID.
* Eventually by exchanging Hellos, Switch with the least Priority \(32768 default Priority\) becomes a RB. If Priority is same then the election goes on to the MAC Address which acts as a tie breaker.
* By default all the ports of a Root Bridge will be marked as Designated Ports & hence will always be in the forwarding state

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 218,219- Wendell Odom.
* RST Notes, Volume 2

