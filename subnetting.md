## Subnetting
- Refers to dividing large network into small networks called subnets
- Each subnet has its own network address, host address, broadcast address

## Subnetting Examples:
  # TYPE1- Find the details of an existing subnet
    - Given IP address- 192.168.10.75/26, find network address, broadcast address, first host, last host etc.  
    - Step 1- Identify CIDR
         - CIDR= /26
         - We know IPv4 contain 32 bits so,
         - Host bit = 32-26= 6
    - Step 2- Find Subnet Mask
         - Subnet mask= 255.255.255.192
    - Step 3- Calculate Total Address
         - 2^6= 64
    - Step 4- Calculate Usable host
         - 64-2 = 62   (2 addresses cannot be assigned that's why they are not included which are network address and broadcast address)
    - Step 5- Calculate Block size
         - 256-192 = 64
        - (note- Since we are subnetting the 4th octet so the ranges that we need to keep in mind are:
            - 0-63
            - 64-127
            - 128-191
            - 192-255
    - Step 6- Find subnet containing the IP
        - IP: 192.168.10.75 (since 75 falls in range of 64-127 so the subnet containing 192.168.10.64/26 is 192.168.10.64/26)
    - Step 7- Network Address
        - 192.168.10.64
    - Step 8- Broadcast Address 
        - 192.168.10.127 (NA + Block size -1)
    - Step 9- first Usable host
        - 192.168.10.65 ( Network Address(NA) +1)
    - Step 10- Last Usable Host
        - 192.168.10.126 ( Broadcast Address-1)
  # Type2- Create/divide subnets
    - Divide the network 192.168.1.0/24 into 4 equal sized subnets
    - Step1- Identify original network bits and host bits
         - Network Bits= 24 (original CIDR)
         - Host Bits= 32-24= 8
    - Step2- Determine Number of bits to borrow
        - We need 4 subnets ( 2^2)
        - Thus No. of borrow bits= 2 (/24→/26)
    - Step3-Calculate new CIDR
        - New CIDR= 24+2= /26 (Original /24 network is divided into 4 /26subnets)
    - step4- New Subnet Mask
        - /26= 255.255.255.192
    - Step5- New host bit
        - Host Bits= 32-26= 6
    - step6- New Total Address
        - Total Address= 2^6= 64
    - Step7- Usable Host
        - Usable Host= 64-2= 62
    - Step 8- Block Size
        - Block Size= 256-192= 64
        - Since our block size is 64 so we start at 0 and keep adding 64 for the subnets that is to be calculated(0,64,128,192)
     - Step9- Subnet ranges to be calculated
        - Subnet1: 192.168.1.0-192.168.1.63
        - Subnet2: 192.168.1.64-192.168.1.127
        - Subnet3: 192.168.1.128-192.168.1.191
        - Subnet4: 192.168.1.192-192.168.1.255
    - Step10- Find the 4 subnets
        - Subnet 1:- Network address= 192.168.1.0
                   - First Host= 192.168.1.1
                   - Broadcast address= 192.168.1.63
                   - Last host= 192.168.1.62
       - Subnet 2:- Network Address= 192.168.1.64
                  - First Host= 192.168.1.65
                  - Broadcast Address= 192.168.1.127
                  - Last Host= 192.168.1.126
      - Subnet 3:- Network Address= 192.168.1.128
                 - First Host= 192.168.1.129
                 - Broadcast Address= 192.168.1.191
                 - Last Host= 192.168.1.190
      - Subnet 4:- Network Address= 192.168.1.192
                 - First Host= 192.168.1.193
                 - Broadcast Address= 192.168.1.255
                 - Last Host= 192.168.1.254


## Subnetting Usage
  - Efficiently utilize IP addresses
  - Reduces broadcast traffic
  - Improves network performance
  - Simplify network management & troubleshooting

    
  
  
  
        
        
     
