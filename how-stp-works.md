# How STP works?

[Previously ](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/why-stp)we understood STP's [main job ](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/what-stp-does)is to Block a port on the loop to break the Loop & to do that STP puts the port either in Forwarding mode or in the Blocking mode in.

* Initially STP's STA \(Spanning Tree Algorithm\) creates a \(spanning\) Tree structure of ports that  are in the forwarding State to & from each Ethernet link just like the structure of a tree from the base to it's each leaf.
* That means [STP](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/stp-spanning-tree-protocol) only works on deciding which interface to put in the forwarding State & then simply put the rest in a Blocking State.
* As all the L2 switches does the same L2 functions hence there must be some criteria just for the sake of formality or for the sake of election.
* **3 Criteria to put an interface in a Forwarding Mode:**
* \*\*\*\*[**Elect a RB**](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/electing-a-rb-root-bridge-switch)**:** 
* \*\*\*\*[**Elect One Root Port on each Non RB**](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/electing-one-root-port-on-each-non-rb)**:**
* \*\*\*\*[**Elect One/Multiple Designated Ports on each Non RB**](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/elect-one-multiple-designated-ports-on-each-non-rb)**:** 

  | Root Port | Designated Port |
  | :--- | :--- |
  | Least path cost from Non-RB to reach the RB | Lowest STP Cost |
  | Single port on each Non-Root Bridge | Single/Multiple Port on every Switch |
  | No Root Ports on the RB | All ports of the RB are Designated Ports |
  | Root Port's opposite end will always be a Designated Port | Designated Port's opposite end will either be a Designated/Non-Designated |

* **Remaining Ports will automatically be elected as Non-Designated Ports & STP will put them in the Blocking State to avoid Loop.**
* Failed interfaces \(interfaces with no cable installed\) or administratively shutdown interfaces are placed in disabled state not to be confused with the shut down state\)

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 216-217, 223 - Wendell Odom.
* [https://www.omnisecu.com/cisco-certified-network-associate-ccna/difference-between-root-port-and-designated-port.php\#:~:text=The Root Port is the,Root Bridge \(Root Switch\).&text=There can be ONLY one,on a Bridge \(Switch](https://www.omnisecu.com/cisco-certified-network-associate-ccna/difference-between-root-port-and-designated-port.php#:~:text=The%20Root%20Port%20is%20the,Root%20Bridge%20%28Root%20Switch%29.&text=There%20can%20be%20ONLY%20one,on%20a%20Bridge%20%28Switch)\).
* [https://community.cisco.com/t5/switching/stp-root-port-vs-designated-port/td-p/1517842](https://community.cisco.com/t5/switching/stp-root-port-vs-designated-port/td-p/1517842)
* [https://vimeo.com/ondemand/ccna200301/397383326?autoplay=1](https://vimeo.com/ondemand/ccna200301/397383326?autoplay=1)

