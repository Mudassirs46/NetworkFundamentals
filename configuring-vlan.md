# Configuring VLAN

### VLAN can be configured in 2 ways:

1. **Full** [**VLAN**](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/vlan) **Configuration:**
   * Create a VLAN in VLAN Database \(\#vlan 10\)
   * Assigning VLAN to an interface \(\#int fa0/1\) \(\#switchport access vlan 10\) 
2. **Shorter VLAN Configuration:**
   * Assigning VLAN to an interface \(\#int fa0/1\) \(\#switchport access vlan 10\)

     \(creating a vlan !\)

     Now switch will automatically create a vlan 10 for you
3. If you don't want a port to become a member of Trunk then the command is \(\#switchport mode trunk\)

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 185-189 - Wendell Odom. 

