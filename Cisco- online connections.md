# Types of Wireless networks

## mobile phones

-the mobile phone uses radio waves to transmit signals to towers in geographical areas

-When a telephone call is made, the voice signal is relayed from one tower to another tower until it is delivered to its destinatio

## cellphone interactions with different networks

-talk : landlines, cellphones, business
-data: data plan
-wifi: hotspots, home wireless
-location services: gps, maps,places
-pay services: cash registers, payment pads

## types of network components

-hosts: computer, server, laptop
-peripherals:webcam, scanner, printer, mouse
-network devices: hubs,switches, routers
-network media: cabling, or wireless. pathway for all of the messages to get from source to destination

## configure IP Addressing Information on Windows

- settings - network and internet- change address options - network connections panel - right click on ethernet ( or the wireless connection) and choose properties

    -in Ethernet properties scroll down and  double click Internet Protocol Ver 4 (TCP/IPv4) - properties - click use the following IP address

    -type: 192.168.1.100 IPV4  255.255.255.0 subnet mask 192.168.1.1 default gateway. Click OK. and close the box.

## End Device Addressing

-The NIC is a piece of hardware that enables the device to connect to the network medium, either wired or wireless. It may be integrated into the device motherboard or may be a separately installed card.

    IP address - This identifies the host on the network.
    Subnet mask - This is used to identify the network on which the host is connected.
    Default gateway - This identifies the networking device that the host uses to access the internet or another remote network.

## Manual IP Confuguration

With manual configuration, the required values are entered into the device via the keyboard, typically by a network administrator. The IP address that is entered is referred to as a static address and and must be unique on the network.

## Dynamic IP Configuration

Most end-user devices can be set up to receive network configuration information dynamically. This enables the device to request an address from a pool of addresses assigned by a Dynamic Host Configuration Protocol (DHCP) server located within the network.

## Network Basics

Let's look at a typical home network, you have a few different components.

    ISP - Your internet service provider, the company you pay to get Internet at your house.
    Router - The router allows each machine on your network to connect to the Internet. In most modern routers, you can connect via wireless or an Ethernet cable.
    WAN - Wide Area Network, this is what we call the network that encompasses everything between your router and a wider network such the Internet.
    WLAN - Wireless Local Area Network, this is the network between your router and any wireless devices you may have such as laptops.
    LAN - Local Area Network, this is the network between your router and any wired devices such as Desktop PCs.
    Hosts - Each machine on a network is known as a host.

The data and information that gets transmitted through networks are known as packets and by the end of the Networking Nomad section, you'll understand in detail how a packet travels to and from hosts. 

## TCP/IP Model

The OSI model gave birth to what eventually became the TCP/IP model and this model is actually what the Internet is based off of. It is the actual implementation of networking. The TCP/IP model uses the TCP/IP protocol suite, which we just commonly refer to as TCP/IP. These protocols work together to specify how data should be gathered, addressed, transmitted and routed through a network. Using the TCP/IP model, we can see how these protocols are used to show the breakdown of how a packet travels through the network.

-Application Layer

The top layer of the TCP/IP model. It determines how your computer's programs (such as your web browser) interface with the transport layer services to view the data that gets sent or received.

This layer uses:

    HTTP (Hypertext Transfer Protocol) - used for the webpages on the Internet.
    SMTP (Simple Mail Transfer Protocol) - electronic mail (email) transmission

-Transport Layer

How data will be transmitted, includes checking the correct ports, the integrity of the data, and basically delivering our packets.

This layer uses:

    TCP (Transmission Control Protocol) - reliable data delivery
    UDP (User Datagram Protocol) - unreliable data delivery

Network Layer

This layers specifies how to move packets between hosts and across networks.

This layer uses:

    IP (Internet Protocol) - Helps route packets from one machine to another.
    ICMP (Internet Control Message Protocol) - Helps tell us what is going on, such as error messages and debugging information.

-Link Layer

This layer specifies how to send data across a physical piece of hardware. Such as data travelling through Ethernet, fiber, etc.

The lists above of protocols each layer uses is not extensive and you'll encounter many other protocols that come into play.

In the following lessons, we will dive through each of these layers and discuss how our packet traverses through the network in the eyes of the TCP/IP model (there are many perspectives on how a packet travels across networks, we won't look at them all, but be aware that they exist).

## DHCP Overview

DHCP assigns IP addresses, subnet masks and gateways to our machines. For example, let's say you have a cell phone and you want to get a cell phone number to start talking to people. You have to call up your phone carrier and they will give you a number. As long as your pay your bills you can keep using your phone. DHCP is the phone carrier in this case, it gives you an IP address so that you can talk to other IP addresses. You are also leased an IP address, these last for a certain period of time, then will get renewed depending on how you have your lease settings.

DHCP is great for many reasons, it allows a network administrator to not worry about assigning IP addresses and it also prevents them from setting up duplicate IP addresses. Every physical network should have its own DHCP server so that a host can request an IP address. In a regular home setting, the router usually acts as the DHCP server.

The way DHCP gets all your dynamic host information is:

    DHCP DISCOVER - This message is broadcasted to search for a DHCP server.
    DHCP OFFER - The DHCP server in the network replies with an offer message. The offer contains a packet with DHCP lease time, subnet mask, IP address, etc.
    DHCP REQUEST - The client sends out another broadcast to let all DHCP servers know which offer it accepted.
    DHCP ACK - Acknowledgement is sent by the server.

## Network Documentation

