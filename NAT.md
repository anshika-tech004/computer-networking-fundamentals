## NAT (Network Address Translation )
- Its a technique that translates private IP address to public IP address and vice versa
- Role- Allows private hosts to communicate with external networks since private IP address are not routable
    - Conserve public IPv4 addresses
    - Controls how internal and external addressing is translated
    - Allows many device to share 1 public IP

## Working
- STEP1: A device inside the local network sends a packet to internet
- STEP2: Router replaces the devices Private IP address with its own public IP address
- STEP3: Router keeps a translation table that maps the private IP and port to the public IP and port
- STEP4: When response comes back router uses the table to forward the packet to correct internal device

