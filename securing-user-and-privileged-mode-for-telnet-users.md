# Securing User & Privileged Mode For Telnet Users

[User & Privileged CLI Modes are secured ](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/securing-user-mode-and-privileged-mode)for: Console Users, Telnet Users & SSH Users.

* **Using password only**
* \(conf t\)\#enable secret cisco
* \(conf t\)\#line vty 0 15

  ```text
   (conf t)#password cisco
   (conf t)#login(to enable password only without username)
  ```

  **Using Username & Password**

* \(conf t\)\#enable secret cisco \(for securing Privileged Mode\)
* \(conf t\)\#username Mudassir secret cisco 
* \(conf t\)\#line vty 0 15 \(conf t\)\#login local \(to enable username access\)

  \(can use multiple Username & their own passwords\)

## Reference:

CCNA 200-301 OCG, Volume 1, Pg. 130-131 - Wendell Odom.

