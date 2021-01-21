# Verifying Duplex Mismatch

#### To check the [Duplex Mismatch](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/duplex-mismatch):

1. Check the duplex setting on each end of the link to see if the values mismatch. 
2. You can also watch for incrementing collision and late collision counters "\#sh interfaces \(_interface_\)"
3. These Duplex mismatch are corrupt frames & no not pass the Error detection by the FCS field.
4. These corrupt frames changes the values in the FCS field while reach the destination device & FCS creates a CRC Error list which further changes the interface counters which is displayed in the "\#sh interfaces \(_interface_\)" command.

   **Types of Error Counters:**

5. **RUNTS:**
   * Frames that did not meet the minimum frame requirement \(64 bytes\)
6. **GIANTS:**
   * Frames that did exceeded the maximum size required \(1518 bytes\)
7. **INPUT ERRORS:**
   * Sum of RUNT+GIANTS+NO BUFFER+CRC+FRAME+OVERRUN+IGNORED COUNT
8. **CRC:**
   * Received frame that did not pass the FCS Math causes the CRC Errors.
9. **FRAME:**
   * Received frame with illegal format \(ending with partial byte\)
10. **PACKET OUTPUT:**
    * Total number of frames forwarded out the interface
11. **COLLISIONS:**
    * Total number of collisions while the interface is transmitting a frame.
12. **OUTPUT ERRORS:**
    * Sum of Frames that the switch tried to transmit but errors occurred due to some problem.
13. **LATE COLLISIONS:**
    * Often points to a Duplex mismatch.
    * These collisions happen after the 64th byte after the frame has been transmitted \(because in a perfectly working Ethernet LAN, collision should occur within the first 64 bytes only\)

## Reference:

CCNA 200-301 OCG, Volume 1, Pg. 166/167 - Wendell Odom.

