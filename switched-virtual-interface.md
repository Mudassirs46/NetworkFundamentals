# Switched Virtual Interface

You can configure IP Address on a PC & a Router but you cannot configure IP Address on a Switch as it is a L2 device. To configure IP Address on a Switch we use SVI \(Switched Virtual Interface\) \(Software Interface\) \(VLAN Interface\) which is configured on a VLAN \(Virtual Local Area Network\) \[\[202012050661 VLAN\]\]\]\] to get an access to the Switch. \[\[202012050660 Ethernet LAN Switching\]\]

* Initially all the ports are the member of VLAN 1 \(Default/Management VLAN\) used for Telnet/SSH purpose only.
* You may configure multiple VLANs & each VLAN can be configured with separate IP Address.
* An IP Address can be set on SVI \(VLAN interfaces\) either Statically or it can also be fetched dynamically with the help of DCHP with the help of \(\#ip address dhcp\) sub-command.

## Reference:

CCNA 200-301 OCG, Volume 1, Pg. 140-141 - Wendell Odom.

