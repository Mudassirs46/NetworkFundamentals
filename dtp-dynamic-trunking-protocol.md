# DTP \(Dynamic Trunking Protocol\)

There are 2 ways to configure a Trunk Port. 1. Statically using \(\#switchport mode trunk\) & another is dynamically using DTP \(Dynamic Trunking Protocol\).

* DTP auto negotiates between the two trunk ports to form a trunk port. There are 2 modes in DTP. DTP mode auto & DTP mode desirable. 
* In DTP Desirable mode Switch asks first to the other end to form a trunk or else it becomes an Access port. 
* In DTP Auto mode it waits until the other end Switch asks first or else it becomes an Access port.  

  **Trunk configuration:**

* **Select the type of Trunking \(802.1Q/ISL/Negotiate \(using DTP\)\):**
  * Command is \(\# switchport trunk encapsulation \([dot1q ](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/trunking-protocol-802.1q)/isl/negotiate\)
* **Select the Administrative Mode:**
  * **Always use Trunk \(Statically\)**
    * Command is \(\# switchport mode trunk\)
  * **Always not use Trunk**
    * Command is \(\# switchport mode access\)
  * **Negotiate \(Dynamically using DTP\)**
    * Command is \(\# switchport mode desirable\)

      \(asks \(negotiates with\) the other end to trunk & if negotiation success then it forms a Trunk or else it becomes an access port\)

    * Command is \(\# switchport mode auto\)

      \(wait until the other end asks \(negotiates\) to be a trunk or else it becomes an access port\)
* To check Trunk port settings \(\#show interfaces gigabitEthernet 0/1 switchport\)

#### The individual combinations of port settings lead to following results:

* dynamic auto + dynamic auto = access
* dynamic auto + dynamic desirable = trunk
* dynamic desirable + dynamic desirable = trunk
* dynamic auto or dynamic desirable + trunk = trunk
* dynamic auto or dynamic desirable + access = access

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 180-183 - Wendell Odom. 
* [https://community.cisco.com/t5/switching/why-dtp-is-used/td-p/1377495](https://community.cisco.com/t5/switching/why-dtp-is-used/td-p/1377495)

