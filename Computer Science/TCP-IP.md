# TCP/IP & The Protocol Stack
### The Protocol Stack
- The **transmission control protocol / internet protocol** protocol stack is a set of networking protocols that work together as four connected layers, passing incoming and outgoing data packets up and down the layers during network during communication. The layers are as follows:

> ##### Application Layer
> - Sits at the top of the stack and uses protocols relating to the application being used to transmit data. If the application is a browser, for example, it would select an appropriate higher level protocol for communication such as HTTP, POP3 or FTP

> ##### Transport Layer
> - Uses the **Transmission Control Protocol (TCP)** to establish an **end-to-end** connection with the recipient computer. 
> - The data is then split into packets and labelled with the packet number, the total number of packets and the port number through which the packet should be routed.
> - The transport layer is responsible for re-requesting packets should any be missing or corrupted, as well as acknowledging the receipt of packages.

> ##### Network Layer
> - Sometimes referred to as IP layer or Internet layer.
> - This layer adds the source and destination IP addresses to the packets. 
> - **Routers** operate on the network layer and will use these IP addresses to forward the packets on to the destination. 
> - The addition of the IP address to the port number is called a **socket**.

> ##### Link Layer
> - The link layer is the physical connection between network nodes and adds the unique **Media Access Control (MAC)** addresses identifying the **Network Interface Cards (NICs)** of the source and destination devices.
> - This means that once the packet finds the correct network using the IP address, it can then locate the correct piece of hardware.
> - MAC addresses are changed at each hop, and specify the MAC address of the device that is receiving the packet that particular hop.

### At The Receiving End
- At the receiving end, the MAC address is stripped off by the link layer, which passes the packets on to the network layer.
- The network layer removes the IP addresses and passes them on to the transport layer.
- The transport layer uses the port number to determine which application to pass the data to in the application layer, then removes the port numbers and reassembles the packets in the correct order.
- Packets move up and down the protocol stack at each router as they have their source and destination MAC addresses changed at each hop.

### Media Access Control (MAC) Addresses
- A MAC address is a unique 12-digit hexadecimal code that is hardcoded on every **Network Interface Card** during manufacture.
- This uniquely identifies a particular device so that data packets can be routed directly to them.

### Well-Known Ports & Protocols
| Server Port Number | Protocol                              |
| ------------------ | ------------------------------------- |
| 20                 | File Transfer Protocol (FTP) data     |
| 21                 | FTP control instructions              |
| 22                 | Secure Shell (SSH) remote login       |
| 23                 | Telnet remote login                   |
| 25                 | Simple Mail Transfer Protocol SMTP    |
| 80 & 8080          | HyperText Transfer Protocol HTTP      |
| 110                | Post Office Protocol v3 POP3          |
| 143                | Internet Message Access Protocol IMAP | 
| 443                | HTTPS (HTTP Secure)                   |

### FTP
- Used to send files between computers.
- Can require authorisation to access, or can be used anonymously.
- Uses instructions on port 21 to manage protocol.

### Secure Shell (SSH)
- **Secure Shell (SSH)** is used for remotely accessing and managing a computer. If is a modern and secure replacement for Telnet which used no encryption at all.
- It is commonly used by network administrators to manage servers because it can be done remotely.
- Using SSH with other application layer protocols means that you can operate a **'tunnel'** through port 22, through which other protocol requests can operate. 
- This means that messages can be sent securely using other protocols, and can bypass any network restrictions that have been placed on other ports.

### Email
- POP3 is responsible for retrieving emails from a mail server that temporarily stores your incoming mail. When emails are retrieved, they are transferred to your local computer and removed from the server.
- IMAP keeps emails on the server, maintaining synchronicity.
- SMTP is used to transfer outgoing emails from one server to another or from an email client to the server when sending an email.

### Rendering Web Pages
- When a browser receives an HTTP response from a web server, the documents containing the HTML, CSS and/or JavaScript are parsed to fit a standard hierarchical model.
- The HTML is broken down into a hierarchy of tags called a **Document Object Model (DOM)** tree in order for the browser to structure the code.
- The CSS styles form their own **CSSOM**. 
- Lastly, any JavaScript is parsed and executed.
- The browser then renders or 'paints' the page on the screen.
