# RSTP Port States

[RSTP ](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/rstp-rapid-spanning-tree)moves an interface from blocking to learning, and then to forwarding state.

### Discarding State \(Disabled/Blocking\):

* Ports are either Administratively disabled \(shut\) by an Admin or is in Blocking State. \(RSTP names the Disabled & Blocking State both as the Discarding State\)
* Alternate Ports are in a Discarding State to block the port on the loop to break the loop.
* In Discarding State, Alternate Ports will just be able to receive the RB BPDUs but won't be able to send any BPDU, Learn MAC Address or Forward Data Packets.

  **Learning State:**

* In Learning State, ports will send & receive BPDUs & will also learn the MAC Address but won't be able to Forward the Data Packets.
* There is no 15 seconds timer for RSTP Learning State.

  **Forwarding State:**

* Root Ports & the Designated Ports are in Forwarding State.
* In Forwarding State, ports will not only be able to Send & Receive the BPDUs but will also be able to Learn the MAC Addresses & Forward the Data Packets.

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 229-232 - Wendell Odom.
* RST Notes
* [https://vimeo.com/ondemand/ccna200301/397383756?autoplay=1](https://vimeo.com/ondemand/ccna200301/397383756?autoplay=1)

