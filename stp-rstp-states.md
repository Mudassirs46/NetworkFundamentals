# STP/RSTP States:

STP \[\[202012071223h STP \(Spanning Tree Protocol\)\]\] moves an interface from blocking to listening, then to learning, and then to forwarding state.

* **Disabled Port State:**
* Disabled ports are Administratively disabled \(shut\) by an Admin. 
* Disabled Port wont be able to Send/Receive any BPDU, Learn MAC Address or Forward Data Packets.

### Blocking State:

* Non-Designated Ports are in a Blocking State to block the port on the loop to break the loop.
* Initially all the ports are in a Blocking State but even after Election one port is blocked and that is the Non-Designated Ports which is then again put in the Blocking State.
* In Blocking State, Non-Designated Ports will just be able to receive the RB BPDUs but won't be able to Receive any BPDU, Learn MAC Address or Forward Data Packets.

  **Listening State:**

* After 20 seconds of Max-Age timer port goes from Blocking to the Listening State.
* In Listening State, ports will send and receive BPDUs in those 15 seconds but won't be learning MAC Address or Forward Data Packets.
* The switch removes old stale \(unused\) MAC table entries for which no frames are received from from each MAC Address during this period which may cause the temporary loops.

  **Learning State:**

* In Learning State, ports will send & receive BPDUs & will also learn the MAC Address in those 15 seconds but won't be able to Forward the Data Packets.

  **Forwarding State:**

* Root Ports & the Designated Ports are in Forwarding State.
* In Forwarding State, ports will not only be able to Send & Receive the BPDUs but will also be able to Learn the MAC Addresses & Forward the Data Packets.

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 227 - Wendell Odom.
* [https://vimeo.com/ondemand/ccna200301/397383497?autoplay=1](https://vimeo.com/ondemand/ccna200301/397383497?autoplay=1)

