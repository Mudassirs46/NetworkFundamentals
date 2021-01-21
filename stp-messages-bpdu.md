# STP Messages \(BPDU\)

STP \[\[202012071223 Why STP\]\] messages are called BPDU \(Bridge Protocol Data Unit\). BPDU contains BID \(Bridge Priority + MAC Address\)

* BID is 8 Byte in size. MAC Address is 6 byte, hence the remaining 2 bytes are Priority.

### Hello BPDU contains the following fields:

1. **RB ID**
   * Bridge ID of the Root Bridge
2. **Sender's BID**
   * BID of the switch sending this BPDU
3. **Sender's Root Cost**
   * STP cost between this Switch & the current Root
4. **Timer Values on the RB**
   * Hello Timer, Max Age Timer, Forward Delay Timer

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 218- Wendell Odom.

