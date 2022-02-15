# Internet Security
### Firewalls
- A **firewall** is a security checkpoint designed to prevent unauthorised access between two networks. It can be implemented using both hardware and software. A router may contain a firewall
- A typical firewall consists of a separate computer containing two Network  Interface Cards (NICs), with one connected to the internal network, and the other connected to the external network. Using firewall software, each packet that attempts to pass between the two NICs is analysed against preconfigured rules (**packet filters**), then accepted or rejected.
- A firewall may also act as a **proxy server**.

### Packet Filtering
- Also referred to as static filtering, packet filtering controls network access according to network administrator rules.
- Static filtering can filter packets based on the source IP addresses, as well as the protocols being used and the port numbers they are trying to access.
- A **port** determines which application may handle a data packet as it arrives at a computer. (I.E which protocol the packet is using)

### Stateful Inspection
- **Stateful inspection** or **dynamic filtering** can examine the payload contents of a data packet to better assess it for safety.
- It can create temporary contextual rules based on the passage of previous packets in a 'conversation'. This is to ensure incoming responses (to your outgoing packets) can be temporarily allowed during that communication stream.
- 'Conversation' data is usually kept in a Connection Table on routers which is dynamically updated and referred to.

### Proxy Servers
- A **proxy server** intercepts all packets entering and leaving a network, hiding the true network addresses of the source from the recipient. This enables privacy and anonymous surfing. 
- A proxy can also store caches of frequently visited websites and return the web page data to the user immediately without the need to reconnect to the internet and re-request the webpage.
- A proxy server may serve multiple (hundreds or thousands) of users.

### Encryption
- **Encryption** is the process of scrambling data so that is becomes very difficult to unscramble and interpret without the correct key.
- Encrypted data is known as **ciphertext**, and the original data is known as **plaintext**.

### Symmetric (Private Key) Encryption
- **Symmetric encryption** uses the same key to encrypt and decrypt data.
- This means the key must be transferred (**key exchange**) to the same destination as the ciphertext which causes obvious security problems. Once the key is intercepted an attacker has access to all messages.
- For this reason **asymmetric encryption** can be used instead.

### Asymmetric (Public Key) Encryption
- **Asymmetric encryption** uses two separate but related keys. 
- One key, known as the **public key**, is made public so that others wishing to send you data can use this to encrypt the data. This public key cannot decrypt data.
- Another **private key** is known only by you and only this can be used to decrypt the data. It is virtually impossible to deduce a private key from the public key.
- It is possible that a malicious party may encrypt a message using your public key and impersonate another party. To overcome this, a digital signature can be used to verify the sender.

### Digital Signatures
- A **digital signature** is a way of verifying the sender of a message's identity, and that the message has not been tampered with.
- Firstly, a mathematical value is calculated from the unencrypted message data. This is known as a hash total, checksum or digest. 
- Any change to the message will produce a different hash total.
- The sender of the message uses their own private key to encrypt the hash total. The encrypted total becomes the digital signature  since only the holder of the private key could have encrypted it.
- The signature is attached to the message to be sent, then the whole message is encrypted using the recipient's public key before being sent.
- The recipient decrypts the message using their private key, then decrypts the digital signature using the sender's public key. 
- The hash total is reproduced based on the message data and if this matches that in the digital signature, the message is verifiable.
- The time and date are also included in the digital signature to ensure the message cannot be copied and sent again later.

### Digital Certificates
- To ensure that the sender of a message is not impersonating a trustworthy source, a **digital certificate**, issued by official **Certificate Authorities (CAs)** is used. (E.g Symantec)
- The certificate contains the certificate's serial number, the expiry date, the name of the holder, a copy of their public key, and the digital signature of the CA so that the recipient can authenticate the certificate as real.

### Worms, Trojans and Viruses
- These are all types of malware.
- A **worm** is a self replicating piece of malware that does not need a host file to spread itself (it is a subclass of viruses). A worm usually enters a computer via a vulnerability or by tricking the user into running a program.
- A **virus** is a self replicating piece of malware that needs a host file to transfer it between computers.
- A **trojan** is a piece of malware that is hidden inside a benevolent and unsuspecting piece of software. A common purpose of a trojan is to install a backdoor in your operating system which the Trojan's creator can exploit (for example to run a botnet).

### Ways To Increase Protection Against Malware
- Regularly updating Operating System and Antivirus software.
- E-mail spam filtering.
- Educating individuals on phishing and other similar scams.
- Using secure passwords.
- Managing user access rights.
- Writing secure code.