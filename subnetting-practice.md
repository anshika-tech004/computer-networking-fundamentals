## Subnetting Practice
This file contains subnetting problems ranging from basic CIDR calculations to practical network-design scenarios.
For each question, I have calculated:
- CIDR notation
- Subnet mask
- Network address
- Broadcast address
- First usable host
- Last usable host
- Total addresses
- Usable hosts
- Block size
- Number of subnets (where applicable)

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

Question 2 — /25 Subnet
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

Question 3 — Find the Subnet of an IP Address
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

The last octet of the IP is:75

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

Question 4 — Divide /24 into /27 Subnets
Divide:192.168.1.0/24
into "/27" subnets.
Find:
1. Number of subnets
2. Total addresses per subnet
3. Usable hosts per subnet
4. Network address of each subnet
5. Broadcast address of each subnet

Solution

New prefix:/27

Original prefix:/24

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

Question — /28 Subnetting
For:192.168.5.0/28
Find:
1. Subnet mask
2. Block size
3. Number of subnets from /24
4. Total addresses per subnet
5. Usable hosts per subnet
6. All network addresses

Solution

Subnet mask:
255.255.255.240

Borrowed bits:
28 - 24 = 4

Number of subnets:
2^4 = 16

Host bits:
32 - 28 = 4

Total addresses:
2^4 = 16

Usable hosts:
16 - 2 = 14

Block size:
256 - 240 = 16

Network Addresses:
 - 192.168.5.0/28
 - 192.168.5.16/28
 - 192.168.5.32/28
 - 192.168.5.48/28
 - 192.168.5.64/28
 - 192.168.5.80/28
 - 192.168.5.96/28
 - 192.168.5.112/28
 - 192.168.5.128/28
 - 192.168.5.144/28
 - 192.168.5.160/28
 - 192.168.5.176/28
 - 192.168.5.192/28
 - 192.168.5.208/28
 - 192.168.5.224/28
 - 192.168.5.240/28

Question  — Find Network and Broadcast Address
Given:10.20.30.200/29
Find:
- Network address
- Broadcast address
- First host
- Last host
- Total addresses
- Usable hosts

Solution

Subnet mask:
255.255.255.248

Host bits:
32 - 29 = 3

Total addresses:
2^3 = 8

Usable hosts:
8 - 2 = 6

Block size:
256 - 248 = 8

Relevant ranges:
192 - 199
200 - 207
208 - 215

"200" falls within:
200 - 207
Therefore:

|Parameter| Result|
|----|----|
|Network Address| "10.20.30.200"|
|First Host| "10.20.30.201"|
|Last Host| "10.20.30.206"|
|Broadcast Address| "10.20.30.207"|
|Total Addresses| "8"|
|Usable Hosts| "6"|


Question — Find CIDR from Host Requirement

A network needs to support 50 usable hosts.
Find the smallest subnet that can support this requirement.

Solution

Formula:

Usable Hosts = 2^Host Bits - 2

Try 5 host bits:

2^5 - 2 = 30

30 is not enough.

Try 6 host bits:

2^6 - 2 = 62

62 is enough.

Therefore:

Host Bits = 6

CIDR:

32 - 6 = /26

Answer

CIDR = /26
Subnet Mask = 255.255.255.192
Usable Hosts = 62


Question — Find CIDR from Subnet Requirement
You have:192.168.100.0/24
You need at least 4 equal-sized subnets.
Find the new CIDR prefix and list all subnet network addresses.

Solution

We need 4 subnets.

2^2 = 4

Therefore, borrow 2 bits from the host portion.

Original prefix:

/24

New prefix:

24 + 2 = /26

Subnet mask:

255.255.255.192

Block size:

256 - 192 = 64

Subnets
  - 192.168.100.0/26
  - 192.168.100.64/26
  - 192.168.100.128/26
  -192.168.100.192/26

Each subnet provides:

64 total addresses
62 usable hosts

## Practical Subnetting scenario

Question- A small company has the network:
192.168.10.0/24
It wants to divide this network into 4 equal-sized subnets.
Find:
1. New CIDR
2. Subnet mask
3. Network address of each subnet
4. Broadcast address of each subnet
5. Usable host range
6. Number of usable hosts per subnet

Solution

Original network:
192.168.10.0/24

We need:
4 subnets

Formula:
"Number of subnets = 2^n"

We need:
"2² = 4"

Therefore, we borrow 2 bits from the host portion.

Original prefix:
"/24"

New prefix:
"24 + 2 = /26"

New Subnet Mask
255.255.255.192

Block Size
"256 − 192 = 64"

Therefore, the four subnets are:

Subnet 1

- Network: 192.168.10.0
- First Host: 192.168.10.1
- Last Host: 192.168.10.62
- Broadcast: 192.168.10.63

Subnet 2

- Network: 192.168.10.64
- First Host: 192.168.10.65
- Last Host: 192.168.10.126
- Broadcast: 192.168.10.127

Subnet 3

- Network: 192.168.10.128
- First Host: 192.168.10.129
- Last Host: 192.168.10.190
- Broadcast: 192.168.10.191

Subnet 4

- Network: 192.168.10.192
- First Host: 192.168.10.193
- Last Host: 192.168.10.254
- Broadcast: 192.168.10.255

Final Table

|Subnet| Network| First Host| Last Host| Broadcast|
|----|----|----|----|----|
|1| 192.168.10.0/26| .1| .62| .63|
|2| 192.168.10.64/26| .65| .126| .127|
|3| 192.168.10.128/26| .129| .190| .191|
|4| 192.168.10.192/26| .193| .254| .255|

Each subnet provides:

- 64 total addresses
- 62 usable hosts

---

🧠 Key Subnetting Formulas

Host Bits

"Host Bits = 32 − CIDR Prefix"

Total Addresses

"Total Addresses = 2^(Host Bits)"

Usable Hosts

"Usable Hosts = 2^(Host Bits) − 2"

Block Size

"Block Size = 256 − Subnet Mask Value"

Number of Subnets

"Number of Subnets = 2^(Borrowed Bits)"

# Quick CIDR Reference

|CIDR| Subnet Mask| Total Addresses| Usable Hosts| Block Size|
|----|----|----|----|----|
|/24| 255.255.255.0| 256| 254| 256|
|/25| 255.255.255.128| 128| 126| 128|
|/26| 255.255.255.192| 64| 62| 64|
|/27| 255.255.255.224| 32| 30| 32|
|/28| 255.255.255.240| 16| 14| 16|
|/29| 255.255.255.248| 8| 6| 8|
|/30| 255.255.255.252| 4| 2| 4|

##  What I Learned

Through these exercises, I practiced:

- Understanding CIDR notation
- Converting CIDR to subnet masks
- Calculating network and broadcast addresses
- Finding first and last usable hosts
- Calculating total and usable addresses
- Calculating block size
- Identifying the subnet to which an IP belongs
- Calculating required CIDR based on host requirements
- Dividing a network into equal-sized subnets
- Applying subnetting concepts to practical network scenarios

🔐 Cybersecurity Relevance

Subnetting is important in cybersecurity because it helps with:

- Network segmentation
- VLAN and subnet design
- Limiting broadcast domains
- Access control and firewall rules
- Isolating sensitive systems
- Understanding network traffic
- Identifying whether an IP belongs to a particular network

«Goal: Build enough subnetting knowledge to confidently analyze IP addresses and understand how networks are divided and secured.»


