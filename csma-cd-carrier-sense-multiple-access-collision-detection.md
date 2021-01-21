# CSMA/CD \(Carrier Sense Multiple Access / Collision Detection\):

Two more computers or communicating devices can get connected over the same Medium. 

* All the computers can communicate whenever they feel as if they are in a democratic world.
* But before a computer communicate it has to sense the medium if available & not used by others it can put its frame on the wire, when computers frame it son wire for that instance it is the owner of that entire medium. 
* At that instance, no other computer can talk. When a computer talks all the other computers will listen & only that computer will reply for whom a frame is sent for.
* If the two computers put their frames on the wire on the same instance then these frames will get converted into an electrical signal which is a form of energy that cannot be created nor destroyed but will get distorted. These distorted signals will not vanish off but will be resonated back to all the computers on that link.
* Computers that were sending the signal will start realizing whatever they are sending is getting corrupted & will immediately back off & the computer that detected the corruption first will start pumping jamming pattern on wire & on receiving jamming pattern all the computers will back off & release the medium.
* After releasing the Medium computers will enter the integral wait state. As these wait states are integral so each computer can increase or decrease the wait state depending on the collision.
* If too many communicating devices wanting to communicate so as a good citizen computer will increase its wait state thereby allowing other communicating devices to finish off their communication. If lesser collisions are happening the computers may reduce their wait state.
* These wait states are in the multiple of 51.2 microseconds.
* When [Half Duplex](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/half-duplex) is enabled it enables CSMA/CD because one can either send/receive at a time in Half Duplex settings.

## Reference:

* RST Notes

