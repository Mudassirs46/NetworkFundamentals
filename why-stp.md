# Why STP?

As mentioned earlier, Switch creates multiple copies of the Frame in 3 Scenarios:

* 1. If it receives the Broadcast Frame
     1. If it receives a Multicast Frame
  2. If DMAC Address is not known in the MAC Address Table. \(unknown Unicast frame/unknown unicast\).
* If 2 Switch connect 2 wires between each other for Redundancy, and because Switch's nature is to create multiple copies of a Broadcast frame if it receives a Broadcast frame that means each switch will receive this Broadcast Frame & the Switches will keep on creating & forwarding these frames thereby creating a **Broadcast Storm & MAC Table instability** which is also called Bridging Loop/ Switching Loop/ L2 Loop. 
* **Bridging Loop/ Switching Loop/ L2 Loop will lead to:**
  1. **Broadcast Storm:**
  2. If the Switch \(SW1\) receives a Broadcast Frame, Multicast Frame, unknown Unicast frame then it create a copy & forward it to all the other ports. If there are 2 links between 2 switches then it kind of creates a circle due to which that broadcast copies are returned back to SW1 & it will again forward it on all the other ports. Creating a broadcast storm with all the links flickering orange LEDs.
  3. **MAC Address Table instability**
  4. PC AAA sends the broadcast frame \(DMAC-FFF\) to SW1's port 1. SW1 will mark in MAC Table that Port 1 is AAA & forward to all the other port including to SW2's port 1. SW2 will receive the frame with SMAC AAA & DMAC FFF & will mark that AAA is @ Port 1 of SW2 & forward it to all the other ports. Because there are 2 links connected between SW1&SW2 now again SW1 will receive this frame at port 4 & will mark that AAA is on port 4 & update it's MAC Table that AAA is not on Port 1 but on Port 4 \(in reality it is on Port 1\). MAC Table instability.
  5. \(Switch will learn the same MAC Address from the different ports as they are creating multiple copies & received on each port on each Switch thereby making the MAC Address Table unstabilized\) 
  6. **Multiple frame transmission:**
  7. Because the same frame is being broadcasted by 2 different Switches & different ports the original receiver will receive same but multiple frames from different senders which may result in an application failure, if not more pervasive networking problems.

     These above issues may also leads to High Memory,CPU & Bandwidth utilization.
* Solution is STP \[\[202012071223h STP \(Spanning Tree Protocol\)\]\]

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 115 - Wendell Odom.
* RST Notes
* [https://courses.davidbombal.com/courses/267624/lectures/4153133](https://courses.davidbombal.com/courses/267624/lectures/4153133)

