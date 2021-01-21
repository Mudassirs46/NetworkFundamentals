# HUB

* When the first 10BASE-T \(Twisted Pair Cable\) connection was introduced in 1990 providing the first 10Mbps connection, HUB was the first device used with a HALF Duplex logic before the other [Networking devices](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/types-of-networking-devices) were invented.
* HUB is an L1 device because it uses Physical Layer Standards rather than Data-Link Layer Standards.
* When received a frame on its port, HUB just like a Dumb Repeater copy & forward \(repeat\) it to all the other ports except the incoming port. Hence it is also called a Multi-Port Repeater.
* HUB is a Half-Duplex device as it does not have any mechanism of Collision Detection/Avoidance, Hence if 2 Frames are sent at a time to a HUB \(usually the case in FULL-Duplex devices\) the Frame just collides.
* Hence to the neighbor device connected to a HUB must always set it's Duplex settings to Half-Duplex.

## Reference:

CCNA 200-301 OCG, Volume 1, Pg. 55 - Wendell Odom.

