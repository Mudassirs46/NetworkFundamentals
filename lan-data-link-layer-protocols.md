# LAN Data-Link Layer Protocols

The most commonly used LAN [Data-Link Layer](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/data-link-layer) protocol is Ethernet & WAN Data-Link Layer protocols are High-Level Data Link Control \(**HDLC**\) and Point-to-Point Protocol \(**PPP**\). 

* Ethernet Frame is Ethernet Header+Trailer encapsulating the Data.

  **Ethernet**

  | Preamble | SFD | DMAC | SMAC | Type | Data & PAD | FCS |
  | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
  | 7 Bytes | 1 Byte | 6 Bytes | 6 Bytes | 2 Bytes | 46-1500 Bytes | 4 Bytes |
  |  |  | Header |  |  | Data | Trailer |

  **Preamble:**

* For Synchronization
* To provide 5MHz clock timing which allows the receiving Computer/device to lock the incoming bitstream.
* It looks like this **\(10101010 10101010 10101010 10101010 10101010 10101010 10101010\)**

  **SFD \(Start Frame Delimiter\):**

* The last ON bit of this field Signifies that the next byte begins the DMAC or DMAC is incoming.
* It looks like this **\(10101011\)**

### DMAC

* The Receiver of the Frame

  **SMAC**

* The Sender of the Frame

  **Type**

* Type of Layer 3 Network Layer packet \(IPv4/IPv6\).
* The Frame is however in a Hexadecimal format so instead of putting 'IPv4'/'IPv6', they put Ether type as **0800 for IPv4** & **86DD for IPv6**. These  **DIFFERENT ETHER TYPES are assigned by IEEE for different Protocols**.
* By looking at this type of field a Networking device that received the frame understands which Protocol stack it belongs to \(IPv4/IPv6\)

  **Data & PAD**

* L3PDU \(Data+IP Header\) + PAD to meet the minimum length requirement of the Data  Field \(i.e. 46 Bytes\)

  **FCS\(Frame Check Sequencing\)/ \(CRC Errors\):**

* To check transmission error.
* Errors occur when Frame's bits changes due to Electrical interference or due to Corrupt NIC.
* Sender's Ethernet Trailer applies a complex Math formula to the frame & store the results in the FCS field & then send it.
* The Receiver on the other side applies the same Math Formula after receiving the Frame & then compares the Sender's results with its own results.
* If the results are the same then the frame is Accepted or else it will show the errors as CRC Errors & Discard them as a Corrupt Frame.

## Reference:

CCNA 200-301 OCG, Volume 1, Pg. 49-50,52-53 - Wendell Odom.

