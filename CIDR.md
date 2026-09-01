## CIDR:- (Classless Inter Domain Routing)
- It tells you the prefix/length through which you can determine:
          - Network bit
          - Host bit
          - Subnet Mask
- CIDR notation is written as: IP Address/ Prefix length
- Example: 192.168.1.25/24
    - Herein /24= CIDR/Network bit
    - Host bit= 32-24=8
    - Total address= $2^8$ =256
    - Usable host= 256-2= 254
    - Subnet mask= 255.255.255.0 ( binary: 11111111.11111111.11111111.00000000)

  ## Calculating Subnet Mask through CIDR Notation
  - Let's understand through an example:
  - /24 Subnet mask
     - Step 1: /24 = 24 network bits + 8 host bits
     - Step 2: Convert the 24 network bits to a mask
          - Write 24 ones followed by 8 zeros:
        
           11111111.11111111.11111111.00000000
        - Convert each 8-bit section to decimal:
             - 11111111 = 255
             - 11111111 = 255
             - 11111111 = 255
              - 00000000 = 0
     - Therefore:
          /24 = 255.255.255.0

 - /25 Subnet mask
    - Step 1: /25= 25 network bit+ 7 host bit
    - Step 2: mask- 11111111.11111111.11111111.10000000
    - 11111111 = 255
    - 11111111 = 255
    - 11111111 = 255
    - 1000000 =  128
    - Subnet mask = 255.255.255.128
      
                          
  |CIDR| Subnet mask/Dotted decimal Subnet mask| Network bit| Host bit| Total address| Usable Host|
  |----|----|----|----|----|----|
  |/24| 255.255.255.0| 24| 8| 254|
  |/25| 255.255.255.128| 25| 7| 128| 126|
  |/26| 255.255.255.192| 26| 6| 64| 62|
  |/27| 255.255.255.224| 27| 5| 32| 30|
  |/28| 255.255.255.240| 28| 4| 16| 14|
  |/29| 255.255.255.248| 29| 3| 8| 6|
  |/30| 255.255.255.252| 30| 2| 4| 2|
  

  
