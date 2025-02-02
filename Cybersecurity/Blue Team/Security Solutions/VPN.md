# VPN Overview

A Virtual Private Network is a technology that creates a private and secure communication channel a user's end device and a remote server or network

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/1_uoTideZRhY7hXrho-9wbFg.png)

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/38KzTKwGStyh7poKFy3CYQ_c8c29cb17ed54105b78f3e2b84afd8e1_M2L1_04_img3.png)

* Increases privacy by concealing personal information (Ex: *IP addresses*, *etc.*)
* Provides a server that acts as a gateway between a computer and the Internet, which creates a path similar to a virtual tunnel that hides the computer's IP address and encrypts the data in transit to the Internet
* Enables trusted and encrypted connections to be established on non-trusted networks
* The secure tunnel varies per protocol
* Uses a process called encapsulation, which wraps a user's encrypted data in an unencrypted data packet enabling their data to be sent across a public network while remaining anonymous

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/Whitespace.png)

# VPN Components

## VPN Client

A VPN client is a software installed on a user device that's responsible for initiating and establishing the VPN connection

* Encrypts outgoing data and decrypts incoming data

## VPN Gateway

A VPN gateway is a network device that's located at the edge of the private network and is responsible for handling incoming VPN connections

* Authenticates users and devices
* Manages encryption and decryptin of VPN traffic
* Routes decrypted data to the appropriate destination within the private network

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/Whitespace.png)

# VPN Tunneling Protocols

A VPN tunneling protocol is a protocol that defines the method used to encapsulate and transmit data securely over the public network

## IPsec

The Internet Protocol Security is a suite of protocols that's used to secure IP communications in order to ensure the confidentiality and integrity of data transmitted over IP networks

* Operates at the Network layer of the OSI model (Layer 3)
* Allows entities to authenticate each other in order to ensure that the communication remains between trusted parties and to prevent unauthorized access to network resources

## L2TP

The Layer 2 Tunneling Protocol is a tunneling protocol that's used to establish VPNs or provide remote access to network resources over a public network by creating a tunnel between a VPN client and a VPN gateway over an existing IP network

* Operates at the Data Link layer of the OSI model (Layer 2)
* Often used in conjunction with IPsec to provide security features (Ex: *Encryption*, *Authentication*, *etc.*)

## PPTP

The Point-to-Point Tunneling Protocol is a networking protocol developed by Microsoft that's used to create VPN tunnels between two devices over a public network

* Uses the GRE protocol to encapsulate frames within a VPN client's IP packets in order to transmit data packets over the internet
* Uses the Microsoft Point-to-Point Encryption encryption algorithm the encrypt the data payload of each packet in order to secure the data transmitted over the VPN tunnel
* Supports various authentication methods (Ex: *MS-CHAP*, *EAP*, *etc.*)

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/Whitespace.png)

# VPN Implementation Types

## Policy-based VPN Implementation

A policy-based VPN is a type of VPN implementation that operates based on predefined security policies or rules

* Uses predefined security policies or rules to match VPN traffic
* Traffic is sent over a pair SAs, one which is used to each direction of traffic, meaning that you can have different rules for different types of traffic between two devices

## Route-based VPN Implementation

A route-based VPN is a type of VPN implementation that uses routing protocols to dynamically determine which traffic should be sent through the VPN tunnel

* Uses routing tables to decide how to route VPN traffic through the tunnel (Ex: *Target matching based on prefix*, *etc.*)
* Each network prefix has a single pair of SAs, meaning that all traffic types between two devices use the same pair of SAs
* Provides less functionality but is much simpler to set up

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/Whitespace.png)

# Types of VPNs

## Remote Access VPN

A remote access VPN is a type of VPN that enables devices to connect to a private network securely from a remote location through the Internet

* Usually used to establish a connection between a personal device and a VPN server
* Encrypts data sent and received through a personal device
* Typically uses TLS
* Requires a VPN client software to be installed on end devices in order for them to be able to form secure tunnels to one of the organization's routers or firewalls that's acting as a TLS server
* Provides service to the one end device that the VPN client software is installed on
* Typically used to provide on-demand access for end devices that want to securely access company resources while connected to a network that isn't secure

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/Whitespace.png)

## Site-to-Site VPN

A site-to-site VPN is a type of VPN that connects entire different LANs together, creating a virtual network-to-network connection

* Creates a secure communication channel between LANs of different locations, allowing them to function as a single, unified network
* Used to extend a network to other networks and locations 
* Useful for enterprises that have offices across the globe
* IPSec is commonly used to create an encrypted tunnel between the primary network and the remote network
* Can be complex to configure and manage compared to remote access VPNs
* Typically uses IPsec
* Provides service to many devices within the sites that they're connected to
* Typically used to permanently connect two sites over the Internet

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/Whitespace.png)

# VPN Solutions

## SSL VPN 

An SSL VPN is a type of VPN that allows users to access web applications via a web browser

* Operates at the Application layer of the OSI model (Layer 7)

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/Whitespace.png)

## OpenVPN

OpenVPN is an open-source VPN software that provides a secure and reliable way to establish encrypted connections over a public network

* Supports client-to-server and site-to-site VPN deployments

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/Whitespace.png)

## IPsec VPN

An IPsec VPN is a type of VPN that utilizes IPsec protocols to establish secure connections over the internet

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/gdfhgfjfhgkjghkghdfgrdtytyuiyiyuf.png)

* Provides a secure tunnel for transmitting data between two endpoints
* Supports only unicast traffic
* Can support broadcast and multicast traffic using Generic Routing Encapsulation (GRE), which can encapsulate a wide variety of Layer 3 protocols as well as broadcast and unicast messages but in plaintext (Using GRE over IPsec encrypts encapsulates the GRE packet within an IPsec VPN header and a new IP header)

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/Whitespace.png)

## L2TP VPN

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/Whitespace.png)

## PPTP VPN

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/Whitespace.png)

## WireGuard VPN

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/Whitespace.png)

## Dynamic Multipoint VPN

DMVPN is a Cisco-developed solution that allows routers to dynamically create a full mesh of IPsec tunnels without having to manually configure every single tunnel

* Provides the configuration simplicity of hub-and-spoke, meaning that each spoke router only needs one tunnel configured
* Provides efficient direct spoke-to-spoke communication, meaning that spoke routers can communicate directly without traffic passing through the hub
