# General Vocab
## Study list for tomorrow:
* MAC
* 


* Encoding - transcribing something in a known way that doesnt use keys (eg. in French)

* Steganography - Hiding that there is a message (Lemon juice)

* One-way functions - predetermined codes (Wys for weed)

* KErchoffs' Principle - Assume the enemy knows all about your system, Security must rely soley on the use of keys

* A good cipher - Hide patterns and have a large amount of keys

* One time pad - A truely randomly generated key that is information-theoretically secure \
-> Not used because generating and transmitting that much key would be impractical except for top secret info (Spies)

* Block Cipher - breaks the key down into blocks to encode different parts 

* ECB Mode - Use the same key and algorithm for each block (Creates repitition see a good cipher)

## CIA
* Confidentiality - only those who are authorized to view data can
* Integrity - only those who are allowed can edit data
* Availability - anyone who must view the information has to be able to 

* Authentication = Identification + Authorization 

* Nonce - Number only used once 
* Weakness - Something that has the potential to give an attacker unwanted access (eg. strcpy)

* Vulnerability - a set of one or more weaknesses that allow an unwanted actor to gain access to a system \
-> The intersection of 3 elements: A weakness in the system, a hacker's access to that weakness, and the hacker's ability to exploit it 

* Exploit - a piece of software or technique which allows actors to use a vulnerability (eg. trojan, worm, virus)

* Network Address Translation - converts data from a local ip to a global one, so as to protect data being transmitted to a device

* Port - An address to distinguish different applications running on one machine

* Port Address Translation - like NAT but on a port level 

* Wide Area Network\ 
-> Data Travels over a large area\
-> Connected by telephone cables\
-> Usually requires a Modem

* Local Area Network\
-> Small area\
-> Data travels over network cables\
-> Usually confined to one building or set of buildings

* Virtual Private Network - a private network that extends over a public network by using cryptographic tools

* IPSec - A protocol suite that allows for encrypted communication between two machines\
-> Transport mode - Just the data is encrypted not the IP Packet\
-> Tunnel Mode - The entire IP Packet along with the data is encrypted and sent 

* SSL / TLS - A way to provide application side CIA and is the most common way to provide it on the internet\
-> SSL - A transport layer security service\
-> TLS - The internet standard version of SSL

* SSL Handshake - Allows for a server and client to exchange information (MAC Algorithms, which keys to use)\
-> Establish Security Capabilities\
-> Server Authentication and Key Exchange\
-> Client Authentication and Key Exchange\
-> Finish

* Firewalls\
-> Can: Log traffic, provide a focal point for monitoring, limit damage done\
-> Cannot: Protect against viruses, completely new threats, malicious insiders, or connections that do not go through it 

* Stateful Inspection - A packet inspecting system that checks the system state of all of the connections into a firewall

* Application Gateway - filters traffic at the application level\
-> Offers a high level of security\
-> Tanks network performance

* Circuit level Gateway - gateway that hides internal network \
-> Often used with Application Gateway


* Attacker Methodology \
-> Aim to get increased privelages\
-> Aquire information / get more privelages\
-> Use said privelages or information for personal gain

* Intrusion Detection System (IDS) - The process of monitoring internal system activity to look for signs of an intrusion\
-> Can react in a timely fassion in order to stop or mitigate the attack\
-> Can discover new attack patterns\
-> Can identify a perpetrator and their methods

* Host based vs Network based IDS\
-> HIDS based uses log information (Antivirus) \
-> NIDS based analyses packets

* IPS = IDS + Firewall - Stops attacks before they gain access and alerts when they do 

* 