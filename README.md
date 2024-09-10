<h1 align="center"><a href="https://github.com/f-corvaro/NETPRACTICE">
	<img src="https://github.com/f-corvaro/NETPRACTICE/blob/main/.extra/netpractice.png" alt="NETPRACTICE">
  </a></h1>
  
<p align="center">
	<b><i>"Master the essentials of network configuration and troubleshooting."</i></b><br>
</p>
<p align="center" style="text-decoration: none;">
    <a href="https://github.com/f-corvaro/NETPRACTICE/blob/main/.extra/en.subject.pdf"><img alt="subject" src="https://img.shields.io/badge/subject-NETPRACTICE-yellow" /></a>
    <a href="https://github.com/f-corvaro/NETPRACTICE"><img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/f-corvaro/NETPRACTICE?color=blueviolet" /></a>
    <a href="https://github.com/f-corvaro/NETPRACTICE"><img alt="Code language count" src="https://img.shields.io/github/languages/count/f-corvaro/NETPRACTICE?color=yellow" /></a>
    <a href="https://github.com/f-corvaro/NETPRACTICE"><img alt="GitHub top language" src="https://img.shields.io/github/languages/top/f-corvaro/NETPRACTICE?color=blueviolet" /></a>
    <a href="https://github.com/f-corvaro/NETPRACTICE"><img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/f-corvaro/NETPRACTICE?color=yellow" /></a>
</p>

<h3 align="center">Index</h3>
<p align="center">

- [Introduction](#introduction)
  - [Overview](#overview)
- [Folder Structure](#folder-structure)
- [Project Requirements - Mandatory Part](#project-requirements---mandatory-part)
  - [Getting Started](#getting-started)
  - [Training Levels](#training-levels)
- [Theoretical Background](#theoretical-background)
  - [Quick Overview](#quick-overview)
  - [Fundamentals of Computer Networks](#fundamentals-of-computer-networks)
  - [Basic Operations on Computer Networks](#basic-operations-on-computer-networks)
  - [Types and Topologies of Computer Networks](#types-and-topologies-of-computer-networks)
  - [Reference models](#reference-models)
    - [Open Systems Interconnection (OSI) - A Theoretical Perspective](#open-systems-interconnection-osi---a-theoretical-perspective)
    - [TCP/IP (Transmission Control Protocol/Internet Protocol) - A Practical Approach](#tcpip-transmission-control-protocolinternet-protocol---a-practical-approach)
  - [Data Sharing](#data-sharing)
    - [Network nodes](#network-nodes)
- [Evaluation Process](#evaluation-process)
  - [Peer-Evaluations](#peer-evaluations)
  - [Correction sheet](#correction-sheet)
- [Developed Skills](#developed-skills)
- [References](#references)
- [Support and Contributions](#support-and-contributions)
- [Author](#author)

</p>
<br>

## Introduction

<p align="justify">
NetPractice is a technical project focused on developing and refining networking skills through practical exercises and scenarios. This designed to equip students with a profound understanding of network configuration and troubleshooting. 

</p>
<br>

### Overview 

<p align="justify">
The project covers a wide range of topics, including IP addressing, subnetting, routing, and network troubleshooting. You will have to configure small-scale networks, which requires a solid understanding of how TCP/IP addressing works. The project consists of 10 levels (i.e., 10 exercises) that you will complete and submit to your Git repository. The networks you will work with are not real; instead, they will be available via a training interface that you will access through your web browser. This setup allows for a controlled environment where you can practice and hone your networking skills. The purpose of this project is to solve networking problems and ensure the smooth operation of a network.

</p>
<br>

## Folder Structure

<p align="justify">

```
.
├── netpractice
│   └── level1.json
│   └── level2.json
│   └── level3.json
│   └── level4.json
│   └── level5.json
│   └── level6.json
│   └── level7.json
│   └── level8.json
│   └── level9.json
│   └── level10.json
├── resources
│   └── net_practice.1.5.tgz
├── LICENSE
└── README.md
```

<p>

## Project Requirements - Mandatory Part

### Getting Started

<p align="justify">

First, download the project file from Intra page or directly from [this link](https://github.com/f-corvaro/NETPRACTICE/blob/main/resources/net_practice.1.5.tgz). Next, extract the files to a folder of your choice. In this folder, open the `index.html` file. This will launch the interface in your web browser:

<p>

<p align="center">
<a href="https://github.com/f-corvaro/NETPRACTICE"><img width="650" src="https://github.com/f-corvaro/NETPRACTICE/blob/main/.extra/index.png">
<p>

### Training Levels

<p align="justify">
The training consists of ten levels, each presenting a non-functioning network diagram. At the top of your window, you will see the goal for each level, outlining the issues you need to resolve to ensure the network operates correctly. You have two main buttons at your disposal:

- **Check again**: Verifies whether your configuration is correct.
- **Get my config**: Downloads your current configuration, which is essential for submitting your assignment.

Upon successfully completing a level, a new button will appear, allowing you to proceed to the next level. Before advancing, remember to export your configuration using the **Get my config** button and save it to your Git repository.

At the bottom of the page, you will find logs that can help you understand why your configuration might be incorrect. To succeed, modify the unshaded fields until your network configuration is correct.

To complete this assignment, it is strongly recommended to understand how addressing works in a network, especially with devices such as routers. Make sure to read about TCP/IP addressing.

You can find my NetPractice logs [here](https://github.com/f-corvaro/NETPRACTICE/tree/main/netpractice).

</p>

## Theoretical Background

<p align="justify">

### Quick Overview

The Internet, a vast network of networks, comprises millions of both public and private networks spanning commercial, academic, and governmental sectors. Individuals typically access the Internet via Internet Service Providers (ISPs), which themselves form networks connecting homes, businesses, and other entities within specific geographic areas. These ISPs also connect to higher-level ISPs to gain broader Internet access, creating a hierarchical structure with a handful of level 1 ISPs at the top and hundreds of thousands of lower-level ISPs at the base. The coverage of ISPs can range from global to local scales. Large content providers, such as Google, often establish their own networks and connect directly to lower-level ISPs to reduce costs and enhance connection speeds for their users.

<p align="center">
<a href="https://www.codequoi.com/en/internet-layered-network-architecture/"><img width="650" src="https://www.codequoi.com/images/internet-architecture/internet_devices_routers_switches_hosts_en.drawio.png">
<p>

In any network, including the Internet, a host is any connected system. Hosts can be clients like desktops, laptops, smartphones, or servers that store and distribute data. Data sent from one host to another is divided into packets, which are reassembled at the destination.

Hosts connect via various physical media (coaxial cables, copper cables, optical fibers, radio waves) and data packets often pass through switches and routers. Switches manage data traffic within a network, while routers interface between different networks or sub-networks.

Every host, router, and switch is a network node. The sequence of nodes a packet passes through to reach its destination is its route.

</p>

### Fundamentals of Computer Networks

<p align="justify">

**Node:** In the context of computer networks, a node is any device that can send, receive, or forward information over the network. This includes computers, routers, and switches. 

**Links (connection between nodes):** Nodes are connected to each other through various telecommunication technologies (phisical mediums) including wired (e.g., Ethernet or coaxial cables), optical (e.g., fiber optics), and wireless (e.g., radio waves) methods. The process include these steps: **Digitisation**, **Modulation**, **Transmission** and **Demodulation & Decoding**. The first step is the digitisation of data. This means converting information, which can be text, images, video or any other type of data, into a sequence of bits (0 and 1). Each bit represents an electrical state (on or off) or a light pulse. Once digitised, the data is modulated on a carrier signal. This carrier signal can be an electromagnetic wave (used in wireless transmissions) or a beam of light (used in fibre optics). Modulation consists of modifying certain characteristics of the carrier signal, such as amplitude, frequency or phase, so that digital data ‘travels over’ it. The modulated signal is then transmitted through the physical medium (cables, optical fibres, radio waves). Upon reception, the signal is demodulated to extract the original digital data. Subsequently, this data is decoded and made comprehensible to the receiving device.

**Computer Networks:** The connections between nodes form the network's structure, a collection of interconnected devices that share resources and communicate with each other using common communication protocols. Computer networks enable a wide range of applications and services, including access to the World Wide Web, digital video and audio streaming, shared use of application and storage servers, printers, and fax machines, as well as email and instant messaging.

**Protocols:** Each node in a computer network, whether it's a computer, router, or switch, is identified by a unique network address and may also have a hostname, a memorable label typically assigned during initial setup. These nodes use protocols to send, receive, or forward information over the network. Protocols are sets of rules that dictate how data should be formatted, addressed, transmitted, and received. They also define how to handle transmission errors. Network addresses are used by these protocols, such as the Internet Protocol (IP), to locate and identify nodes. Some common protocols include TCP/IP, HTTP, and FTP.

A **network address** could be an IP address like `192.168.1.1`. This is a unique identifier used by devices to communicate within a network. The **Dynamic Host Configuration Protocol(DHCP) server**  is responsible for assigning IP addresses to devices on a network. When a device connects to the network, it sends a request to the DHCP server, which then assigns an available IP address to the device. The DHCP server keeps track of which IP addresses are currently in use, ensuring that each device on the network gets a unique IP address. If a device disconnects from the network, its IP address is returned to the pool of available addresses and can be reassigned to a different device.

**IP (Internet Protocol):**: Used to identify devices on a network and to route data packets from one device to another. It is a logical address that can change.This is used to communicate between different networks, over the Internet. When you send an email or browse a website, your device uses its IP address to reach remote servers.

**MAC (Media Access Control):** Used to identify a physical device on the local network. It is a unique and immutable physical address. It is used locally, within the same network, to communicate between devices. For example, when you connect an Ethernet cable to your computer, your network card uses its MAC address to communicate with the network switch.

A **hostname** is a more human-friendly label for a device on a network. For example, a server might have the hostname `webserver1`. This hostname can be used to access the server on a local network, provided the network's DNS (Domain Name System) is set up to associate that hostname with the server's IP address.

**DNS (Domain Name System):** It is like a phone book for the internet. Imagine having to remember the IP address (a long sequence of numbers) for every Web site you want to visit, it would be an impractical task. DNS solves this problem by allowing us to use easy-to-remember names such as `www.google.it` instead of a complicated IP address.

**HTTP (Hypertext Transfer Protocol):** is the protocol used for transmitting hypertext over the World Wide Web. It defines how messages are formatted and transmitted, and what actions web servers and browsers should take in response to various commands. For example, when you enter a URL in your browser, this actually sends an HTTP command to the web server directing it to fetch and transmit the requested web page. HTTP uses a stateless request-response model, meaning that each request from a client to a server is processed independently, without any knowledge of the requests that came before it. HTTP is not secure, so it is often replaced by HTTPS, a secure version that uses SSL/TLS protocols to encrypt the communication.

</p>

### Basic Operations on Computer Networks

<p align="justify">

**Addressing** is the process of assigning a unique identifier, such as an IP address, to each device (node). This allows for precise communication between specific devices. Data is sent across the network in small units called **packets**. Each packet contains a portion of the data being sent, along with metadata such as the source and destination addresses. **Routing** is the process of determining the best path for these packets to take from the source to the destination. This is typically handled by devices called routers, which analyze the network's topology and traffic conditions to make this decision. Finally, the **Domain Name System (DNS)** translates human-friendly domain names (like `www.google.com`) into the IP addresses that networks use to route traffic. This makes it easier for users to access websites without having to remember complex IP addresses.

</p>

### Types and Topologies of Computer Networks

<p align="justify">

Computer networks can be categorized based on their size and the geographical area they cover. **Local Area Networks (LANs)** are networks that connect devices over a relatively short distance, such as within a building or campus. **Wide Area Networks (WANs)** cover larger geographical areas, often spanning cities, countries, or even the globe. **Metropolitan Area Networks (MANs)** are larger than LANs but smaller than WANs, typically covering a city or suburb. **Wireless Local Area Networks (WLANs)** are similar to LANs, but use wireless communication methods instead of traditional wired connections. **Storage Area Networks (SANs)** are networks designed to provide access to consolidated, block-level data storage. **Controller Area Networks (CANs)** are vehicle bus standards designed to allow microcontrollers and devices to communicate with each other within a vehicle without a host computer.

<p align="center">
<a href="https://github.com/f-corvaro/NETPRACTICE"><img width="650" src="https://informationq.com/wp-content/uploads/2016/09/Type-of-Computer-Network.jpg">
<p>

The **topology** of a network refers to the arrangement of the network nodes and the physical or logical connections between them. Common topologies include the bus, ring, star, mesh, and tree topologies. Each has its own advantages and disadvantages in terms of complexity, robustness, and cost. In general, the more interconnections there are, the more robust the network is; however, this also increases the cost and complexity of installation. The physical layout of the nodes in a network may not necessarily reflect the logical network topology. 

<p align="center">
<a href="https://github.com/f-corvaro/NETPRACTICE"><img width="650" src="https://systemzone.net/wp-content/uploads/2017/09/network-topology.png">
<p>

</p>

### Reference models

<p align="justify">

Reference models offer a valuable framework for understanding, designing, and troubleshooting computer networks. They promote standardization, modularity, education, and problem-solving.

</p>

#### Open Systems Interconnection (OSI) - A Theoretical Perspective

<p align="justify">

The Open Systems Interconnection (OSI) model is a reference model from the International Organization for Standardization (ISO) that "provides a common basis for the coordination of standards development for the purpose of systems interconnection." In the OSI reference model, communications between systems are split into seven different abstraction layers: Physical, Data Link, Network, Transport, Session, Presentation, and Application.

<p align="center">
<a href="https://github.com/f-corvaro/NETPRACTICE"><img width="650" src="https://media.fs.com/images/community/upload/kindEditor/202107/29/original-seven-layers-of-osi-model-1627523878-JYjV8oybcC.png">
<p>

Each intermediate layer serves a class of functionality to the layer above it and is served by the layer below it. Classes of functionality are implemented in software development using established communication protocols. Each layer in the OSI model has well-defined functions, and the methods of each layer communicate and interact with those of the layers immediately above and below as appropriate. Although the OSI model is largely theoretical and not all networks strictly adhere to its structure, it provides a useful way to understand and describe how different network protocols interact and co-operate to provide network services.

***Example:***

In this example, we simplify the model by considering only five layers. This approach makes it easier to understand how the model works. We've combined the Presentation, Session, and Transport layers into a single layer, referred to as the Transport layer.

<p align="center">
<a href="https://www.codequoi.com/en/internet-layered-network-architecture/"><img width="650" src="https://www.codequoi.com/images/internet-architecture/internet-layered-architecture-en.drawio.png">
<p>

The **application layer**, the highest layer in the network protocol stack, hosts network applications and their associated protocols. These applications and protocols, which are the very reason for the existence of computer networks, are diverse and continually evolving. The table below showcases only a subset of the most prevalent applications and protocols:

| Application                                   | Protocol(s)       |
| --------------------------------------------- | ----------------- |
| Request and transfer Web pages                | HTTP, HTTPS       |
| File transfer                                 | FTP               |
| Email transfer and access                     | SMTP, IMAP        |
| Shell remote access with secure connection    | SSH               |
| Instant message transfer                      | IRC, XMPP         |
| Clock synchronization to local time           | NTP               |
| Internet domain name translation into IP      | DNS               |
| Streaming audio/video                         | RMTP, HLS, SRT    |
| Peer-to-peer file sharing                     | BitTorrent, eDonkey|

An application-layer protocol facilitates information exchange between applications on different hosts. Packets of the application layer are known as “messages”.

The **transport layer** of the Internet plays a crucial role in facilitating communication between applications on different hosts. It conveys application-layer messages between application endpoints. The two primary protocols at this layer are TCP and UDP.

TCP is a connection-oriented, reliable protocol. It establishes a connection before data transmission and ensures data is received correctly, resending if necessary. It controls data flow, adjusts transmission speed during network congestion, and breaks down long data streams into smaller segments. TCP is typically used by file transfer, message transfer, web page transfer, and streaming services like YouTube and Netflix.

On the other hand, UDP is a simpler, connection-less protocol. It doesn't regulate traffic or transmission rate and doesn't guarantee message delivery. However, its simplicity is beneficial for quick transmission of small data amounts, such as server-to-client data or situations where data loss is acceptable over retransmission. DNS, voice over IP, and online gaming typically use UDP.

In the transport layer, data packets are referred to as "segments".

The **network layer** of the Internet is tasked with routing "datagrams" (packets at this layer) from one host to another. The Internet Protocol (IP) is the primary protocol at this layer. It's essential for any host wishing to connect to the Internet, defining the datagram structure and unique IP addresses for each host. Two main versions exist: IPv4 and IPv6, performing similar functions with slight differences.

Other smaller routing protocols, such as RIP, OSPF, IS-IS, and BGP, work alongside IP, primarily determining the datagram's path to its destination. The ICMP protocol communicates information or error messages, like when a service or host is unreachable.

Despite the presence of other protocols, the network layer is often simply referred to as IP, highlighting its central role in holding the Internet together.

The **link layer**'s primary function is to transport a datagram from one network node to the next. It works closely with the network layer, receiving datagrams from it, moving them to the next node, and then passing them back to the network layer.

Link layer protocols are largely dependent on the physical medium between two nodes. These protocols include Ethernet, WiFi, DOCSIS, and PPP. Some ensure reliable packet delivery, while others do not.

A datagram often traverses multiple physical media, requiring different link-layer protocols. For instance, a datagram might be handled by Ethernet on the first link, PPP on the next three, and WiFi on the final link.

At the link layer, data packets are referred to as "frames".

The **physical layer**, the base layer of the network, is responsible for transmitting individual bits of the link-layer frames from one node to another. The protocols at this layer are intrinsically tied to the physical medium used for transmission and the link-layer protocols above it. For instance, Ethernet employs various physical-layer protocols, each tailored for a specific medium - twisted-pair copper wire, coaxial cable, optic fiber, and so on. Each protocol has a unique method for transmitting a bit across the link.

</p>

#### TCP/IP (Transmission Control Protocol/Internet Protocol) - A Practical Approach

<p align="justify">

The **TCP/IP (Transmission Control Protocol/Internet Protocol) Model**, also known as **Internet Protocol suite**, is a more practical counterpart to the OSI model. It is the foundation upon which the internet and most commercial networks operate. The TCP/IP model consists of four layers: the Network Interface, Internet, Transport, and Application layers. The Network Interface layer corresponds to the combination of the Physical and Data Link layers in the OSI model. The Internet layer is equivalent to the Network layer in the OSI model, handling IP addressing and routing. The Transport layer is responsible for reliable data transmission, similar to its OSI counterpart. Finally, the Application layer of the TCP/IP model combines the functions of the Session, Presentation, and Application layers in the OSI model. It handles high-level protocols like HTTP and FTP, enabling user applications to interact with the network. It is named after the two most important protocols in the suite: the Transmission Control Protocol (TCP) and the Internet Protocol (IP). TCP/IP provides end-to-end connectivity specifying how data should be packetized, addressed, transmitted, routed, and received at the destination.

<p align="center">
<a href="https://github.com/f-corvaro/NETPRACTICE"><img width="650" src="https://media.geeksforgeeks.org/wp-content/uploads/20230417045622/OSI-vs-TCP-vs-Hybrid-2.webp">
<p>

</p>

### Data Sharing

<p align="justify">

In a computer network, data is shared using a process called **packet switching**. The data to be sent is broken down into small units, called packets, in a fixed format. Packets, also known as **Datagrams**, consist of a header and a payload section. The header, placed at the beginning of the block of data, contains information about the source and destination addresses, packet number, and error-checking data. The payload is the actual intended message. Headers contain metadata essential for payload delivery, while the payload is extracted and used by an operating system, application software, or higher-layer protocols.

<p align="center">
<a href="https://github.com/f-corvaro/NETPRACTICE"><img width="650" src="https://upload.wikimedia.org/wikipedia/commons/f/f6/Packet_Switching.gif">
<a href="https://github.com/f-corvaro/NETPRACTICE"><img width="650" src="https://upload.wikimedia.org/wikipedia/commons/3/39/Network_packet.jpg">
<p>

The packets are then sent over the network from the source node to the destination node. Along the way, they may pass through several intermediate nodes, such as routers and switches, which read the packet headers to determine the best path to the destination. This process is known as routing. Once all the packets reach the destination, they are reassembled in the correct order to form the original data. If any packets are lost or damaged during transmission, the error-checking data in the packet headers can be used to detect this and request retransmission of the affected packets. This ensures reliable data transmission over the network. The physical link technologies of packet networks typically limit the size of packets to a certain maximum transmission unit (MTU).

With packets, the bandwidth (the maximum rate of data transfer across a given path) of the transmission medium can be better shared among users than if the network were circuit-switched. When one user is not sending packets, the link can be filled with packets from other users, allowing the cost to be shared with relatively little interference, provided the link is not overused. Often, the route a packet needs to take through a network is not immediately available. In such cases, the packet is queued and waits until a link is free.

</p>

#### Network nodes

<p align="justify">

Each node in a network has a unique network address, which can be used to send data to that node. Nodes can be connected to each other in various ways, forming different network topologies. The way nodes are connected and interact with each other determines many properties of the network, such as its speed, reliability, and resilience to faults.

**Modem:** A modem (short for modulator-demodulator) is a device that converts data between digital formats used by computers and analog formats used by older telephone lines or radio signals. In a home network, the modem connects to the internet service provider's network, allowing devices in the home to access the internet.

**Router:** A router is a device that forwards data packets between computer networks, creating an overlay internetwork. Routers perform the traffic directing functions on the internet; data sent through the internet, such as a web page or email, is in the form of data packets. A packet is typically forwarded from one router to another through the networks that constitute the internet work until it reaches its destination node.

**Bridges:** A network bridge is a computer networking device that creates a single aggregate network from multiple communication networks or network segments. This function is called network bridging. Bridging is distinct from routing, which allows multiple different networks to communicate independently while remaining separate.

**Switches:** A network switch is a multiport network bridge that uses MAC addresses to forward data at the data link layer (layer 2) of the OSI model. Some switches can also forward data at the network layer (layer 3) by additionally incorporating routing functionality. Such switches are commonly known as layer-3 switches or multilayer switches.

**Firewall:** A firewall is a network security device that monitors incoming and outgoing network traffic and decides whether to allow or block specific traffic based on a defined set of security rules. Firewalls have been a first line of defense in network security for over 25 years. They establish a barrier between secured and controlled internal networks that can be trusted and untrusted outside networks, such as the internet.

**Network Interfaces:** A network interface is the point of interconnection between a computer and a private or public network. A network interface is generally a network interface card (NIC) but does not have to have a physical form. Instead, the network interface can exist in software or can be a combination of hardware and software.

**Repeaters:** A repeater is an electronic device that receives a signal and retransmits it at a higher level or higher power, or onto the other side of an obstruction, so that the signal can cover longer distances. In a wired network, a repeater can receive a signal on an electromagnetic or optical transmission medium, amplify it and retransmit it. Repeaters overcome the attenuation caused by free-space electromagnetic-field divergence or cable loss.

**Hubs:** A network hub is a node that broadcasts data to every computer or Ethernet-based device connected to it. A hub is less sophisticated than a switch, the latter of which can isolate data transmissions to specific devices. The hub does not manage any of the traffic that comes through it; any packet of data entering any port is rebroadcast out on every other port. In a hub, a frame is passed along or "broadcast" to every one of its ports. It does not matter that the frame is only destined for one port. The hub has no way of distinguishing which port a frame should be sent to.

</p>


## Evaluation Process

### Peer-Evaluations

<p align="justify">

Submit your assignment in your Git repository as usual. Only the work inside your repository will be evaluated during the defense. Double-check the names of your files to ensure they are correct.

Since there are 10 levels in the training interface, you need to submit 10 files in your repository (one file per level). Place them at the root of your repository. Make sure to enter your login in the training interface and export a file per level using the **Get my config** button. It is crucial that you enter your login in the interface.

During the defense, you will be required to successfully complete 3 random levels as specified on the training platform. You will have a limited time to do so. The use of external tools is not allowed during your evaluation. However, the use of a simple calculator such as `bc` is tolerated but will be the limit. 

`bc` is a command-line calculator that supports arbitrary precision arithmetic. It is commonly used in Unix-like operating systems, including Linux. `bc` stands for "basic calculator" and can handle complex mathematical expressions, including floating-point calculations, making it a useful tool for quick computations directly from the terminal.

```bash
# Start bc in interactive mode
bc

# Perform a calculation
scale=2
5 / 3

# Output: 1.66
```

</p>


### Correction sheet

<p align="center">
<a href="https://github.com/f-corvaro/NETPRACTICE"><img width="650" src="https://github.com/f-corvaro/NETPRACTICE/blob/main/.extra/.cs/cs1.png">
</p>
<p align="center">
<a href="https://github.com/f-corvaro/NETPRACTICE"><img width="650" src="https://github.com/f-corvaro/NETPRACTICE/blob/main/.extra/.cs/cs2.png">
</p>
<p align="center">
<a href="https://github.com/f-corvaro/NETPRACTICE"><img width="650" src="https://github.com/f-corvaro/NETPRACTICE/blob/main/.extra/.cs/cs3.png">
</p>
<br>

## Developed Skills

<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=git,linux" />
  </a>
</p><br>

## References


- [CodeQuoi: Internet Layered Network Architecture](https://www.codequoi.com/en/internet-layered-network-architecture/) - A comprehensive guide to the architecture of Internet networks, explaining the different layers and their functions.
- [CodeQuoi: IPv4 Addresses, Routing, and Subnet Masks](https://www.codequoi.com/en/ipv4-addresses-routing-and-subnet-masks/) - Detailed explanation of IPv4 addressing, routing, and subnet masks, key concepts in network communication.
- [Wikipedia: Computer Network](https://en.wikipedia.org/wiki/Computer_network) - An overview of computer networks, including their history, types, and key principles.
- [Wikipedia: Datagram](https://en.wikipedia.org/wiki/Datagram) - Detailed explanation of datagrams, basic units of data transfer in packet-switched networks.
- [Wikipedia: Packet Switching](https://en.wikipedia.org/wiki/Packet_switching) - Detailed article on packet switching, the method used to send data across networks.
- [Wikipedia: OSI Model](https://en.wikipedia.org/wiki/OSI_model) - Comprehensive article on the OSI Model, a conceptual framework used to understand network interactions.
- [BMC Blog: Understanding the OSI Model](https://www.bmc.com/blogs/osi-model-7-layers/) - A blog post that breaks down the seven layers of the OSI Model and their functions.
- [Wikipedia: Internet Protocol Suite](https://en.wikipedia.org/wiki/Internet_protocol_suite) - Detailed article on the Internet Protocol Suite, also known as TCP/IP, the set of protocols used for the Internet.
- [Wikipedia: IP Address](https://en.wikipedia.org/wiki/IP_address) - Comprehensive article on IP addresses, unique identifiers for devices on a network.

- [Netpractice on Medium](https://medium.com/@imyzf/netpractice-2d2b39b6cf0a) - A Medium article discussing the concept of network practices.
- [New Subnetting on Medium](https://toufa7.medium.com/new-subnetting-34fadfb86c70) - A Medium article explaining the concept of subnetting in networking.
- [42bangkok-netpractice on GitHub](https://github.com/viruskizz/42bangkok-netpractice) - A GitHub repository.
- [NetPractice on GitHub](https://github.com/lpaube/NetPractice) - Another GitHub repository.
- [42-net-practice on GitHub](https://github.com/ricardoreves/42-net-practice) - Another GitHub repository.
- [Net_Practice on GitHub](https://github.com/tblaase/Net_Practice) - Another GitHub repository.
- [42-net-practice on GitHub](https://github.com/ricardoreves/42-net-practice) - Another GitHub repository.
  
## Support and Contributions

<p align="center">
If you find this repository helpful, please consider starring it to show your support. Your support is greatly appreciated!</p>

<p align="center">
<a href="https://ko-fi.com/fcorvaro"><img width="180" img align="center" src="https://github.com/f-corvaro/42.common_core/blob/main/.extra/support-me-ko-fi.svg"><alt=""></a>
<a href="https://github.com/sponsors/f-corvaro"><img width="180" img align="center" src="https://github.com/f-corvaro/42.common_core/blob/main/.extra/support-me-github.svg"><alt=""></a>

<br>

## Author

<p align="center"><a href="https://profile.intra.42.fr/users/fcorvaro"><img style="height:auto;" src="https://avatars.githubusercontent.com/u/102758065?v=4" width="100" height="100"alt=""></a>
<p align="center">
<a href="mailto:fcorvaro@student.42roma.it"><kbd>Email</kbd><alt=""></a>
<a href="https://github.com/f-corvaro"><kbd>Github</kbd><alt=""></a>
<a href="https://www.linkedin.com/in/f-corvaro/"><kbd>Linkedin</kbd><alt=""></a>
<a href="https://42born2code.slack.com/team/U050L8XAFLK"><kbd>Slack</kbd><alt=""></a>

<hr/>