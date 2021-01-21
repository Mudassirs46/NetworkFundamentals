# Securing User & Privileged Mode For Console Users

[User & Privileged CLI Modes are secured ](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/securing-user-mode-and-privileged-mode)for: Console Users, Telnet Users & SSH Users.

**Securing User & Privileged Mode For Console Users:**

* **Using password only**
  1. \(conf t\)\#line con 0

      \(conf t\)\#password cisco

      \(conf t\)\#login\(to enable password only without username\)
* **Using Username & Password**
  1. \(conf t\)\#enable secret cisco \(for securing Privileged Mode\)
  2. \(conf t\)\#username Mudassir secret cisco 
  3. \(conf t\)\#line con 0 \(conf t\)\#login local \(to enable username access\)

     \(can use multiple Username & their own passwords\)

## Reference:

CCNA 200-301 OCG, Volume 1, Pg. 130-131 - Wendell Odom.

