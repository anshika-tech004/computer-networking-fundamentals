## OSI MODEL (Open System Interconnection)
-  It is a conceptual model
-  Goal- To understand how data travels between 2 devices over a network
  > my understanding
   - According to me it's a step by step framework that explains what happens to data when you send or receive something over network

## THE 7 OSI LAYERS
. Layer1 (Physical Layer)
- Data unit- Bits
- Goal- Transporting bits
- Through- wires, cables, wifi, repeater, hub, radio signals.
- Addressing scheme- None

. Layer2 (Data Link Layer)
- Data unit- Frame
- Goal- 1. To group bits into frame
        2. add MAC address to identify devices and perform error detection
- Devices- NICs, switches
- Protocols- Wi-Fi (802.11), PPP, HDLC, ARP
- Addressing scheme- MAC address (48 bits)- Hop to hop delivery
- Common question- "How do I get to next directly connected device"?


. Layer3 (Network Layer)
- Data unit- Packet
- Goal- 1. Assigns IP address to devices.
        2. Ensures data packet to reach its destination
        3. Routing
- Devices- Router, switch
- Protocols- IP (IPv4/IPv6), ICMP, IPsec, OSPF, RIP, BGP
- Addressing scheme- IP address(32 bits)- End to end delivery
- Common question- " Which device should the packet go to"?


. Layer4 (Transport Layer)
- Data unit- Segment (TCP)  Datagram (UDP)
- Goal- Right program/application receives right data
- Protocols-
-  1. TCP (Transmission Control Protocol)
        - Connection oriented
        - Reliable delivery of packets
        - Ordered data
        - Used for- web page(HTTPS), file transfer(FTP), email(SMTP)

   2. UDP (User Datagram Protocol)
        - Connectionless
        - No reliable delivery of data packets
        - No guaranteed ordering
        - Useful when speeds matter more than perfect reliability and ordering
- Addressing scheme- Port
- Common question- "How is data transported?"

NOTE- IP address- which device?  Port number- which application?
| PORT | SERVICE |
|------|---------|
| 20/21 | FTP |
| 22 | SSH |
| 23 | TELNET |
| 25 | SMTP |
| 53 | DNS |
| 80 | HTTP |
| 443 | HTTPS |


. Layer5 (Session Layer)
- Data unit- Data
- Goal
   1. To manage session between applications
   2. To maintain those sessions
   3. To synchronize session
   4. To terminate session
- Protocols- PPTP, Net Bios, SIP
- Addressing scheme- Session identifier
- Common question- "How do I manage the communication/session"?


. Layer6 (Presentation Layer)
- Data unit- Data
- Goal- Handles how data is represented
     - Data compression/ decompression
     - Encryption/ decryption
     - Data formatting
- Protocols/Technologies- 	SSL/TLS, JPEG, PNG, GIF, MPEG, ASCII, Unicode


. Layer7 (Application Layer)
- Data unit- Data
- Goal- web communication
       - File transfer
       - email service
       - name resolution
- Protocols- HHTP/HTTPS
            - FTP
            - SMTP
            - POP3
            - IMAP
            - DNS
- Common question- " What network service does my application needs"?


            
