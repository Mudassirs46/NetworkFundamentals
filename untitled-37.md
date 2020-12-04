# WAN Data-Link Layer Protocols

* The most commonly used WAN [Data-Link Layer](untitled-18.md) protocol is Ethernet & WAN Data-Link Layer protocols are High-Level Data Link Control \(**HDLC**\) and Point-to-Point Protocol \(**PPP**\). 
* The two most commonly used WAN Data-Link Layer protocols are High-Level Data Link Control \(**HDLC**\) and Point-to-Point Protocol \(**PPP**\).
* On WAN Links Ethernet Frames are De-encapsulated & Re-encapsulated [HDLC Encapsulating and Re-encapsulating](untitled-38.md) with HDLC Header&Trailer or they use EoMPLS to avoid Serial Technology using HDLC WAN Protocol.

## HDLC \(Cisco Proprietary\)

| Flag | Address | Control | Type | Data | FCS |
| :---: | :---: | :---: | :---: | :---: | :---: |
| 1 Byte | 1 Byte | 1 Byte | 2 Bytes | \(Variable\) | 2 Bytes |
|  |  | Header |  | Data | Trailer |

### Flag \(Eq to Preamble+SFD of Ethernet\):

* For Synchronization
* To provide 5MHz clock timing which allows the receiving Computer/device to lock the incoming bit stream.

  It looks like this \(10101010 10101010 10101010 10101010 10101010 10101010 10101010\)

### Address \(Eq to DMAC of Ethernet\):

* Identifies the destination device.

### Control \(N/A\):

* no longer in use today

### Type \(Eq to Type of Ethernet\):

* Type of Layer 3 Network Layer packet \(IPv4/IPv6\).
* The Frame is however in a Hexadecimal format so instead of putting 'IPv4'/'IPv6' they put Ether type as 0800 for IPv4 & 86DD for IPv6. These DIFFERENT ETHER TYPES are assigned by IEEE for different Protocols.

### FCS \(Eq to FCS of Ethernet\):

* To check transmission error.
* Errors occurs when Frame's bits changes due to Electrical interference or due to Corrupt NIC.
* Sender's Ethernet Trailer applies a complex Math formula to the frame & store the results in the FCS field & then send it.
* Receiver on the other side applies the same Math Formula after receiving the Frame & then compare the Sender's results with it's own results.
* If the Results are same then the frame is Accepted or else Discarded as a Corrupt Frame.

## Reference:

CCNA 200-301 OCG, Volume 1, Pg. 63 - Wendell Odom.

