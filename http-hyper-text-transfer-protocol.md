# HTTP \(Hyper Text Transfer Protocol\)

TCP/IP Application Layer's \[\[202011170304 Application Layer\]\] HTTP was built in the early 1990s by Tim Berners-Lee who gave HTTP the functionality to ask for the contents of a Web Page from a Web Server & also to provide Server a the way to return the contents of those files.

* The default Web pages are stored in a file called home.htm in every Web Browser.
* When you hit any website from a Web Browser then PC automatically sends a 'Get' request in it's HTTP Header \(encapsulated by Application Layer\), asking a Web Browser for a Web & if no Filename is mentioned the Server assumes that the default Web Page of that website is being requested.
* In turn Server replies with a return code '200' in it's HTTP Header meaning 'OK' & then another reply follows the actual Data but this time omitting the HTTP Header to avoid the wastage of Space.
* Return codes are used by the Web Server to tell the Web Page whether the request worked or not.

## Reference:

CCNA 200-301 OCG, Volume 1, Pg. 20 - Wendell Odom .

