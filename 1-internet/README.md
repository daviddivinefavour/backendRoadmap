# INTERNET

## History Of Internet.
The internet originated from an experiment carried out by the defence department. This project was called ARPANET. 
> ARPANET: Advanced Research Project Agency Network
The experiment was aimed at building a communication system that may survive nuclear disasters/attacks. His design was breaking messages into blocks and sending them fast through the meshed network. The messages are scattered into packets(these packets hold small bits of the message as a whole) which are then sent through one origin node, scattered throughout the various nodes of the network and reassemble at the destination node to form whatever was sent as the information in the first place. 

## Components Of The Internet
The internet is made up of a large number of independently  operated networks. This system is **fully distributed**: there is no central network that is controlling the whole.

## Information Transfer on the Internet.
All sorts of information(text,audios,videos,etc) regulated on the internet are transferred from one end to the other as bits(0's and 1's). 
You may ask, how are these bits of information sent? 
Well...they sure aren't sent as emails :), rather they could be sent over the following media;
* Ethernet cables
* Fibre Optic cables 
* Wireless signals(i.e. radio waves)

Considering the fact that the sizes of media files sent over the internet varies greatly, into bits, bytes(8 bits), kilobytes(1024 bits), megabytes(1024 kilobytes), etc. If a person wishes to recieve of transfer information faster, the _bandwith_ of the device being used to access the internet must be increased.
> Bandwidth: The maximum transfer capacity of a device. Bandwidth is measured using bit rate. 

> Bit rate: the total number of bits transferred over a given time, preferably seconds: bit per seconds.

> Latency: is the different amount of speed taken for a piece of information to be transferred from the source to the destination.

## Transfer Media
Earlier we mentioned some media used for transfer of bits, the likes of ethernet cables, fibre optic cables, and wireless transmission.
<table>
	<tr>
		<th>Medium</th>
		<th>Pro</th>
		<th>Con</th>
	</tr>
	<tr>
		<td>Ethernet cables: transmits bit in the form of electric pulses</td>
		<td>Cheap</td>
		<td>Signal loss </br> low signal range</td>
	</tr>
     	<tr>
		<td>Fibre Optic: transmits bits with the speed of light(light waves)</td>
		<td>Extremely fast </br>No signal loss </td>
		<td>Expesive </br> Hard to work with </td>
	</tr>
     	<tr>
		<td>Wireless: transmits bits using radio signals</td>
		<td>Mobile internet</td>
		<td>low signal range</td>
	</tr>
</table> 

## IP Address and DNS
The internet relies on protocols for the transfer and recieval of data. These set of protocols are known as IP(Internet Protocol), it is a set of rules and standards used to communicate between machines. 
Each and every computer on the internet has its own unique address that is used during communication.User1 on his computer sends a request to User2 for a set of information on his own computer. The request is sent to the IP address of User2, and this request also holds the address of User1 to facilitate easy response being sent from User2 back to User1.
**IP ADDRESS:** An IP address has many parts just like every other regular address has many parts making up the address. The IP address is also represented in bits _because it is a digital information_. The IP address is made up of 32bits with each part containing 8bits each e.g 174.129.23.114

> interpretation of each bytes IPv4.

>    * First byte: Country/Network

>    * Second byte: Region/Network

>    * Third byte: Sub-Network

>    * Last byte: Device

The IPv4, though being able to provide up to 4 billion unique IP addresses for users/devices on the internet is definetely not capable of keeping an infinite supply for the indefinite demand of users. 
So therefore, the transition to a newer version of IP address(IPv6) which is made up of 128 bits and capable of providing  up to 340 undecillion unique address (36 zeros, for folks who have never heard of that value before, just like me :stuck_out_tongue:)

Domain Name System(DNS): Is a system that helps the computer to match up the domain names of websites to their corresponding IP address, thereby aiding communication between client and server. 

## Packets, Routers, and TCPs
It was mentioned earlier that information on the internet is not sent as a whole, neither is it sent on a direct connection from the server to the client or vice versa. The information being transferred on the internet is done using packets. 
#### What are packets? 
When data is sent on the internet(lets say a picture), it is broken down into numerous bits and pieces called packets. These packets would follow the routing systems provided by the **routers** to the designated reciever IP address.
#### Routers
Routers are devices along the internet that helps direct packets on the best route possible during the sending or recieval of data. The best route does not neccessarily mean the route with the shortest distance between sender and reciever, it also entails further details, such as, considering the route with less traffic, avoiding congested routes, etc. 
Data packets don't necessarily need to arrive all at once at the destination IP address, as the TCP would handle the recieval and signing of packets.
#### TCP
The TCP can be likened to a strick supervisor that doesn't take cr*p from nobody. TCP(Transmission Control Protocol) is responsible for taking accounts of the packets that got to the destination IP during communication. If the packets recieved is less than the packets sent, it sends a query back to the originating IP requesting for the missing packets. It is only when the missing packets are accounted for that the original data can be assembled from all the data packets.
These makes the internet reliabe and efficient.

## HTTP and HTML
HTTP  is the standard protocol by which webpages are transferred over the Internet. While HTML is the language that is used to tell the browser how the page is to be arranged/formatted.
When a client/user opens the web browser on his device(either smart phone, desktop, laptops, tablets, etc) types an address/URL and hit "enter". What happens under the hood is that your computer starts talking with another computer called a server(and this conversation is completed using a language both the server and browser understand - HTTP). The computer asks the server for the contents of the website in the address using "GET requests", and the response(website) provided is interpreted and arranged by the browser with the help of HTML, thereby making the view of the website understandable for the user.

> HTTP: HyperText Transfer Protocol

> HTML: HyperText Markup Language

> URL: Uniform Resource Locator


## Cryptography/Cryptology
According to wikipedia, it is the practice and study of techniques for secure communication in the presence of adversarial behavior.
Since the internet is an open network(free for all), where everyone and anyone have access to, it is of utmost importance that is secured during communication, as sometimes private data(credit card informaion, etc) is being used while on the internet. 
Without a secured means of communication, these sensitive information can be intercepted by third parties and could be used as they see fit for any ill purposes. 
To secure communication on the internet, user info is usually encrypted before being sent to where such information is needed. And only the intended recipient should have the correct means of decryption of such messages. Cipher is an algorithm that is used for encryption where the each character of the message sent is moved a "key" step forward and for decryption the reciever takes each character of the message sent the same "key" step backwards.
	> Note: the key is agreed upon before hand by the sender and reciever. An example is when both parties agree for the key to be 2, in such a case, "HELLO" becomes "JGNNQ" after it is encrypted.
The problem of using a single digit as key is that a person only needs try a maximum of 26 times to crack the encryption of such message. A new method was thence introduced of using multiple keys per characters of a message(e.g. using 12 keys for every succeeding 12 characters of the message).

#### The concept of public and secret/private keys. 
The internet will always remain an open an open network and no one would have the time to track the server where he is communicating to in order to exchange keys before providing sensitive information. So the method that was utilized was to have a public key that everyone can use to access, encrypt and send information. But each user of the network will have their individual private key used to access and decrypt what ever information is meant for them on the network. This way before a third party can intercept the information meant for user1, such third party must first have access to user1's private key which is nearly impossible is no sensible person would explicitly make his private key known to public.
