# IPv4:

Internet Protocol \[\[202011201239 IP\]\] Version 4 is a L3 Network Protocol of 4 Bytes 32 bits Decimal Address which can produce over 4 Billion \(4,294,967,296\) Unique Addresses.

* This 32 bit IPv4 Address is divided into 4 parts called Octets \(each of 1 byte/8 bits\)
* Those bits in each Octet are represented by a Number.  Starting from the left they have a value of 128, 64, 32, 16, 8, 4, 2, 1.
* Each bit on the octet can be either 1 or 0. If a Number is 1 then that octet is counted if it is a 0 then it is ignored.
* Just by manipulating 1s & 0s in each octet we get a range from 0-255.
* **IPv4 Header:**

  !\[\[Pasted image 20201125174503.png\]\]

* It is a connectionless Protocol which offers only best effort delivery. 
* Each packet is treated differently hence packets may take different paths based on options like Hop Count, Load Balancing or Bandwidth offered by different Routing Protocols.
* IP has no Data Recovery, No built in Sessions & No Re-transmission features. Hence, L3 Internet Protocol relies on the L4 TCP which offers all these features & provides guaranteed delivery of Data & packets.
* Routers route packets based on NID & not HID.
* IPv4 Address is divided into 2 parts: \[\[202011201506 IPv4 Address parts\]\]
  * Network Port \(NID\)
  * Host Portion \(HID\)

## Reference:

* [https://www.youtube.com/watch?v=ThdO9beHhpA&ab\_channel=PowerCertAnimatedVideos](https://www.youtube.com/watch?v=ThdO9beHhpA&ab_channel=PowerCertAnimatedVideos)
* CCNA 200-301 OCG, Volume 1, Pg. 74 - Wendell Odom . 

