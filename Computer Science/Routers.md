# Packet Switching & Routers
### Packet Switching
- **Packet switching** is a method of communicating packets of data across a network on which other similar communications are happening simultaneously. The communications cables are shared between many communications to allow efficient use of them.

### Data Packets
- Data that is to be transmitted across a network is broken down into more manageable chunks called **packets**.
- The size of packets can vary but is usually between 500 and 1500 bytes.
- Each packet contains a header and a payload containing the body of data being sent. Some packets may also use a trailer section with a checksum or Cyclical Redundancy Check (CRC) to detect transmission errors by creating and attaching a hash total calculated from the data contained in the packets.
- The **header** contains the sender's and recipient's IP addresses, the protocol being used and the number of packets being sent. It also includes the Time To Live (TTL) or hop limit, after which point the data expires and is discarded.
- When a packet of data leaves a user's computer, the fastest or least congested route is taken. At the receiving end, the packets can be reassembled into the correct order and any missing packets could be re-requested.

### Routers
- Routers are used to connect at least two networks. The act of traversing between one router and the next across a network is referred to as a hop. 
- The router reads the recipient's IP address in each packet and forwards it on to the recipient via the fastest and least congested route to the next router, which will do the same until the packet reaches its destination.
- Routers use routing tables to store and update the locations of other network devices and the best route to them. A routing algorithm like Dijkstra's Algorithm is commonly used to deduce the most efficient routes.

### Gateways
- Where protocols differ between networks, a **gateway** is used rather than a router to translate between them.
- All header data is stripped from the packet leaving only raw data and new header data is added in the format of the new network before the gateway sends the packet on its way again.
