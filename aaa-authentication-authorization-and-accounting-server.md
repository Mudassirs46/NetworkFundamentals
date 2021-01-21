# AAA \(Authentication, Authorization and Accounting\) Server

In an Enterprise Network where there are hundreds of thousands of Switches so it is not possible to configure/change the passwords regularly & Secure the CLI \[\[202012050654 Securing CLI Modes\]\] on each and every device manually/locally.

* AAA servers centralize the Authentication of the user of a Network \(hold the usernames/passwords of all the devices of that Network\). 
* It authenticates the password before a user can access the Network.
* AAA Server like Cisco ACS \(Access Control Server\) Servers uses 802.1x Protocols like RADIUS \(Remote Authentication Dial-In User Service\) / TACACS+ \(Terminal Access Controller Access-Control System Plus\) for authentication \[\[202012050659 AAA 802.1x Protocols \(Radius & TACACS+\)\]\]. 
* AAA Server may use Local Data Base or AD for storing those Usernames & passwords.

  **Flow:**

* PC \(also running 802.1x compliant Software\) will put in the Username & Password & try to login the Switch/Router \(Authenticator\) using Telnet/SSH. 
* Switch then forwards that frame \(without reading\) to the AAA Servers using 802.1x Protocols like RADIUS / TACACS+ for authentication/approval of those Username/Passwords. 
* If credentials matches then AAA Server will reply in affirmation to Switch \(Authenticator\) which then permits the client to the Network.

## Reference:

* CCNA 200-301 OCG, Volume 1, Pg. 136 - Wendell Odom.
* [https://courses.davidbombal.com/courses/267624/lectures/4159176](https://courses.davidbombal.com/courses/267624/lectures/4159176)

