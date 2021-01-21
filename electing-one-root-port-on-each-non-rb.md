# Electing One Root Port \(on each Non RB\)

### Criteria:

* **Port with the Least Cost to reach RB**

  **Tie Breaker:**

* **Least Neighbor BID**
* **Least neighbor Port Priority**
* **Least neighbor port Number**
* As mentioned [earlier](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/how-stp-works) that to prevent loop STP puts an interface either in Forwarding or Blocking mode. To do that it elects a RB first then Elect Root Port on each Non RB.
* Root port is the port with the least Root Cost to reach the RB on each Non-Root Switches in that LAN Segment & put them also in Forwarding State.
* The cost is the sum of the costs of all the Switch ports the frame would exit if it flowed over that path \(ignoring the inbound ports\). RB will send it's cost as 0 in BPDU, & the receiving Switches will add their port's cost to it then calculate accordingly. **Cost=In cost+Own Port cost**.

  Root Port leads to Root Bridges directly.

* **If the cost is same for 2 or more paths then Switch applies 3 tie breakers for the Root Port election:**
  1. **Lowest neighbor BID \(upstream \(towards RB\) Switch's BID\)**

     If however there is 1 Neighbor Bridge then BID will be the same.

     * Default Priority is 128, ranges from 0-256 \(multiple of 16\)
     * If the BID will be same then the election goes to Lowest Neighbor Priority 

  2. **Lowest neighbor Port Priority**

     If however there is 1 Neighbor Bridge then Port Priority will also be the same.

     * If the Port Priority will be same then the election goes to Lowest Port Number.

  3. **Lowest neighbor port Number**

     Our Switch's port connected with the lowest numbered Port of the Neighbor Switch becomes the Root Port finally.

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 220-222- Wendell Odom.
* [https://mrncciew.com/2013/07/07/stp-root-port-selection/\#comment-73647](https://mrncciew.com/2013/07/07/stp-root-port-selection/#comment-73647)

