# Networking

### What is a network

- A collection of computers, servers and devices. Allows to share data between devices.

### What is an IP address

- Internet Protocol address, identifier for a computer within a network. 

1. Public IP: Allows access over the internet.
2. Private IP: Allows access of LAN.

### What is IPv4 

- IP represented in a 32-bit long address space. Each byte is represented as a decimal up to the value of 255. 

### IP Binary

1. Binary is 1s and 0s which is the primary language read by computers. 
2. Each 1 or 0 is known as a bit, bits come in blocks of 8 which is known as a byte.

- IP addresses are formatted as 4 numbers ranging from 0 to 255, seperated with dots '.'
- Each number in decimal is actually a byte. There is a total of 4 bytes. 4x8 = 32-bits

### Firewalls & AWS

1. A firewall acts as a protective layer outside your computer.
2. Monitors incoming and outgoing traffic, the firewall rules allows what can bypass the firewall.

- Example in AWS where we allowed different ports in a security group resembles a firewall example in AWS.

### Max number of IPs

- Max number of IPs is just over 4billion

### Solution: IPv6

- IPv6 is 128-bit opposed to IPv4's 32-bit design. 

### Problem with IPv6

- No backwards compatibility 
- Reduced security with no submasking
- Most smartphones from 2015 onwards are ready for IPv6
- All modern computers have IPv6

### Address classes

1. Class A: First 8 bits, ranges from 1.x.x.x to 126.x.x.x

### Address classes pt.2

1. First decimal: The network
2. The three decimals afterwards will be addresses 

### Subnet masks

- The process of taking a network and splitting it into smaller networks.

- Masks can have different bits used.

### Subnet mask example

- Every computer uses the same subnet mask address

### Submask and IP

- Used to free up IPs 

### CIDR block

- Classless Inter-Domain Routing

### DOS Brute Force Attack

- Trial and error method to guess credentials such as login, password, encryption keys etc.

### Changing IPs into Binary

- Make a table. 128, 64, 32, 16, 8, 4, 2, 1. Calculate Binary IP.

### Submask

- Submask will have an IP. 

1. If 1 then the values must match
2. If 0 then the values can differ

### CDRI Blocks 

- /8 : 255.0.0.0
- /16 : 255.255.0.0
- /24 : 255.255.255.0
- /32 : 255.255.255.255

### VPC - Virtual Private Cloud

- AWS - Allows us to create a networking system inside their cloud which is our Cloud.
- Create machines and add storage
- VPCs exist in regions and can exist in several availability zones
- Region > VPC > Availability zones

1. We give our VPC an IP. e.g. 111.0.0.0/8
2. We are going to create a Public Subnet and give it an IP. e.g. 111.10.0.0/16
3. We are going to create a Private Subnet and give it an IP. e.g. 111.20.0.0/16
4. We will put our DB in the Private Subnet. 
5. We will put our App in the Public Subnet.

- Each instance (machine) will have its own security group.
- NACL - Firewalls at the Subnet level. Applies to all instances inside the subnet.
 

- Routes Table

#### IGW - Internet Gateway

- Brings an IP which we add to our VPC. 




