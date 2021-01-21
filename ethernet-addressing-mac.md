# Ethernet Addressing \(MAC\)

* Ethernet \[\[202011211558 Ethernet\]\] Address is also called as MAC Address \(Media Access Control\).
* MAC Address is 6 Bytes, 48 bits Hexadecimal Address.  
* This MAC Address is made up of 6 Sets & each Set includes 8 bits of Hexadecimal characters separated by periods.
* MAC Address is pre-programmed in every NIC card.
* IEEE Assigns the first 3 Bytes unique to the NIC card called the Organizationally Unique Identifier \(OUI\). And the manufacturer assigns the remaining 3 Bytes unique to every NIC card that they manufacture.
* In this way, No two NIC card will have the same MAC Address. Hence MAC Address is also called as a Unicast Ethernet Address, LAN address, Ethernet address, hardware address, burned-in address, physical address & universal address.

  **6 Bytes \(48 Bits\) MAC Address:**

  | OUI | Vendor |
  | :---: | :---: |
  | 24bits | 24bits |
  | 00 60 2F | 3A 07 BC |
  | \(6 Hex digits\) | \(6 Hex digits\) |

### Group Address:

Apart from the Unicast Ethernet Address, Ethernet also uses Group Addresses which are divided into two categories:

* **Broadcast Address:**
  * Frame sent to this Address will be delivered to all the devices of that LAN. It is FF:FF:FF:FF:FF:FF
* **Multicast Address:**

  * Frame sent to this Address will be copied & delivered a group belonging to that specific Multicast address & not to all the devices.    

  **Reference:**

  CCNA 200-301 OCG, Volume 1, Pg. 50-51 - Wendell Odom.

