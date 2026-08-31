Length- 32bits (4octets X 8bits)

## Classes
|class| Range| Default Subnet mask| Purpose|
|----|----|----|----|
|A| 1-126| 255.0.0.0| very large network|
|B|128-191| 255.255.0.0| medium size network| 
|C|192-223| 255.255.255.0| small network|
|D|224-239| -| Multicasting|
|E|240-255|-|reserved for experimental/research purposes|

## Examples
  - Class A- 10.1.2.3
  - Class B- 172.16.1.5
  - Class C- 192.168.1.10
  - Class D- 224.0.0.1

## Binary Representation
 - Example 1
    - 192.168.1.10
       - 192= 128+64 ( 2on bit)
            |128|64|32|16|8|4|2|1|
            |----|----|----|----|----|----|----|----|
            |1|1|0|0|0|0|0|0|

        - 168= 128+32+8 (3 on bit)
            |128|64|32|16|8|4|2|1|
            |----|----|----|----|----|----|----|----|
            |1|0|1|0|1|0|0|0|

        - 1= ( 1on bit)
           |128|64|32|16|8|4|2|1|
           |----|----|----|----|----|----|----|----|
           |0|0|0|0|0|0|0|1|

       - 10= 8+2 ( 2 on bit )
           |128|64|32|16|8|4|2|1|
           |----|----|----|----|----|----|----|----|
           |0|0|0|0|1|0|1|0|
   - Thus 192.168.1.10= 11000000.10101000.00000001.00001010

## Network ID VS Host ID
|Basis| Network ID| Host ID|
|----|----|----|
|Meaning| Identifies Network| Identifies device in that network|
|Assigned to| Network| Individual device|
|Determined by| Subnet Mask| Remaining bits after network portion|
|Example| 192.168.1.0| 192.168.1.10 (10= host ID)|

## Loopback Address (local host)
127.0.0.1- Its a IP address used by computer to communicate with itself.

## Private IP Range
  - 10.0.0.0-10.255.255.255
  - 172.16.0.0-172.16.255.255
  - 192.168.0.0-192.168.255.255



      
          
