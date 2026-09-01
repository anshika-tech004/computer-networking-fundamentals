## Subnetting Practice
Question 1 — Basic /24 Network
Given the network:
192.168.1.0/24
Find:
1. Subnet mask
2. Network address
3. Broadcast address
4. First usable host
5. Last usable host
6. Total addresses
7. Usable hosts

Solution

CIDR:/24

Subnet mask:255.255.255.0

Host bits:
32 - 24 = 8

Total addresses:2^8 = 256

Usable hosts:

256 - 2 = 254

Answer

|Parameter| Result|
|----|----|
|Network Address| "192.168.1.0"|
|First Host| "192.168.1.1"|
|Last Host| "192.168.1.254"|
|Broadcast Address| "192.168.1.255"|
|Total Addresses| "256"|
|Usable Hosts| "254"|
|Subnet Mask| "255.255.255.0"|

🟢 Question 2 — /25 Subnet
For:192.168.1.0/25
Find:
- Subnet mask
- Network address
- Broadcast address
- First host
- Last host
- Total addresses
- Usable hosts

Solution

CIDR:/25
Subnet mask:255.255.255.128
Host bits:32 - 25 = 7
Total addresses:2^7 = 128
Usable hosts:128 - 2 = 126

Block size:256 - 128 = 128
Therefore, the ranges are:
192.168.1.0   - 192.168.1.127
192.168.1.128 - 192.168.1.255

For the first subnet:

|Parameter| Result|
|----|----|
|Network Address| "192.168.1.0"|
|First Host| "192.168.1.1"|
|Last Host| "192.168.1.126"|
|Broadcast Address| "192.168.1.127"|
|Total Addresses| "128"|
|Usable Hosts| "126"|
|Subnet Mask| "255.255.255.128"|

🟡 Question 3 — Find the Subnet of an IP Address
Given:192.168.10.75/26
Find:
- Subnet mask
- Network address
- Broadcast address
- First host
- Last host
- Total addresses
- Usable hosts

Solution

"/26" gives:

Subnet Mask = 255.255.255.192

Host bits:

32 - 26 = 6

Total addresses:

2^6 = 64

Usable hosts:

64 - 2 = 62

Block size:

256 - 192 = 64

Subnet ranges:

0 - 63
64 - 127
128 - 191
192 - 255

The last octet of the IP is:

75

"75" falls within:

64 - 127

Therefore:

|Parameter| Result|
|----|----|
|Network Address| "192.168.10.64"|
|First Host| "192.168.10.65"|
|Last Host| "192.168.10.126"|
|Broadcast Address| "192.168.10.127"|
|Total Addresses| "64"|
|Usable Hosts| "62"|
|Subnet Mask| "255.255.255.192"|

🟡 Question 4 — Divide /24 into /27 Subnets
Divide:192.168.1.0/24
into "/27" subnets.
Find:
1. Number of subnets
2. Total addresses per subnet
3. Usable hosts per subnet
4. Network address of each subnet
5. Broadcast address of each subnet

Solution

New prefix:

/27

Original prefix:

/24

Borrowed bits:

27 - 24 = 3

Number of subnets:

2^3 = 8

Host bits:

32 - 27 = 5

Total addresses per subnet:

2^5 = 32

Usable hosts:

32 - 2 = 30

Subnet mask:

255.255.255.224

Block size:

256 - 224 = 32

Subnet Table

|Subnet| Network Address| First Host| Last Host| Broadcast|
|----|----|----|----|----|
|1| "192.168.1.0"| ".1"| ".30"| ".31"|
|2| "192.168.1.32"| ".33"| ".62"| ".63"|
|3| "192.168.1.64"| ".65"| ".94"| ".95"|
|4| "192.168.1.96"| ".97"| ".126"| ".127"|
|5| "192.168.1.128"| ".129"| ".158"| ".159"|
|6| "192.168.1.160"| ".161"| ".190"| ".191"|
|7| "192.168.1.192"| ".193"| ".222"| ".223"|
|8| "192.168.1.224"| ".225"| ".254"| ".255"|

Result
8 subnets
32 addresses per subnet
30 usable hosts per subnet

