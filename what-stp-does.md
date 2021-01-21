# What STP Does?

Previously in \[\[202012071223 Why STP\]\] we understood STP's \[\[202012071223h STP \(Spanning Tree Protocol\)\]\] main job is to Block a port on the loop to break the Loop. Let us understand What STP does to break that Loop.

* **To break the Loop STP put interfaces of each Switch either in a Forwarding State or in a Blocking State.**
* **Forwarding State:**
  * In Forwarding State ports are Forwarding & receiving the Frames.
* **Blocking State:**
  * In Blocking State ports are not Forwarding Frame. Ports however receiving the Frames but keep on discarding them \(except STP/RSTP & and some other overhead messages\).
* If however something changes in the LAN \(e.g. a running link goes down\) then the STP convergence process can also bring the blocked ports up form the Blocking to the Forwarding State.
* Lets take a look at What How works \[\[202012071223b How STP works\]\]

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 215-216 - Wendell Odom.

