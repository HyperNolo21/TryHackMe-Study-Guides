# Room Name: Introductory Networking 
Date: 5/20/2026
Path: Concepts 
Difficulty: Easy

---

# Objective
What was the goal of this room/lab?
Go Over Basic Topics
A brief introduction into Networking 




---

# Key Concepts Learned

## Concept 1
Definition/explanation in your own words.

Example:
### IP Address
An IP address identifies a device on a network.

Concept 1:

OSI Model: Open Systems Interconnection, its a model which is used to demonstrate the theory behind computer networking 

It has seven layers: 
My mnemonic i came up for it was A Puncher shoots to not die patiently 
Physical: this is the hardware of the computer, its the job of the physical layer to convert the binary data of the transmission into signals and transmit them across the network, as well as receiving incoming signals and converting them back into binary data.
Which layer transmits and receives data 1 it is 1 

Data Link: The datalink layer focuses on the physical addressing of the transmission. Receives the packet from the network layer which includes the (IP address for the remote computer) and adds in the physical (MAC) address of the receiving endpoint its the job of the data link layer to present the data in a format suitable for transmission it also has one more job which is to make sure thwart the received information hasnt been corrupted during transmission which could happen when the data is transferred to the physical layer.
In which layer would data be formatted in preparation for transmission? 2 it is 2  

Network: The internet is a huge network so when you want to request information from a webpage, the network layer is responsible for location of the destination of your request, it is the IP address for the page and figures out the best route to take. Logical Addresses are used to provide order to networks. Categorizing them and allowing us to properly sort them. The most common type of logical addressing is the IPv4 format.

Transport: Its first purpose is to choose the protocol over which the data is to be transmitted Which is either TCP(Transmission Control Protocol) or UDP (User Datagram Protocol) With TCP the transmission is connection based Also the TCP connection allows the two computers to remain in constant communication to ensure that the data is sent at an acceptable speed. With UDP the opposite is true: packets are thrown at the receiving computer and that's why some videos are pixelated if the connection is bad. That's why TCP would be chosen for situations where accuracy is favoured over speed like file transfer or loading a webpage, where UDP would be used for more speed like video streaming,




Session: The Session layer receives the formatted data from the presentation layer, it looks around to establish a connection with any other computers in the network if it cant it will send back an error but if a session can be established then this layers job is to maintain it, also to cooperate with the session layer of the other computer in order to synchronize the communications. Also the session layer is able to create multiple requests at different endpoints without all the sessions getting mixed up like having multiple tabs open.

Presentation: The presentation layer receives data from the application layer and it has to decrypt the data into standardized format and also handles any encryption compression with this data.

Application : It provides networking options to programs running on a computer only works with applications  

Which layer would the FTP ( File Transfer Protocol( protocol communicate with? 7 its 7 

---




## Concept 2
Definition/explanation.

Encapsulation: The process by which data can be sent from one computer to another
:::;Data being passed down each layer of the model and more details from that specific latter is added through the transmission. 

When the message is received by the second computer, it reverses the process it reverses the OSI model to translate the data this is referred as de-encapsulation 

— UDP is for Datagram and TCP is for Segment. I think for it more as UDP = University Department Police for Datagram like tech stuff and i just pair the other together.



TCP = Transmission Control Protocol 
It controls the flow of data between two endpoints, and the internet protocol, which controls how packets are addressed and sent. 

TCP is connection based so before you send any data via TCP, you must first form a stable connection between two computers. Like when using Wireshark, and this process is a called the three-way handshake.

Making a Connection to a remote server
Our Server sends a request to the remote server, this request contains a SYN{Synchronise ) 
Which the SYN makes the first contact in the connection process.
The remote server will the respond contained with a packed containing the SYN bit but also an another “Acknowledgement” bit, called ACK.
Finally your computer will send a packet that contains the ack bit by itself, confimding that the connection has been setup successfully.
And with that the threeway handshake has been complete and data can be reliably transmitted between the two computers. 

Also any data that is lost or corrupted on transmission is re-sent, thus leading to a connection which appears to be lossless

Which layer of the TCP/IP model covers the functionality of the transport layer of the OSI model? Transport


## Concept 3
Definition/explanation.

Ping Tool
The ping command is used to reach out to a remote computer or server to see if the connection is able to be established using the ICMP protocol 

Ping Command-  
The ping command is used when we want to test whether a connection to a remote resource is possible. 
The ICMP protocol is the internet control message protocol it runs on the network layer of the OSI model
ICMP is completely connectionless. There is no session setup, no handshake, and no teardown. 


## Concept 4
Definition/explanation.

Tranceroute:so how i kind of understand it is that traceroute uses a command that shows a map of the routes and which servers it bounced to get to the preferred destination 

Traceroute command:: it can be used to map the path your request takes as it heads to the lab machine. Traceroute allows you to see each of these connections it allows you to see every intermediate step between your computer and the resource you requested.

It is preferred to do it after a ping.





Concept 5
Definition/Explanation

Domains: so a domain is an IP address
Domains are leased out by companies called domain regstars. If you want a domain, you would go and register with a registrar, then lease the domain for a certain length of time 


WhoIS: pretty much allows you to search up the data from who a domain name is registered to. So you can get a great deal of information from a whois search.

Whois: essentially allows you to query who a domain name is registered to. In Europe personal details are redacted; however, elsewhere you can potentially get a great deal of information from a whois search. .

This is comparatively a very small amount of information as can often be found. Notice that we've got the domain name, the company that registered the domain, the last renewal, and when it's next due, and a bunch of information about nameservers (which we'll look at in the next task). 





Concept 6
Definition/Explanation

DNS: how I interpret it is that DNS lets us ask a special server to give us the IP address of the website we're trying to access, like we like if i made a request to docs.google.com. our computer would send a request to a special DNS server then the server would go looking for the IP address and then send it back to us.

DNS:(Domain Name System)- At the most basic level, DNS allows us to ask a special server to give us the IP address of the website we're trying to access. For example, if we made a request to www.google.com, our computer would first send a request to a special DNS server (which your computer already knows how to find). The server would then go looking for the IP address for Google and send it back to us. Our computer could then send the request to the IP of the Google server. 

Our Computer makes a request to a website then our computer checks its local hosts file to see if an already explicit IP-> domain mapping has been created if found then great but The first thing that your computer does is check its local "Hosts(opens in new tab) File" to see if an explicit IP->Domain mapping has been created 
if not our computer will send a request to a recursive DNS server, this server are stored in my router or computer, and this serve twill also maintain a cache of results for popular domains. 
If not that then it will pass a request on to a root name server, the root name servers keep track of the DNS server in the next level down, choosing an appropriate one to redirect your request to. 
These lower level servers are called Top Level Domain servers. And TDL servers are split up into extensions.  Like .com or .co.uk

Dig command
The dig command allows us to manually query recursive DNS servers of our choice for information about domains 
















# Commands Learned

## Command
ping command. 

The Basic syntax for ping is [ping <target>]

TryHackMe


My Version

—----------
##Command
traceroute  
The basic syntax for traceroute on linux is traceroute <destination>

TryHackme

My Version didnt work to well but i still did it 

—----------------


##Command
Whois 
Basic syntax for  this is whois <domain>
TryHackme


My Version 











##Command
Dig Command
dig <domain> @<dns-server-ip>


Tryhackme

We want to be focused on the Answer section of this room
This information is telling we got one query successful unlike mine which got errors. In the Tryhackme they got the IP address for the domain name 
Another thing is we got the TTL(Time to live which is the 157) of the queried DNS record, the TTL of the record tells your computer when to stop considering the record as being valid.












My Version


Then went to WSL and did it with the right public IP Adress



```bash
command here

