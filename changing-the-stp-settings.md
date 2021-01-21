# Changing the STP Settings:

#### There are 2 tools available to change the [STP ](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/stp-spanning-tree-protocol)Settings:

1. Configure BID
2. Configure STP Port costs

### Configure BID:

* BID consists of Bridge Priority + MAC Address. We cannot configure MAC Address as it is a burned in MAC Address. Hence we can change the priority of a Switch.
* Default Priority is 32768 
* Admin can reduce the Priority to make that Switch a Root Bridge.

### Configure STP Port costs:

* Default Port Costs:

| Ethernet Speed | IEEE Cost: \(1998 & Before\) Short Path Cost Method Port Cost | IEEE Cost: \(2004 & After\) Long Path Cost Method Port Cost |
| :--- | :--- | :--- |
| 10 Mbps | 100 | 2,000,000 \(2 Million\) |
| 100 Mbps | 19 | 200,000 \(2 Hundred Thousand\) |
| 1 Gbps | 4 | 20,000 |
| 10 Gbps | 2 | 2000 |
| 100 Gbps | N/A | 200 |
| 1 Tbps | N/A | 20 |

* Reduce the port cost to favor the link & increase the port cost to avoid the link.
* You can change the Short/Long port cost by using \(\#spanning-tree pathcost method \(short/long\)\) command.

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 223-224- Wendell Odom.

