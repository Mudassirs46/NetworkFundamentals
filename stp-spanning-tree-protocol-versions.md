# STP \(Spanning Tree Protocol\) Versions

Although CST is obsolete, now Cisco by default uses RSTP+ from amongst the different [STP ](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/stp-spanning-tree-protocol)Versions.

## 3 STP Versions you can use today:

1. **To use STP you can only use Cisco-proprietary PVST+ \(802.1D\) \(1STP/VLAN\)**
2. **To use Multiple Spanning Tree you can only use IEEE Standard MSTP \(802.1S\) \(1STP/VLAN\)**
3. **To use RSTP you can only use Cisco-proprietary RPVST+\(802.1W\) \(1STP/VLAN\)**
4. Rest other versions are Obsolete !!!

### Year 1990&1998...

### 802.1D

1. **CST \(Common Spanning Tree\): !!! OBSOLETE !!!**
   * One Spanning Tree for the entire Bridged Network. 
2. **PVST \(Per VLAN Spanning Tree\):!!! OBSOLETE !!!**
   * One Spanning Tree per VLAN
   * Only supported ISL
3. **PVST+ \(Per VLAN Spanning Tree Plus\):**
   * Supports ISL & 802.1Q

## Year 2000...

### 802.1W:

1. **RSTP \(Rapid Multiple Spanning Tree Protocol\): !!! OBSOLETE !!!**
   * Faster convergence.
   * One **RAPID Spanning Tree** for the entire Bridged Network. 

     **802.1S:**
2. **MSTP \(Multiple Spanning Tree Protocol\):**
   * Mapping Multiple VLAN on a single Spanning Tree Instance.

## Year 2001...

### 802.1W \(2001\):

1. **RPVST+ \(Rapid per VLAN Spanning Tree Plus\)**
   * One **RAPID Spanning Tree** per VLAN

     **\(DEFAULT VERSION ON CISCO SWITCHES\)**

     \(if you have Thousands of Switches then use MSTP\)

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 241-242 - Wendell Odom.

  [https://courses.davidbombal.com/courses/267624/lectures/4153133](https://courses.davidbombal.com/courses/267624/lectures/4153133)

