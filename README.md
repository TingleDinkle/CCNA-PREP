# ROAD TO CCNA
My notes while I'm learning about networks, and materials to gain CCNA.

Also some labs and assignments.

Networking today
---------------
- Our usage of phones and internet in general consumes a large time of our day, from the moment of waking up to the moment of going to sleep.
- Convenience, companies could switch from offline working to online working for more efficiency and reach.
- Practically, a world without boundaries, you could reach just about anywhere on Earth.
- Human networking. (expand on this later)

What is a computer network?
---------------------------
- There must be a connection between two or more computing devices with the purpose of transmitting data and sharing information.
- There are two ways to connect: physical wiring or wireless.
- Computing device ex: + computer, phone, server, tablet, tv...etc
|
v
as long as it has data, it can be a computing device and can share and transmit data.

- transmitting data ex: text, file, image, voice, video,..etc

computer network ex: downloading songs to phone using a wire (qualifies as a computer network)

Network components
------------------
Three main components:
1. End devices: Data originates here, then comes through no.2 before finally reaching another end device (end device = computing device)
2. Intermediary Devices: Used to connects end devices.
3. Network media: Transfer data into "waves", more specifically, electrical pulses for metal wires within cables, pulses of light with fiber-optic cables and electromagnetic waves with wireless transmission.

Intermediary devices example: Wireless router, LAN Switch, Router, Multilayer Switch, Firewall Appliance.

Router(or access point) usage: Makes sure the "path" is efficient and makes it's way to the intended end device. (VERY loose definition, needs further clarification).

LAN switch: is ONLY used for connecting, basically nothing else

Multilayer switch: connects using many more switches, aka more pathways aka a switch with many pathways pretty much it.

About VoIP phone: It doesn't take any "data" as a normal IP Phone, but only the sound through network?? (not sure)

Network Representation
----------------------
- Physical topology: the physical location of intermediary devices and cable installation.
  
- Logical topology: illustrates devices, ports, and the addressing scheme of the network.

  
   ![image alt](https://github.com/TingleDinkle/Notes-for-Networking/blob/92a0610e98db5c7f13399e62b22eed4baee91533/image.png)

LANs and WANs
-------------
To do research on:
- Size of area covered
- Number of users connected
  
To NOT do(yet) cuz too hard:
- Number and types of services available
- Area of responsibility

Size(ascending order): PAN->WLAN->LAN->CAN->MAN->WAN

Number of users connected: 1-10->10-100->100-1000->1000-10.000->10.000-100.000->1.000.000-1.000.000.000

very small->small->small-average->average->big->very big

Abbreviation solve for dummies(me): Personal Area Network->Wireless LAN->Local Area Network->Campus Area Network->Metropolitan Area Network->Wide Area Network

Security Threats
----------------
https://docs.google.com/document/d/1Dto63rntqmhdeRu6oYHPh5Jj4sOezSn3L6Pycmb11uE/edit?usp=sharing

The report of Security Threats

Module Objectives
-----------------
Hub: Is the same as a switch, but now less commonly used because of less secure connection.

Switch: Explained in previous notes above, used the most currently along with route.

Route: Same thing as Switch notes.

Networking Devices
------------------
A Network service needs an address(or also known as IP), so they know where to send their data to.

Usually you will be using IPv4.

Networking services example: Vinaphone, Viettel,..etc

Network Interface Card
----------------------
- Is basically a physical hardware that is responsible for handling networks in your device, you almost always HAVE to have it to connect to the internet or wifi.

Hub
---
- Transfer data through multiple ports.

Switch
------
- Have a table that holds all of the information of MACs in different device and saves it to the table once a connection is made.
- Also works through ports but through a table system, which is different from a Hub.

Unrelated note: any LAN networks work with MAC addresses.

Router
------
- Finds the most efficient path to send to the end device that might receive the data through IP addresses. 

For example: your way to school have two ways, one is 5km, one is 10km, yet, the most efficient way is faster in the way that the 10km road is cleaner and there are less vehicles occupying it. Efficiency is the fastest time.

- Connects to IP Addresses outside of the LAN.

 -Gateway-Router-IP

 -Port-Switch

Cisco Packet Tracer:
>: limited

> #: full function

> (config)#: configuration


![image alt](https://github.com/TingleDinkle/Notes-for-Networking/blob/f8401d796d34f8e5cfdab52c0b6952011306c494/image1.png)

Config Settings Report for Cisco Packet Tracer(configuring passwords on routers and switches, configuring SSH on router): https://docs.google.com/document/d/1EqirhWrfimHeYUvpIfVKuo4nJQpftnXeSzVoAxbVuoA/edit?usp=sharing

![image alt](https://github.com/TingleDinkle/Notes-for-Networking/blob/6b4b03e738bdc6ebd4f5d8e61b9a43d3cc2ac742/Screenshot%202025-09-26%20123117.png)

192.168.10.1: IP

255.255.255.0: Subnet Mask

The Rules
---------
Common computer protocols should entails these requirements as follow:
- Message encoding

- Message formatting and encapsulation

- Message size

- Message timing

- Message delivery options

Message Encoding
----------------
- Encoding is converting information into another form for acceptable transmission.

Message Formatting and Encapsulation
------------------------------------
- Encapsulation: ALWAYS go through these 7 layers
 ![image alt](https://github.com/TingleDinkle/Notes-for-Networking/blob/9add4e2c89fdcc92fe674346f636f25acbdfe548/Screenshot%202025-10-03%20155630.png)

Message Size
------------
- Encoding between hosts MUST be in an appropriate format for the medium.

- Messages across the network are converted into bits.

- Bits then are encoded into a pattern of light, sound, or electrical impulses.

- The destination host MUST decode that to then interpret message.

Message Timing
--------------
- Flow Control: Rate of transmission and how much information can be sent and the speed at which it can be delivered

- Response Timeout: How long a device waits when it doesn't get reply from destination.

Message Delivery Options
------------------------
- Unicast: one to one communication.

- Multicast: one to many, usually not all.

- Broadcast: one to ALL.


Lab 3: https://docs.google.com/document/d/1Oo8SUQS7kIzVoNvqmxhO7aJodMuJ3rrG/edit?usp=sharing&ouid=102375238109184631579&rtpof=true&sd=true (finished)

# ULTRA NETWORKING REPORT
https://github.com/TingleDinkle/Notes-for-Networking/blob/6e62d6a7f599559214277c0aed56a4d1c0f32aa2/ULTRA%20NETWORKING%20GRAHH.pdf

# First simple (static) network config successfully!

https://www.youtube.com/watch?v=37izIpHXFRg

# VLAN Config Stuff:

Dividing VLAN:
- Number of devices(expected) = n
  
- 2^(32 - prefix length) - 2 >= n
  
=> prefix length [i...., 32)

IP: host = 0

IP Broadcast: host = 1

First Address: everything...1

Last Address: 1111...0

VTP, or VLAN Trunking Protocol

Switch:

> int ...

> switchport mode access

VTP mode: server/client/transparent

VTP domain: <name_of_domain> (space = death)

VTP password:<pass_word> (space = also death)

trunk: many VLANs

access: 1 VLAN

![image alt](https://github.com/TingleDinkle/CCNA-PREP/blob/d38600efd6eeb3a29dc19e73fd0c2f458d8bbfe0/Screenshot%202025-11-21%20131717.png)

ALTHOUGH mode transparent is rarely used and probably really trash, could be ignored (for now)

Config and settings go into vlan.dat (short for database btw)

Switch core (Multi-layer Switch): Operates at layer 3 in OSI, which means it could work as both a router and a switch.

You use a router to ping between different subnets using a router, which also means you can use a Switch Core to do this.

Config VTP:
> vtp mode server

> vtp domain nyc.com

> vtp password 123

Config VLAN:
> vlan 10

> name Teacher

> vlan 20

> name Staff

> vlan 30
> name CEO

> vlan 100

> name Server

> vlan 50

> name Student

Normal Switch:

Config VTP:
> vtp mode client

> vtp domain nyc.com

> vtp password 123

> do show vlan brief (shows what you have done)

Config trunk:
> int range f0/1-3

> switch trunk encap dot1q (802.1Q)

> switch mode trunk
  
the switch HAVE to be in mode client to access the VTP - Server

which needs domain and password too to actually get the VLAN, so not everyone can just come in and grab it.

# VLAN Network System configuration(in progress):
