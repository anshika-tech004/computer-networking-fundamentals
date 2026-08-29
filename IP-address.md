## Internet Protocol (IP)
  - It's a numerical address assigned to any device that is connected to network
  - Also called Logical Address
  - OSI layer- Network Layer
  - Assigned by- ISP, DHCP
  - Goal
      - 1.Identification of a device on network
      - 2.Identifies where data should be delivered.
  - Example- 192.168.1.10

## IP Address VS MAC Address
|Basis| IP Address| MAC Address|
|----|----|----|
|Full form| Internet Protocol Address| Media Access Control Address|
|OSI Layer| Network Layer| Data Link Layer|
|Type| Logical Address| Physical Address|
|Format(IPv4)| 192.168.1.5| 00:1A:2B:3C:4D:5E|
|Length| IPv4= 32 bits IPv6= 128 bits| 48 bits|
|Usage| Routing packets between networks| Delivering frames within a LAN|

## Versions of IP Address
|IPv4|IPv6|
|----|----|
|Length-32 bits| Length-128bits|
|Octet-4| Octet-8|
|Range 0-255| Range 0-ffff(65535)|
|Numeric address separated by dots(.)| Alphanumeric separated by colon(:)|
|classes-5| classes- None|
|Ex- 192.168.1.10| Ex- 2001:db8::1|

## Types of IP Address
  1.- Public IP address
        - Assigned by-ISP (Internet Service Provider)
        - Its an address that identifies a network/device on Internet.
        - USES:
             - Connecting to website and internet services.
             - Online gaming- used for connection between gaming system and servers
             - Helps in remote access of computers and CCTVs
             - Helps to run internet services like email, VPN, web app
        - EX- Home router connected to internet (ISP assigns it a public IP address)
  2.- Private IP address
        - Assigned by- Router/DHCP server
        - Identifies devices inside a local network like home, school, office 
        - Range- 10.0.0.0 – 10.255.255.255
                - 172.16.0.0 – 172.31.255.255
                - 192.168.0.0 – 192.168.255.255
        -USES:
            - Identifies devices within a LAN
            - Allows devices on same network to communicate
            - Connects computer to local printers
            
- NOTE:- Public and Private IP address can be static or dynamic
  
|Basis| Static IP Address| Dynamic IP Address|
|----|----|----|
|Meaning| Remains fixed| Can change|
|Assignment| Manually configured| Automatically assigned|
|Given By| Network administrator| DHCP Server|
|cost| Expensive for Public IPs| Cheaper|
|Common use| Servers, CCTVs, printers| Phones, laptop, home users|
|Examples| 192.168.1.10(permanently assigned to servers)| 192.168.1.25(assigned temporarily to laptop)|

## Public IP Address VS Private IP Address
|Basis| Public IP Address| Private IP Address|
|----|----|----|
|Meaning| Identifies device on Internet| Identifies device within a LAN|
|Used on| Internet/WAN| LAN(Home, school)|
|Assigned by| ISP| Router/ DHCP Server|
|Internet Access| Access granted| Not accessed directly from Internet|
|EX- 8.8.8.8| EX- 192.168.1.3|

  
        
