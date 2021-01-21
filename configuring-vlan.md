# Configuring VLAN

### VLAN can be configured in 2 ways:

1. **Full VLAN \[\[202012050661 VLAN\]\] Configuration:**
   * Create a VLAN in VLAN Database \(\#vlan 10\)
   * Assigning VLAN to an interface \(\#int fa0/1\) \(\#switchport access vlan 10\) 
2. **Shorter VLAN Configuration:**
   * Assigning VLAN to an interface \(\#int fa0/1\) \(\#switchport access vlan 10\)

     \(creating a vlan !\)

     Now switch will automatically create a vlan 10 for you
3. If you don't want a port to become a member of Trunk then the command is \(\#switchport mode trunk\)

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 185-189 - Wendell Odom. 

