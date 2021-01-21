# Memory Types

Cisco OS \(IOS\) \[\[202012011007 Cisco OS \(IOS\)\]\] are stored in different Types of Memory installed in Cisco Switches \[\[202011231919 SWITCH\]\] & Routers \[\[202011251750 Router\]\].

### Four types of Cisco Switch/Router Memory:

1. **FLASH Memory:**
   * FLASH Memory is a Removable/Non-Removable chip which stores the original but Compressed Cisco IOS image. 
   * Some part of FLASH memory can also be used to store the backup config files.
2. **ROM \(Read Only Memory\):**
   * Contains the POST & BOOTSTRAP program which finds the IOS image from FLASH Memory, decompresses & loads the compressed IOS from the Flash Memory to the RAM.
3. **NVRAM \(NonVolatile RAM\):**
   * Stores the Initial/Startup configuration file that is used when the Router/Switch is first powered on/Reloaded.
4. **RAM/DRAM \(Dynamic Random Access Memory\):**
   * Just like the computer's Random Access Memory \(RAM\) which is used to store the running configuration, Cisco's DRAM also does the same job.

## Reference:

CCNA 200-301 OCG, Volume 1, Pg. 99-100 - Wendell Odom.

