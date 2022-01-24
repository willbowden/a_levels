# IP Addresses
- An Internet protocol or IP address is a unique numerical address used to identify a host computer or network node trying to communicate over IP on the Internet.
- IPv4 addresses provide 4 billion possible addresses.
- IPv6 uses hexadecimal addresses rather than binary, providing 340 trillion, trillion, trillion unique addresses.

### IPv4
- An IPv4 address consists of a 32-bit number written in a dotted-part represents an 8 bit binary pattern giving a range of 0-255 for each decimal number.

### Reserved IP Addresses
- 127.x.x.x are private, non-routable addresses used for diagnostics within local networks only.
- x.x.x.0 is the network identifier.
- x.x.x.255 is reserved for the broadcast address on that subnet where data is sent simultaneously to all subnetwork hosts.
- x.x.x.1 is conventionally the default router address.

### Network & Host Identifiers
- An IPv4 address contains two parts to identify both the individual network and the host computer within that network. The network part of the address uses the first bits in the 32-bitherefore the size of the network ID determines the number of bits remaining in the address for the host ID.

### Classful Addressing
- Historically, systems of classes were used to define the size or proportion of the network and host identifiers within an IP address. Class A networks had very few network identifiers (7 bits), for example.

### Classless Addressing 
- The more modern classless system specifies the number of bits in the subnet mask. For example:
> 103.27.104.92/24
> --

- , where '/24' indicates that the first 24 bits of the IP address are the network ID and the remaining 8 are the host ID. This allows the split between network ID and host ID to be anywhere in the 32 bits.

### Subnet Masking
- A **subnet mask** is used in conjunction with an IP address to identify the two unique parts of the address.
- A subnet mask of 255.255.255.0 indicates that 24 bits have been used for the network ID, corresponding to a suffix of '/24' in a classless address.
- A subnet mask is 'ANDed' with the IP address using the bitwise logical AND operator to separate out the network ID from the full IP address.

### Subnetting
- A network administrator of a large organisation using an IP address with a 16-bit network ID may wish to create **subnetwork** segments within their own larger IP network in order to ease management and improve efficiency by routing data through one segment only. Using a bus network, this would allow computers in different subnetworks to communicate with computers in their same subnetwork simultaneously. 
- A **subnet ID** is created by using the most significant bits from the **host ID** section of the IP addresses.
- The term subnet ID is commonly used to cover the network and subnet ID together.

### Public and Private IP Addresses
- A **public** (or routable) IP address must be globally unique and can be addressed directly by any other computer in the world. 
- Within a local network, addresses can be **private** (non-routable) and the web server or router can forward the data going through it to the correct internal device. 
- For that reason, private addresses do not need to be globally unique.
- To allow external access to a privately addressed computer, a **Network Access Translator (NAT)** is required.

### Dynamic Host Configuration Protocol
- A **DHCP** server is used to automatically assign a dynamic IP address from a pool of available addresses to a computer attempting to operate on a public network such as an Internet hotspot. Since IP addresses are in short supply, this system of dynamic addressing enables active computers to request and IP address for the duration they are online and release the IP address back to the pool for another computer when it is not in use.
- DHCP also provides the subnet mask and other automatic configuration details alongside the IP address. 
- **Static IP addressing** is uncommon as it permanently allocates a networked computer a scarce IPv4 address.

### Network Address Translation (NAT)
- **Network Address Translation (NAT)** is used to convert IP addresses as they pass between a public address space and a LAN with a private address space.
- NAT is required to translate private IP addresses since they are not routable.
- When a non-routable computer makes an outgoing request, the router logs its IP address and port number in a translation table and swaps the packet IP address and port number for its own.
- An incoming response, identified by the port number, is then rebadged with the original IP address and port number, then forwarded to the local machine.
- Using NAT allows more devices to exist than IPv4 will allow, while the transition to IPv6 is made.
- It also allows for greater security by automatically creating a firewall between internal and external net

### Port Forwarding
- **Port forwarding** is commonly a product of **NAT** when a public computer is trying to communicate with a server on a private network. An external router can be programmed to filter out packets destined for certain computer or applications, based on their port numbers.