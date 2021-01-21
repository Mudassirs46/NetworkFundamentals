# CLI Modes

* After accessing the [CLI](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/cisco-cli) using either of the three Access Methods \(Console, Telnet & SSH\), user will be initially placed in the User EXEC Mode/User Mode where user has only Read-Only Access. Then there are additional 2 Modes, Enable Mode/Privileged Mode/Privileged EXEC mode, Global Configuration Mode where a user gets the access to configuration.

### User Mode/ User EXEC Mode \(&gt;\):

* When a user gets the access to CLI they are initially placed in User EXEC Mode/User Mode.
* Only display commands work here & in return Switch/Router executes \(where it got this name\) those commands & displays the result as this mode has Read-Only Access.

  **Enable Mode/Privileged Mode/Privileged EXEC mode \(\#\):**

* An advanced version of EXEC Mode/User Mode where a user gets more privileges \(where it got this name\) like Rebooting a Router/Switch from '\#Reload' command. 
* To get in the Enable/ Privileged/ Privileged EXEC mode, user has to type in '&gt;Enable' \(where it got this name\) in EXEC/User Mode. Similarly, to get back to EXEC/User Mode user needs to type in '&gt;Disable'.

The commands that can be used in either **User Mode/ User EXEC Mode** or **Enable Mode/Privileged Mode/Privileged EXEC mode** are called EXEC Commands.

### Global Configuration Mode \(conf t\):

* The only mode where Switch/Router accepts the configuration as the User gets the full access to the Router/Switch.
* Generally, when multiple commands \(instances\) of a parameter are to be set in a single Switch then SUBCOMMAND is likely used to set the parameters \(E.g. host name Command\). However, if a Single instance command are to be used for a single instance of a single Switch then GLOBAL command is likely used to set the parameters\(E.g. interface speed Command\).

  **The User Mode and Privileged Mode can be secured in the following ways:**

* Using password only
* Using Username & Password

  \([Securing CLI Modes](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/securing-user-mode-and-privileged-mode)\)

* Using External Authentication Servers

  \([AAA Server](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/aaa-authentication-authorization-and-accounting-server)\)

## Reference:

CCNA 200-301 OCG, Volume 1, Pg. 91-92,97,99 - Wendell Odom.

