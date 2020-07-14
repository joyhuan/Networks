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
Teletype Network 

Developed in 1969 (developed before internet)

All commands are in clear text 

No encryption 

A terminal emulation progarm that is used to access remote servers 

Also used to test ports 

Command line tool 

No graphical user interface 

All commands are sent by keyboard 

It's fast 
Telnet may have to be used when working with older equipement 

- SSH secure shell 
SSH protects the data from being attacked or stolen 
  - Encrypts the data 
  - Provides passwork and public key authentication 

## Firewall
Firewall is a system that is designed to prevent unauthorized access from entering a private network. 

Creates a safety barrier between a private network and the public internet

Especially importatnt to large organizations 

A network firewall and a structure firewall work in a similar way 

Rules: Access Control List 

Firewall rules can be based on: 
- IP addresses 
- Domain names 
- Protocols 
- Programs 
- Ports 
- Key words 

Types
- Host-based firewall 
  - Software firewall that is installed on a computer 
  - Protects that computer only 
  - Zone Alarm is a popular 3rd party host-based firewall. 
  - A lot of antivirus programs come with a host-based firewall. 
- Network-based firewall
  - Combination of hardware & software 
  - Protects an entire network 
  
- Stand-alone firewall/ Routers have a built-in firewall/ Cloud firewall 

## Ethernet Cables, UTP vs STP, Straight vs Crossover, CAT 5,5e,6,7,8 Network Cables
Twisted Pair Cable 
- Unshielded Twisted Pair 
  - UTP consists of 4 pairs of color-coded wires twisted around each other 
  - The wires are twisted to prevent electromagnetic interference (crosstalk)
  - Most commonly used 
- Shielded Twisted Pair 
  - STP has a foil shield that covers the wires 
  - The foil shield adds a layer of protection against electromagnetic interference leaking into and out of the cable. 
  - Used in industry, not so common in home/business
  
- The most common types of twisted pair cables that are used in a LAN are: 
  - Straight (patch) cable
  - Crossover cable 
  - 568A 568B
  - A straight(patch) cable is when both ends of a cable are wired using the same standard 
    - The most common type of ethernet cable that's used on a LAN

## What is a Proxy Server? 
Retrieves data on the internet on behalf of a user 

Proxy benefits:
- Privacy - allows you to surf the internet anonymously (Without using a proxy, your public IP address is visible)
- Speed  
- Saves bandwidth
- Activity logging 
- A proxy server cannot encrypt data 
  - VPN(Virtual Private Network)
  
## SSL, TLS, HTTP, HTTPS Explained
- HTTP (Hypertext transfer protocol)
  - The protocol that is used for viewing web pages 
  - In standard HTTP, all info is sent in clear text
  - Vulnerable to hackers 
  
- HTTPS (Secure hypertext transfer protocol)
  - Encrypts the data that is being retrieved by HTTP 
  - Uses encryption algorithms to scramble the data that's being transferred 
  
- SSL (Secure Sockets Layer)
  - Protocol that's used to ensure security on the internet
  - Uses public key encryption to secure data 
  - An SSL certificate is used to authenticate the identity of a website 
  
- TLS (Transport Layer Security)
  - The latest industry standard cryptographic protocol 
  - The successor to SSL 
  - Authenticates the server, client, and encrypts the data 
  
## HDMI, DisplayPort, DVI, VGA, Thunderbolt - Video Port Comparison 
- VGA 
  - Video Graphics Array 
  - Older technology - developed in 1987 
  - Has 15 pins - divided into 3 rows 
  - Only carries analog data 
  - End adapter will typically have a blue color 
  - Was used on CRT monitors 
  - Can still be found on new equipment 
  
- DVI 
  - Digital Visual Interface 
  - Succeeded the VGA port
  - Developed in 1999 
  - Designed to provide uncomproseed, high-quality video to LCD monitors 
  - DVI - A Used to send analog signals only 
  - DIV - D Used to send digital signals only 
  - DVI - I Used to send both analog and digital signals 
  - Dual link DVI has a max resolution of 2560 * 1600 
  - Single link DVI has a max resolution of 1920 * 1200 
  
- HDMI 
  - High Definition Multimedia Interface 
  - Has a broad range of use in electronic products 
  - Dominant Vidio Port Today 
  - Develped in 2002 
  - Designed for transmitting uncompressed video & audio through a single cable 
  - In 2009, HDMI 1.4 was released 
    - Added network communication 
    - Sends and receives data at 100 Mbit/s Ethernet 
    - 4K video at 30 Hz 
  - In 2017, HDMI 2.1 was released 
    - Higher resolutions & refresh rates 
    - 4K video at 120 Hz 
    - 8K video at 60 Hz 
    - 10K video for commercial A/V systems and specialty usages 
    
- DisplayPort 
  - Debuted in 2006
  - Developed by VESA (Video Electronics Standard Association)
  - Primarily used for video 
  - Can be used to carry USB & audio data 
  - High performance interface 
  - Can also connect to older ports by using adapters 
  - Has multi-monitor capability 
  - Allows the use of multiple monitors in a daisy chain configuration 
  - Has a locking mechanism that keeps the cable locked in place 
  - Royalty free 
  - March 2016, DisplayPort 1.4 was released 
    - Max resolution of 8K at 60 Hz 
- Thunderbolt 
  - High speed tech interface that outputs one serial signal from a combination of PCI express and the DisplayPort 
  - Can daisy chain up to 6 devices 
  - Released in 2011 
  - Version 1 & 2 Uses mini DisplayPort 
  - Version 3 Used USB type-C connector 
