# Net_Practice
This project is a general practical exercise to let you discover networking.
_Project's Score:_ [![mnaimi's 42 NetPractice Score](https://badge42.vercel.app/api/v2/cl1txsvi6008009jppddlp1hr/project/2645050)](https://github.com/JaeSeoKim/badge42)

## Communication inside a Network
When a Client sends a request to a Server, it stamps its IP Address _(Source)_ along with the Server's IP Address _(Destination)_ inside the request _Packet_ (more on that later), and so as the Server when it sends the requested Data back.

The reason for that is because that specific request may be passed between different Hosts, and for these hosts to know whether the request was made for them or not, they need to know the _"who sent what to who"_ informations, which are embedded in the previously mentioned _Packet_.

### IP Addresses
An IP Address is basically just a number that represents a Host (as previously mentionned), we can represent it in a _Human readable_ way like this:

```text
192.168.0.1
```

or in a _Computer savy_ way like this: 

```text
11000000.10101000.00000000.00000001
```

We can Conclude from this that IP Addresses are just **32bit** combinations of _ones_ and _zeros_

### Repeater
If two hosts are located very far from each others physically, then the chance of a _Signal Decay_ to happen automatically increases _(btw Signal Decay means that the signal gets weaker and weaker as it travels through greater distances, until it gets lost eventually)_.

This problem can be solved by installing a **Repeater** between two hosts to ensure that the signal gets Regenerated along the way in order to avoid the previously mentioned _Signal Decay_ problem, i.e. when a Host sends a signal to another Host, the Repeater grabs that signal, and sends a Duplicate of that signal _(an identical signal)_ to the receiving host that way the signal stays alive throughout its journey to reach its destination.

### Hub
Another problem that we may face as a Network Technicien _(I know that you're not one, but hypothetically speaking)_, is that you'll need to connect different Hosts so they can communicate with each other, one way to do it is to physically connect every Hosts with  every other Host, so if we have a Network containing 5 Hosts, the total amount of connections would be 10, and that may be problematic in networks with dozens of Hosts.

To avoid this problem, really smart people invented what is called a **Hub**

# Glossary

| Word             | Definition |
| ---------------- | ---------- |
| **Hosts**        | Any device that sends and/or receives data from other devices |
| **Clients**      | Hosts that initiate requests, i.e. devices that request data from other devices |
| **Servers**      | Hosts that respond to Clients by sending the appropriate data, i.e. devices that provide other devices with the data that this latter requested |
| **IP Addresses** | The identity of Hosts inside a specific Network, i.e. a bunch of numbers that represent a single Host inside a Network, it helps with the communication between multiple hosts inside a network by identifying _who sent what to who_ |
| | |

