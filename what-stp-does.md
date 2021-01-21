# What STP Does?

[Previously](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/why-stp) we understood [STP's](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/stp-spanning-tree-protocol) main job is to Block a port on the loop to break the Loop. Let us understand What STP does to break that Loop.

* **To break the Loop STP put interfaces of each Switch either in a Forwarding State or in a Blocking State.**
* **Forwarding State:**
  * In Forwarding State ports are Forwarding & receiving the Frames.
* **Blocking State:**
  * In Blocking State ports are not Forwarding Frame. Ports however receiving the Frames but keep on discarding them \(except STP/RSTP & and some other overhead messages\).
* If however something changes in the LAN \(e.g. a running link goes down\) then the STP convergence process can also bring the blocked ports up form the Blocking to the Forwarding State.
* Lets take a look at [How STP works](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/how-stp-works)

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 215-216 - Wendell Odom.

