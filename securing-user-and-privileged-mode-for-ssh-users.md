# Securing User & Privileged Mode For SSH Users

[User & Privileged CLI Modes are secured ](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/securing-user-mode-and-privileged-mode)for: Console Users, Telnet Users & SSH Users.

* As SSH is a secured alternative of Telnet hence it add the additional credential commands for added security & hence it cannot work with password only.

### To enable SSH on your Router/Switch

1. \(conf t\)\# hostname sw1
2. \(conf t\)\# ip domain-name cisco.com 

   \(SSH uses the host name + domain name to create the key\)

3. \(conf t\)\#crypto key generate rsa general-keys modulus 1024 \(generates key pairs & key modulus size is 360-4096\) \(768 keys at least for SSH v2\)

   \(you may use ''\#ip ssh version 2' command to enable more stable SSH Version\)

### Using Username & Password

1. \(conf t\)\#enable secret cisco \(for securing Privileged Mode\)
2. \(conf t\)\#username Mudassir secret cisco 
3. \(conf t\)\#line vty 0 15 \(conf t\)\#login local \(to enable username access\)

   \(can use multiple Username & their own passwords\)

\(to view SSH Server '\#sh ssh' & to view SSH Clients '\#sh ip ssh'\)

## Reference:

CCNA 200-301 OCG, Volume 1, Pg. 130-131 - Wendell Odom.

