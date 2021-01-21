# Autonegotiation

If we configure Full Duplex & 100 Mbps on SW1 but Full Duplex & 1000 Mbps on it's Neighbor Router's port then communication won't happen because Standards won't match.

* Because, '\#Speed 100' command forces the port to use 100Mbps Fast Ethernet settings which uses only 2 pairs of wires & 802.3u Standard whereas for '\#Speed 1000' command which forces the port to use 1000Mbps Gigabit Ethernet Settings it uses all the 4 pairs of wires & 802.3ab Standard.
* Both the nodes tries to Autonegotiate but if either of the two nodes hears nothing then that node follow the 

  **IEEE Default Autonegotiation rule:**

* **"IF AUTONEGOTIATION FAILS SET 10Mbps SETTING & FOR 10/100Mbps SET HALF DUPLEX SETTINGS "**
  * **SPEED:**

      Switch will sense the speed of it's Neighbor node before using IEEE Autonegotiation & set the same speed as the other node's speed. 

      But if it can't sense the speed then it uses IEEE default Auto Negotiation Rule that says, **"IF AUTONEGOTIATION FAILS SET 10Mbps SETTING & FOR 10/100Mbps SET HALF DUPLEX SETTINGS "**

  * **DUPLEX:**

    10/100 - [Half Duplex](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/half-duplex) 1000 - Full Duplex \(means Gig ports will always use [Full Duplex](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/full-duplex)\)

  * Autonegotiation failure leads to [Duplex Mismatch](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/duplex-mismatch)

## Reference:

CCNA 200-301 OCG, Volume 1, Pg. 140-141, 160 - Wendell Odom.

