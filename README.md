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
  - [Computer Networks](#computer-networks)
    - [Network Packets](#network-packets)
    - [Network Topology and Its Impact](#network-topology-and-its-impact)
    - [Overlay Networks](#overlay-networks)
    - [OSI Model](#osi-model)
    - [Physical Layer and Network Transmission Media](#physical-layer-and-network-transmission-media)
    - [Network nodes](#network-nodes)
    - [Communication protocols](#communication-protocols)
  - [Internet Protocol (IP) Address](#internet-protocol-ip-address)
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

First, we need to understand how to connect multiple computers.

### Computer Networks

<p align="justify">

A computer network is a collection of interconnected devices that share resources and communicate with each other using common communication protocols. These devices, or nodes, can include personal computers, servers, and other specialized or general-purpose hosts. The interconnections between nodes are established through various telecommunication technologies, including wired (e.g., Ethernet or coaxial cables), optical (e.g., fiber optics), and wireless (e.g., radio waves) methods, which can be organized into different network topologies.

Each node in a computer network is identified by a unique network address and may also have a hostname, which serves as a memorable label. Hostnames are typically assigned during the initial setup and rarely change, while network addresses are used by communication protocols, such as the Internet Protocol (IP), to locate and identify nodes.

Computer networks enable a wide range of applications and services, including access to the World Wide Web, digital video and audio streaming, shared use of application and storage servers, printers, and fax machines, as well as email and instant messaging.

</p>

#### Network Packets

<p align="justify">

Most modern computer networks use protocols based on packet-mode transmission. A network packet is a formatted unit of data carried by a packet-switched network. Packet switching is a method of grouping data into short messages in a fixed format. Packets consist of a header and a payload. The header, placed at the beginning of the block of data, contains information about the source and destination addresses, packet number, and error-checking data. The payload is the actual intended message. Headers contain metadata essential for payload delivery, while the payload is extracted and used by an operating system, application software, or higher-layer protocols.

<p align="center">
<a href="https://github.com/f-corvaro/NETPRACTICE"><img width="650" src="https://upload.wikimedia.org/wikipedia/commons/f/f6/Packet_Switching.gif">
<p>

<p align="center">
<a href="https://github.com/f-corvaro/NETPRACTICE"><img width="650" src="https://upload.wikimedia.org/wikipedia/commons/3/39/Network_packet.jpg">
<p>

With packets, the bandwidth (the maximum rate of data transfer across a given path) of the transmission medium can be better shared among users than if the network were circuit-switched. When one user is not sending packets, the link can be filled with packets from other users, allowing the cost to be shared with relatively little interference, provided the link is not overused. Often, the route a packet needs to take through a network is not immediately available. In such cases, the packet is queued and waits until a link is free.

The physical link technologies of packet networks typically limit the size of packets to a certain maximum transmission unit (MTU). A longer message may be fragmented before it is transferred, and once the packets arrive, they are reassembled to reconstruct the original message.

</p>

#### Network Topology and Its Impact

<p align="justify">

The physical or geographic locations of network nodes and links generally have relatively little effect on a network, but the topology of interconnections can significantly impact its throughput and reliability. Network topology refers to the arrangement of different elements (links, nodes, etc.) in a computer network. With many technologies, such as bus or star networks, a single failure can cause the entire network to fail. In general, the more interconnections there are, the more robust the network is; however, this also increases the cost and complexity of installation.

<p align="center">
<a href="https://github.com/f-corvaro/NETPRACTICE"><img width="650" src="https://upload.wikimedia.org/wikipedia/commons/9/97/NetworkTopologies.svg">
<p>

The physical layout of the nodes in a network may not necessarily reflect the logical network topology. For example, with Fiber Distributed Data Interface (FDDI), the logical network topology is a ring, but the physical topology is often a star because all neighboring connections can be routed via a central physical location. While the physical layout is not completely irrelevant, common ducting and equipment locations can represent single points of failure due to issues like fires, power failures, and flooding.

</p>

#### Overlay Networks

<p align="justify">

An overlay network is a virtual network that is constructed on top of an existing network. Nodes in the overlay network are interconnected by virtual or logical links, each of which corresponds to a path that may traverse multiple physical links in the underlying network. The topology of the overlay network often differs significantly from that of the underlying network. For instance, many peer-to-peer networks are overlay networks, organized as nodes within a virtual system of links that operate on top of the Internet.

Overlay networks have been utilized since the early days of networking, when computers were connected via telephone lines using modems, even before the advent of dedicated data networks.

A prominent example of an overlay network is the Internet itself. Initially, the Internet was built as an overlay on the telephone network. Even today, each Internet node can communicate with virtually any other node through an underlying mesh of sub-networks with diverse topologies and technologies. Address resolution and routing facilitate the mapping of a fully connected IP overlay network to its underlying network. While the overlay network does not control how packets are routed in the underlying network between two overlay nodes, it can manage the sequence of overlay nodes that a message traverses before reaching its destination.

</p>

#### OSI Model

<p align="justify">

The Open Systems Interconnection (OSI) model is a reference model from the International Organization for Standardization (ISO) that "provides a common basis for the coordination of standards development for the purpose of systems interconnection." In the OSI reference model, communications between systems are split into seven different abstraction layers: Physical, Data Link, Network, Transport, Session, Presentation, and Application.

<p align="center">
<a href="https://github.com/f-corvaro/NETPRACTICE"><img width="650" src="https://media.fs.com/images/community/upload/kindEditor/202107/29/original-seven-layers-of-osi-model-1627523878-JYjV8oybcC.png">
<p>

The model partitions the flow of data in a communication system into seven abstraction layers to describe networked communication from the physical implementation of transmitting bits across a communications medium to the highest-level representation of data in a distributed application. Each intermediate layer serves a class of functionality to the layer above it and is served by the layer below it. Classes of functionality are implemented in software development using established communication protocols. Each layer in the OSI model has well-defined functions, and the methods of each layer communicate and interact with those of the layers immediately above and below as appropriate.

</p>

#### Physical Layer and Network Transmission Media

<p align="justify">

The Physical Layer is the first and lowest layer in the OSI model. It is responsible for the actual transmission and reception of unstructured raw data between a device and a physical transmission medium. This layer defines the hardware elements involved in the network, including electrical cables, optical fibers, and wireless transmission media such as radio waves and infrared signals.

The Physical Layer specifies the physical characteristics of the transmission medium, including the layout of pins, voltages, cable specifications, and radio frequencies. It also defines the data rate (the number of bits sent per second), the modulation scheme, and the signal strength. The primary function of this layer is to convert digital data into electrical, optical, or radio signals and transmit them over the physical medium.

A widely adopted family of technologies that use copper and fiber media in local area networks (LANs) is collectively known as Ethernet. The media and protocol standards that enable communication between networked devices over Ethernet are defined by IEEE 802.3. Wireless LAN standards use radio waves, while others use infrared signals as a transmission medium. Power line communication uses a building's power cabling to transmit data.

</p>

#### Network nodes

<p align="justify">

Apart from any physical transmission media, networks are built from additional basic system building blocks, such as network interface controllers, repeaters, hubs, bridges, switches, routers, modems, and firewalls. Any particular piece of equipment will frequently contain multiple building blocks and so may perform multiple functions.

**Network Interfaces:** A network interface controller (NIC) is computer hardware that connects the computer to the network media and has the ability to process low-level network information. In Ethernet networks, each NIC has a unique Media Access Control (MAC) address—usually stored in the controller's permanent memory. To avoid address conflicts between network devices, the Institute of Electrical and Electronics Engineers (IEEE) maintains and administers MAC address uniqueness. The size of an Ethernet MAC address is six octets. The three most significant octets are reserved to identify NIC manufacturers. These manufacturers, using only their assigned prefixes, uniquely assign the three least-significant octets of every Ethernet interface they produce.

**Repeaters and Hubs:** A repeater is an electronic device that receives a network signal, cleans it of unnecessary noise and regenerates it. The signal is retransmitted at a higher power level, or to the other side of obstruction so that the signal can cover longer distances without degradation. In most twisted-pair Ethernet configurations, repeaters are required for cable that runs longer than 100 meters. With fiber optics, repeaters can be tens or even hundreds of kilometers apart. Repeaters work on the physical layer of the OSI model but still require a small amount of time to regenerate the signal. This can cause a propagation delay that affects network performance and may affect proper function. As a result, many network architectures limit the number of repeaters used in a network. An Ethernet repeater with multiple ports is known as an Ethernet hub. In addition to reconditioning and distributing network signals, a repeater hub assists with collision detection and fault isolation for the network. Hubs and repeaters in LANs have been largely obsoleted by modern network switches.

**Bridges and Switches:** Network bridges and network switches are distinct from a hub in that they only forward frames to the ports involved in the communication whereas a hub forwards to all ports. Bridges only have two ports but a switch can be thought of as a multi-port bridge. Switches normally have numerous ports, facilitating a star topology for devices, and for cascading additional switches. Bridges and switches operate at the data link layer (layer 2) of the OSI model and bridge traffic between two or more network segments to form a single local network. Both are devices that forward frames of data between ports based on the destination MAC address in each frame. They learn the association of physical ports to MAC addresses by examining the source addresses of received frames and only forward the frame when necessary. If an unknown destination MAC is targeted, the device broadcasts the request to all ports except the source, and discovers the location from the reply. Bridges and switches divide the network's collision domain but maintain a single broadcast domain. Network segmentation through bridging and switching helps break down a large, congested network into an aggregation of smaller, more efficient networks.

**Routers:** A router is an internetworking device that forwards packets between networks by processing the addressing or routing information included in the packet. The routing information is often processed in conjunction with the routing table. A router uses its routing table to determine where to forward packets and does not require broadcasting packets which is inefficient for very big networks.

**Modems:** Modems (modulator-demodulator) are used to connect network nodes via wire not originally designed for digital network traffic, or for wireless. To do this one or more carrier signals are modulated by the digital signal to produce an analog signal that can be tailored to give the required properties for transmission. Early modems modulated audio signals sent over a standard voice telephone line. 

**Firewalls:** A firewall is a network device or software for controlling network security and access rules. Firewalls are inserted in connections between secure internal networks and potentially insecure external networks such as the Internet. Firewalls are typically configured to reject access requests from unrecognized sources while allowing actions from recognized ones. The vital role firewalls play in network security grows in parallel with the constant increase in cyber attacks.

</p>

#### Communication protocols

<p align="justify">

A communication protocol is a set of rules for exchanging information over a network. They may be connection-oriented or connectionless, they may use circuit mode or packet switching, and they may use hierarchical addressing or flat addressing. In a protocol stack, often constructed per the OSI model, communications functions are divided up into protocol layers, where each layer leverages the services of the layer below it until the lowest layer controls the hardware that sends information across the media. The use of protocol layering is ubiquitous across the field of computer networking. An important example of a protocol stack is HTTP (the World Wide Web protocol) running over TCP over IP (the Internet protocols) over IEEE 802.11 (the Wi-Fi protocol). This stack is used between the wireless router and the home user's personal computer when the user is surfing the web.

</p>

### Internet Protocol (IP) Address

<p align="justify">

An Internet Protocol address (IP address) is a numerical label (e.g. 192.0.2.1) that is assigned to a device connected to a computer network that uses the Internet Protocol for communication. IP addresses serve two main functions: network interface identification, and location addressing.

The Internet Protocol (IP) is the network layer communications protocol in the Internet protocol suite for relaying datagrams across network boundaries. 


</p>

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

- [Computer Network - Wikipedia](https://en.wikipedia.org/wiki/Computer_network)
- [Packet Switching - Wikipedia](https://en.wikipedia.org/wiki/Packet_switching)
- [Osi Model - Wikipedia](https://en.wikipedia.org/wiki/OSI_model)
- [Osi Model - bmc blog](https://www.bmc.com/blogs/osi-model-7-layers/)
- [Internet Protocol (IP) Address - Wikipedia](https://en.wikipedia.org/wiki/IP_address)
- [](https://en.wikipedia.org/wiki/Internet_Protocol)
- [](https://en.wikipedia.org/wiki/Network_layer)

- [](https://en.wikipedia.org/wiki/Datagram)


- [1](https://medium.com/@imyzf/netpractice-2d2b39b6cf0a)
- [2](https://toufa7.medium.com/new-subnetting-34fadfb86c70)
- [3](https://github.com/viruskizz/42bangkok-netpractice)
- [4](https://github.com/lpaube/NetPractice)
- [5](https://www.codequoi.com/en/internet-layered-network-architecture/)
- [6](https://github.com/ricardoreves/42-net-practice)
- [7]()
  
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