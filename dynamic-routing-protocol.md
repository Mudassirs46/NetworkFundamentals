# Dynamic Routing Protocol

**Routing Rules:**

* * **Two directly connected devices must be in the same Subnet**

    \(Two IP addresses, not separated from each other by a router, must be in the same subnet\).

  * **Every Port of a Router must be in the different Subnet**

    \(Two IP addresses, separated from each other by at least one router, must be in different subnets\).
* Router's \[\[202011251750 Router\]\] Routing Table should be populated with Routes. 
* **Routes can be populated in 3 ways:**
* Directly connected Routes will automatically reflect in Router's Routing Table.
* Administrator can make Static Rote Entry in Router's Routing Table 
* Dynamic Routing Protocols will learn Routes Dynamically in Router's Routing Table.

| Static Routing | Dynamic Routing Protocol |
| :---: | :---: |
| Use Static Route when Network is simple | Use Dynamic Routing Protocol when Network is complex |
| Static Route paths are selected by an Administrator | DRP are responsible for the best path selection |
| Requires minimum Resources \(Memory,CPU, Bandwidth, etc.\) | Requires sufficient Resources \(Memory,CPU, Bandwidth, etc.\) |

* **Routing Protocols role is:**
  * To learn about all the Networks.
  * To learn about all the paths to reach all the Networks.
  * To select the best path to reach all the Networks.
* Routing Protocol's messages are called Updates.
* **Routing Updates includes:**
* 1. Details of Networks on which Routing Protocol is operating
* 1. Routes that Routing Protocol has received from Neighbors.

## References:

RST Notes

