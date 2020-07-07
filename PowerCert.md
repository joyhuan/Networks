# PowerCert
## DHCP 
Dynamic Host Configuration Protocol 

Every computer on a network has to have an IP address 

2 ways that a computer can be assigned an IP address:
- static IP: a user assigns an IP address manually (IP addresses must be unique)
- dynamic IP: a computer gets an IP address from a DHCP server 
  - a DHCP server automatically assigns a computer an: 
    - IP addresss 
    - Subnet mask
    - Default gateway 
    - DNS server 
  - The DHCP server assigns the IP address as a lease 
    - A lease is the amount of time an IP address is assigned to a computer 
    - The lease is to help make sure the DHCP server does not run out of IP addresses  
    - A reservation ensures that a specific computer or device will always be given the same IP address 
    - Reservations are typically given to special devices to computers, such as network printers, servers, routers, etc. 
    - DHCP is a service that runs on a server, such as a Microsoft server or a Linux server
    - It's also a service that runs on routers 

## DNS 
Domain Name System 

Resolves names to numbers/ 

Resolves domain names to IP addresses 

Your computer => 
look for cache if no 

Resolver Server(ISP Internet Service Provider) => 
look for cache if no 

Root server (top/root of the DNS hierarchy)
- 13 sets of theses root servers strategically placed around the world 
- Operated by 12 different organizations 
- Each set has their own unique IP address 

TLP Server (Top Level Domain) => 
- Stores the address info for top level domains 
  - Such as .COM .NET .ORG etc. 
  
Authoritative Name Server (Final Authority)
- Responsible for knowing everything about the domain 
  - Including the IP address 
  
## Hub, Switch & Router
- Hub 
  - Only detects that a device is physically connected to it
  - Not intelleigent - Data is copied to all other ports
  - Has unnecessary traffic - waster bandwidth 
  
- Switch 
  - Can detect specific devices that are connected to it 
  - Keeps a record of the Mac addresses of those devices 
  - Intelligent - Data directed only to intended port 
  - Much more preferred over Hub

Hubs and Switches are used to exchange data within a local area network. 

Not used to exchange data outside their own network. 

To exchange data outside their own network, a device needs to be able to read IP addresses 

- Router 
  - Routes data from one network to another based on their IP address 
  - Essentially the gateway of a network 

Hubs & Switches are used to create networks. 

Routers are used to connect networks. 

## Modem vs Router 
A modem is what brings the internet into your home/business

- A computer only reads digital signals 
- The internet only reads analog signals 

- Modem demodulates incoming analog signals into a digital signal 
- Modem modulates outgoing digital signals into an analog signal 
- Name: modulator demodulator 

- Router 
  - Business router vs Small office/home office router 
  - A router is waht routes or passes your internet connection to all of you devices 
  - Cable Modem (cable televation eg. comcast)
  - DSL Modem (phone line eg. AT&T)
  
- A modem/router device would have a modem with a built-in wireless router, in one device   
  
## RAM 
Random Access Memory

- Stored on the motherboard in modules that are called DIMMs (Dual Inline Memory Module)
  - Can have 168, 184, 240, or 288 pins 
  
- RAM is installed on the motherboard in the memory slots 
  - The average motherboard will have between 2 and 4 memory slots 
  
- In order for a program to run, it needs to be loaded into RAM first 

- Increasing the RAM will make the computer run faster 
 
- Requires constant electrical power to store data 

- DRAM Dynamic RAM 
  - Contains capacitors 
  - Capacitors have to be refreshed with electribity constantly 
  
- SDRAM Synchronous Dynamic RAM 
  - Used today in RAM DIMMS 
  - Difference with DRAM is speed 
    - DRAM - Operates Asynchronously with the system clock 
    - SDRAM - Synchronously
    - All signals are tied to the system clock for a better controlled timing 
    
- The term 64 or 32 bit data path refers to the number of bits of data that are transferred in 1 clock cycle 

- A single bit/ 1 bit of data is the smallest form of data that the computer reads 
    - 8 bits = 1 byte 
    - 64 bit data path <=> 8 byte wide bus 
    - PC-100: 100 MHz = The speed at which it operates 
      - 100 MHz * 8 bytes = 800 MB/s total bandwidth 
      
- RIMM - Rambus Inline Memory Module 
  - Has 184 pins 
  - Looks similar to DIMMS
  - Bottom notches are near the center of the module 
  - Debuted in 1999
  - Was a breakthrough in the speed of memory 
  
  - Debuted in 1999 
  - RDRAM speed was at 800 MHz (SDRAM speed was 133 MHz)
  - Only had a byte wide bus (SDRAM has an 8 byte wide bus)
  
- DDR - Double Data Rate 
  - Sends double the amount of data in each clock signal 
  - DDR may include both the clock speed and the total bandwidth in its name 
    - DDR-333MHz PC-2700(actual total bandwidth)
    
- DDR2 
  - DDR2 is faster than DDR because it allows for higher bus speeds (less power than DDR)
  - Has 240 pins compared to DDR (184 pins)
  
- DDR3 
  - Twice as fast as DDR2 (less power than DDR2)
  - Also has 240 pins 
  - Bottom notches are in different places 
  - Not interchangable with DDR, DDR2, or DDR4 
  
- DDR 4 
  - Has 288 pins 
  - Use less power 
  - Offers a higher range of speed than DDR3 
  
Sometimes there are circumstances where memory data corruption cannot be tolerated 
ECC - Error Correcting Code 
  - Detects if the data was correctly processed by the memory module 
  - Makes a correction if it needs to 
  - Non ECC 8 Memory; Chips ECC 9 Memory
  - Mostly used in servers 
  
## Hotspot 
Wifi Router or 

Wireless Access Point 

Internet Service Provider 

A hotspot is a location

## RAID 
Storage is another very important part of fault tolerace

Data loss prevention(In case of disk failuure)

RAID(Redundant Array of Independent Disks)
- RAID 0
  - Not fault tolerant 
  - Incoming data is 'striped' across multiple disks 
  - Only reason wants to use is speed 
- RAID 1
  - Fault tolerant 
  - Each disk has the same data 
- RAID 5
  - Requires 3 or more disks 
  - Most common setup used (fast and can store lots of data)
  - Data is 'sriped' across multiple disks along with parity 
  - The equivalent of an entire disk is used to store parity 
- RAID 10 
  - Combines RAID 1 with RAID 0
  - needs minimum of 4 disks 
  - Benefits from the fault tolerance of RAID 1 and the speed of RAID 0
  - Can only use 50% for data storage 

## Telnet 
A terminal emulation progarm that is used to access remote serverse 
