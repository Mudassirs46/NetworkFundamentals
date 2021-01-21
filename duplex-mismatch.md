# Duplex Mismatch:

Duplex & Speed mismatch occurs when [Autonegotiation ](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/autonegotiation)fails because of Duplex&Speed mismatched settings.

* Because of IEEE Autonegotiation rule which says "IF AUTONEGOTIATION FAILS SET 10Mbps SETTING & FOR 10/100Mbps SET HALF DUPLEX SETTINGS "

  **ONLY ETHERNET & FAST ETHERNET MAY FACE DUPLEX MISMATCH BUT GIGABIT & + PORTS WILL NEVER FACE IT.**

  **WHY IT IS NOT RECOMMENDED TO CHANGE DUPLEX/SPEED SETTINGS:**

* The reason why it is not recommended to change the duplex/speed settings is because when you change the duplex/speed settings on a Switch \(E.g. SW2\) then that port's Manual Autonegotiation will stop working \(as it is configured by an Admin Statically\).
* And if you set Duplex Full **BUT** Speed 100 & the neighbor Switch \(E.g. SW1\) tries to Autonegotiate it won't receive any Autonegotiation replies & the SW1 will follow the default steps:
  1. Sense the maximum speed of the neighbor port \(SW2's port\) \(100Mbps\).
     * Will set it's own interface's speed to 100Mbps
  2. Will follow the IEEE Autonegotiation default Duplex Settings:
     * "On 10/100 ports - set Half Duplex setting"
* SW1 will put it's port to Half Duplex but SW2's port is manually in Full Duplex. This leads to **DUPLEX MISMATCH**
* If on one side [Half Duplex](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/half-duplex) is used & [Full duplex](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/full-duplex) on the other Full Duplex port by default will keep sending & receiving frames at the same time whereas Half Duplex by default who uses CSMA/CD will wait until the line is clear before sending the frame & realize collision is occurring & will back off.
* All these collisions & re-transmission are using up all the Bandwidth on the Half Duplex side. You may be able to PING but won't get full Bandwidth.

  \([Verifying Duplex Mismatch](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/verifying-duplex-mismatch)\)

## Reference:

CCNA 200-301 OCG, Volume 1, Pg. 140-141, 161, 165 - Wendell Odom.

