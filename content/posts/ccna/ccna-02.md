---
title: CCNA 02 - UTP vs Fiber
subtitle: "UTP vs FIBER"
description: "CCNA 02"
date: 2023-05-22T17:22:44+02:00
tags: ["CCNA", "networking", "cisco" ,"notes", "network fundamentals"]
keywords: [""]
categories: ["CCNA"]
type: posts
featuredImagePreview: https://imgs.xkcd.com/comics/rewiring.png
comment: false
toc: true
---
In the right corner we have the reigning champion, the UTP cable. In the left corner we have the challenger, the Fiber cable. Let's get ready to rumble!
<!--more-->

## Champion: UTP Copper Cable

{{< admonition type=warning title="Our reigning champion is know by many names:" open=true >}}

- For the peasants &rarr; Ethernet cable *(don't be a peasant)*.
- For the nerds &rarr; UTP as in Unshielded Twisted Pair *(don't be a nerd)*.
- For the heretics &rarr; RJ45 *(don't be a heretic)*.
{{< /admonition >}}

### Clarifications

- **UTP** is the twisty cable that allows to send and receive data between devices.
- **RJ45** is the connector that allows to connect the UTP cable to a device.
- **Ethernet** is a collection of protocols that allows to send and receive data between devices.

{{< center-quote >}}
I cant be bothered put an image of an UTP cable and RJ45 connector here, you know what it looks like. If you don't, Google it.
{{< /center-quote >}}

### Things you should know about UTP cables

1. They are cheap.
2. They have 8 pins &rarr; 4 pairs of 2 pins.
3. They can only be used for short distances &rarr; 100 meters or less. Mostly used for LANs.
4. They are not secure &rarr; can be easily tapped into, since they are not shielded.
5. They are not reliable &rarr; They are prone to electromagnetic interference.
6. Electrical signals are used to send and receive data.

### UTP cable types

1. **Straight-through** &rarr; used to connect different devices.
2. **Crossover** &rarr; used to connect similar devices.

{{< center-quote >}}
I hope you remember that UTP cables have 8 pins. If you don't, go back and read from the start.
{{< /center-quote >}}  

| Device Type                 | Transmit Pins | Receive |
| --------------------------- | ------------- | ------- |
| ROUTER, Firewall, PC/Server | 1 and 2       | 3 and 6 |
| Switch                      | 3 and 6       | 1 and 2 |

{{< center-quote >}}
Now that you have learned about the different types of UTP cables, you can go ahead and forget about them. Because nowadays, all devices have Auto-MDIX. This means that they can automatically detect the type of cable and adjust accordingly.
{{< /center-quote >}}

### Ethernet Standards for UTP cables

| Speed    | Common Name      | Street Name | Cable Name | Pins Used |
| -------- | ---------------- | ----------- | ---------- | --------- |
| 10 Mbps  | Ethernet         | 10 BASE-T   | Cat 3      | 4         |
| 100 Mbps | FaseEthernet     | 100 BASE-T  | Cat 5      | 4         |
| 1 Gbps   | Gigabit Ethernet | 1000 BASE-T | Cat 5e     | 8         |
| 10 Gbps  | 10 Gig Ethernet  | 10G BASE-T  | Cat 6a     | 8         |

## Challenger: Fiber

New kid on the block is the Fiber cable. It's a bit more expensive, but it's faster, more secure and more reliable.

It basically consists of a glass core surrounded by a cladding. The cladding is surrounded by a buffer and the buffer is surrounded by a jacket. The jacket is the outer layer of the cable. BORINGG!!!

{{< center-quote >}}
Basically its a glass tube with a plastic tube around it and you use lasers to *phew phew* data through it.
{{< /center-quote >}}

### Things you should know about Fiber cables

1. Normally not used in LANs, but in WANs.
2. They are expensive.
3. Light signals are used to send and receive data.

### Connectors: Small Form-factor Pluggable (SFP)

{{< admonition type=tip title="As Micheal Scott would say:" open=true >}}
{{< figure src="https://media0.giphy.com/media/IjJ8FVe4HVk66yvlV2/giphy.gif" height=20%, width=60% >}}
{{< /admonition >}}

{{< admonition type=info title="Behold the SFP connector" open=true >}}
{{< image src="images/ccna/sfp.png" height=20%, width=60% >}}
{{< /admonition >}}

{{< admonition type=info title="The far less interesting cable" open=true >}}
{{< image src="images/ccna/fiberCable.jpg" height=20%, width=60% >}}
{{< /admonition >}}

### Types of Fiber Cables

| Multi-Mode                                 | Single-Mode                         |
| ------------------------------------------ | ----------------------------------- |
| Wider (allowing more angles of light wave) | Narrower                            |
| Cheaper                                    | Expensive                           |
| Shorter Cable length                       | Longer  Cable length                |
| LED base transmitter                       | Laser based transmitter (phew phew) |

### Ethernet Standards for Fiber cables

For the sake of conceive:

- Single-Mode &rarr; SM
- Multi-Mode &rarr; MM

| Speed   | Street Name  | Cable Type | Cable Length      |
| ------- | ------------ | ---------- | ----------------- |
| 1 Gbps  | 1000 BASE-LX | MM/ SM     | 550m (MM) 5km(SM) |
| 10 Gbps | 10G BASE-SR  | MM         | 400m              |
| 10 Gbps | 10G BASE-LR  | SM         | 10km              |
| 10 Gbps | 10G BASE-ER  | SM         | 30km              |

## TLDR

| UTP Cable  | Fiber Cable |
| ---------- | ----------- |
| Cheap      | Expensive   |
| Short      | Long        |
| Slow       | Fast        |
| Unsecure   | Secure      |
| RJ45       | SFP         |
| Copper     | Glass       |
| Electrical | Light       |
| LAN        | WAN         |

## OUR NEW Champion is

{{< admonition type=success title="Champion is..." open=false >}}
There is no winner here. Both have their pros and cons. It all depends on the situation.

## DIDN't EXPECT THAT DID YOU?

{{< figure src="https://media.giphy.com/media/Xg5qpmzzzp10rt01l0/giphy.gif" height=20%, width=60% >}}
{{< /admonition >}}

## Resources

1. [Jeremy's IT LAB Day 2](https://www.youtube.com/watch?v=ieTH5lVhNaY)
