# Port Roles in RSTP

### Port Roles in [RSTP](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/rstp-rapid-spanning-tree)

| Port Role | Function |
| :--- | :--- |
| **Root Port** | Same as STP's Root Port \(Port with least Cost to reach the RB. Or else Least BID, Least Port Priority, Least Port Number\) |
| **Alternate Port** | Backup Root port if Root Port fails \(same as Blocking Port \(in discarding State\)\) |
| **Designated Port** | Same as STP's Designated Port \(Port with lowest Cost to reach the RB. Or else Lowest BID, Lowest Port Priority, Lowest Port Number\) |
| **Backup Port** | Backup Designated port if Designated Port fails \(in discarding State\) |
| **Disabled Port** | Same as STP's Port \(Administratively disabled\) |
| **Edge Port** | Ports connected to End devices \(where STP is disabled generally\) |

#### Alternate Port:

* Blocked ports are marked as Alternate Ports which are basically Backup Root Port. 
* If Root Port fails, this Alternate port becomes the RP immediately \(generally in 1 sec\) skipping the Listening & the Learning State.

  **Backup Port:**

* The backup port role is only needed in the designs that are little unlikely today \(E.g. A Switch connected to a HUB with 2 ports \(in same Collision Domain\) & HUB is connected to an End device\). One from amongst these 2 ports will be Designated port and another port will be blocked marked as a backup port. 

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 229-233 - Wendell Odom.
* RST Notes
* [https://vimeo.com/ondemand/ccna200301/397383697?autoplay=1](https://vimeo.com/ondemand/ccna200301/397383697?autoplay=1)

