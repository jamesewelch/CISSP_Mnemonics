# Domain 1: Security and Risk Management

## Ethics

### ISC2 Ethics Canons

PAPA
* Protect, Act, Provide, Advance

## Risk Managment

Annual Lost Expectancy = Annual Rate of Occurrence * Single Loss Expectancy
* ALE = ARO * SLE

## Threat Modeling

STRIDE
* Spoofing
* Tampering
* Repudiation
* Information Disclosure
* Denial of Service
* Elevation of Privilege

DREAD
* Damage
* Reproducibility
* Exploitability
* Affected users
* Discoverability

## Control Types

PTA
* Phyiscal
* Technical/Logical
* Administrative

## RMF Framework 

Crime Scene Investigators Always Act Modestly
* Categorize
* Select
* Implement
* Assess 
* Authorize
* Monitor

# Domain 2: Asset Security

### US Military Classifications

U S Can Stop Terrorism 
* Unclassified
* Sensitive But Unclassified
* Confidential
* Secret
* Top Secret

# Domain 3: Security Engineering

### Notes
* Ceaser Cipher = Ceas3R (3 to right)
* Twofish = pre and post whitening

### <u>Symmetric Encryption</u>

23BRAIDS
* Twofish (2 fish)
* 3DES
* Blowfish
* RC5 (RC4, RC6)
* AES
* IDEA
* DES
* Skipjack 

RC4 is streaming

DES and 3DES modes
* ECB (initial/first, doesn't support initialization vector)
* the other 3 in middle are alphabetical (CBC, CFB, OFB)
* CTR (last)

### <u>Asymmetric Encryption</u>

DEREK 
* Diffie-Hellman
* Elliptic Curve
* RSA
* El Gamal
* Knapsack

Discrete logarithms
* Diffie-Hellman
* El Gamal
* Both sound like calculus professor names

### <u>Hash Functions</u>

MSHH
* MD5
* SHA-1/2/3
* HMAC
* HAVAL


## Security Models

Brewer-Nash
* "Chinese Wall", Conflict of Interest, China "brews" tea

Simple Property
* Reading is Simple

Star ( * ) Property
* It's Written in the stars

Integrity vs Confidentiality models
* Integrity models have "i"
  * Biba = Integrity
  * Clark-Wilson = Integrity
* Confidentiality
  * Bell-LaPadula = Confidentiality

Confidential
* NRU (No Read Up)

Bell-Lapdula (No read up, no write down)
* (No) Ride Ugly White Donkey
* Biba is opposite (No read down, no write up)

Clark-Wilson
* TLC - Tampered, Logged, Consistent

# Domain 4: Communications and Network Security

### <u>Firewalls</u>

Firewalls are layer 1, 4, 5, 7 
* Layer 1 = Stateless
* Layer 4 = Stateful
* Layer 5 = Circuit, Stateful, Anomaly
* Layer 7 = Application

### <u>The OSI Reference Model</u>

Physical (1), Data Link (2), Network (3), Transport (4), Session (5), Presentation (6), Application (7)

Bottom Up 1-7
* Please Do Not Throw Sausage Pizza Away
* Please Do Not Touch Steve’s Pet Alligator
* Please Do Not Teach Students Pointless Acronyms
* Please Do Not Tell Sales People Anything
* Please Do Not Tell Secret Passwords Anytime
* People Don't Need Those Stupid Packets Anyways 
* People Don't Need To See Paula Abdul 
* People Don't Need To See Pamela Anderson

Top Down 7-1
* At Present, Some Teachers Need Dr. Phil
* All People Seem to Need Data Processing
* All Presidents Say They Never Did Pot

### <u>PDU Names</u>

Data (7,6,5), Segments (4), Packets (3), Frames (2),  Bits (1)

Top Down 7-1
* Don't Stop Pouring Free Beer
* Don't Spill Paul's Free Beer
* Don't Smoke Pot From Bongs

### <u>TCP/IP Model</u>

Application, Host, Internet, Network
* All Happy Insects Nest

Application, Transport, Internet, Network Access
* Armadillos Take in New Ants 

Network, Internet, Transport, Applicaton
* NITA

### <u>DHCP IP Assignment</u>

Discover, Offer, Request, Acknowledge
* DORA (the discoverer)

### <u>TCP Flags</u>

Urg (32), Ack (16), Psh (8), Rst (4), Syn (2), Fin (1)
* Unskilled Attackers Pester Real Security Folks

# Domain 5: Identity and Access Management

# Domain 6: Security Assessment and Testing

### <u>TCSEC (Trusted Computer System Evaluation Criteria) Orange Book
  
* A - Verified
* B - Mandatory
* C - Discretionary
* D - Minimal

# Domain 7: Security Operations

### <u>Incident Response</u>

Prepare, Detect, Response, Mitigate, Report, Recovery, Remediate, Lessons Learned
* Please Don't Rub My Red Round Rash Larry

### <u>Forensic Evidence Steps</u>

IP CEA PD
* Identify
* Preserve
* Collect
* Examine
* Analyze
* Presentation
* Decision


### <u>Fire Extinguisher Classes</u>

USA Classes
* A - Ash -> Combustible 
* B - Boil -> Liquid 
* C - Current -> Electrical 
* D - Dent -> Metal 
* K - Kitchen -> Oil/Fat 

# Domain 8: Software Development Security

### <u>CMMI</u>

IRDMO (thIRDMOon)
* Initial
* Repeatable
* Define
* Measure
* Optimize

### <u>Database Security</u>

ACID
* Atomic
* Consistency
* Isolation
* Durability

### <u>Pentration Steps</u>

PIVER
* Planning
* Information gathering and discovery
* Vulenerability mapping\scanning
* Expoitation
* Reporting

DEVER
* Discovery
* Reconnaisance
* Enumeration
* Vulnerability mapping
* Expoitation
* Report

PAP - Pen testing from CEH 
* Planning or pre-attack
* Assessment or attack
* Post-Assessment or post-attack

Hacking phases (CEH)
* Reconnasiance
* Scanning
* Gaining Access
* Maintaining Access
* Covering Tracks

### <u>Ring Model</u>

KODU
* -1 Hypervisor (type 1)
* 0 Kernal
* 1 Operating System
* 2 Drivers
* 3 User
 
# Unsorted

RAID
* RAID 1 = imagine the "1" is a mirror
* RAID 0 = imagine a circle of writing across multiple disks


| Layer  | Name |  Attacks | Hardware | Protocols  
| --- | --- | --- | --- | ---
| Layer 7 | Applicaton | Worms | applications, application firewall, proxy firewalls | SOAP, DHCP, HTTP/S, DNS, POP3, SMTP, FTP, NTP, IMAP
| Layer 6 |Presentation| ? | .jpg, .mime, etc  | TLS, SSL, FTP, IMAP, SSH, Telnet 
| Layer 5 |Session|? | Circuit Firewalls |H.245,NetBIOS,SOCKS
| Layer 4 |Transport|SYN, Fraggle|Stateful Firewalls|NetBIOS, TCP, UDP
| Layer 3 |Network| Loki, Smurf, Teardrop| routers | IPX, NAT, AppleTalk, IP, ICMP, RIP, OSPF, IPSec
| Layer 2 |Data Link|    MAC spoofing     | switches, bridges   | ARP, CHAP\PAP, FDDI, IEEE 802.11 WiFi & IEEE 802.16 WiMax, L2TP\PPP\PPTRP, VLAN
| Layer 1 | Physical| evesdropping (splicing wires) | hubs, repeaters statelss firewalls  | DSL, ISDN, Frame Relay, Modems
