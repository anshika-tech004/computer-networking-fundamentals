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

    - Private IP → NAT Router → Public IP → Internet


## PAT (Port Address Translation)
- It is extension of NAT that uses port number to allow multiple private devices to share single IP address

## NAT VS PAT
|Features| NAT| PAT|
|----|----|----|
|Full form| Network Address Translation| Port Address Translation|
|Role| Translates IP address| Translates IP address and port number|
|Mapping| One to one or many to many| Many to one|
|Public IP requirement| can require multiple public IPs| usually uses 1 public IP|
|Port number| generally unchanged| modifies|


