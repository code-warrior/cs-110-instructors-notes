## CS 110 Lecture Notes

---

* What is input to a computer?
  + Keyboard, Mouse, Scanner, Wacom, Trackpad, Touch (as in iPhone), etc
* What is output to a computer?
  + Screen, Screen (as in iPhone), Printer
* Data is processed by the CPU, or Central Processing Unit
* References to “memory” means RAM, which is volatile; Retains data as long as power is available
* Long-term Storage is a traditional hard drive or solid state drive (SSD). It’s non-volatile: Data is kept after power to the computer is turned off
* IPOS: Input, Process, Output, Store
* Stored programs allow the computer to switch tasks
* The ability to switch between tasks is what makes a computer a multi-purpose device
* Digital electronics represents data as bits
   + Bits: 1 or 0, HI or LO; binary
* Buying a computer
* An IC is an integrated circuit: A set of microscopic electronic components
* Three historical categories of computers:
  1 — **Mainframes**: Large, room-sized machines in metal frames
  2 — **Minicomputers**: Smaller and support multiple users
  3 — **Microcomputers**: Single user
* The term “minicomputer” isn’t used very often.
* Mainframes
  + Primarily used by business and government
  + Large; Expensive (upwards of hundreds of thousands of dollars)
  + Used to centralized large amounts of data
+ Servers
  + Serve data to many Internet connected users
  + Your home computer can act as a server — a slow one

## Microprocessors
* Intel introduces the first microprocessor: the 404
* The 8086 chip family set the standard for today’s chips
* This standard is often referred to as an x86, where the “x” represents the numbers leading up to the “86” in the chip name: 8086, 80286, 80386, etc
* Modern computer deal with with i3, i5, i7, and i9
* Configure a machine at Dell: [https://www.dell.com/en-us/shop/scc/sc/laptops?~ck=mn](https://www.dell.com/en-us/shop/scc/sc/laptops?~ck=mn)
* Configure a Mac at Apple: [https://www.apple.com/shop/buy-mac/mac-mini](https://www.apple.com/shop/buy-mac/mac-mini)
* While x86 chips are found in desktops/laptops/servers, ARM (Acord RISC Machines) processors are found in phones and tablets
* ARMs are energy efficient, which is a high requirement for portable devices

## How Processors Work
* Microprocessors handle a limited set of activities called an *instruction set*
* Instruction sets are endemic to their processor
* x86 instructions are not compatible with ARM instructions
* ARM contains a simple instruction set: ~ 35
* x86 contains a larger instructions set: 100+
* Programming languages such as Java, C, JavaScript, C++, etc, are high level languages
* High level languages need to be translated into machine language, which corresponds to the microprocessor’s instruction set
* An example of what machine language looks what is found on page p107
* A microprocessor contains an Arithmetic Logic Unit, or ALU
* The ALU works with its Control Unit. Together, they work to process the instructions in RAM
* Gigahertz means a billion cycles per second
* 3.4Ghz means 3.4 billion clock cycles per second
* A “core” refers to a microprocessor’s ALU *and* control unit
* A processor with more than one core is called a multi-core processor

---

## Serial, Pipeline, and Parallel Processing
* **Serial**: One instruction at a time, each completing before a new one is fetched
* **Pipeline**: Before completing an instruction, a new one is fetched
* **Parallel**: Multiple instructions at a time
* Make an analogy of getting coffee at a coffee shop

---

## Cache
* Special, high-speed memory that allows a microprocessor to access data more quickly than RAM
* Measure in MB *not* GB
* Level 1 is quickest; Level 3 is slowest. Using any level is faster than accessing RAM. (See p103)

---

## Word Size
* Controls amount of memory processor can access
* 32-bit fits less than 64-bit, obviously
* Windows can run 32- and 64-bit programs
* On a 32-bit version of Windows, all 32-bit programs are kept in `C:\Program Files`
* On a 64-bit version of Windows, 32-bit programs are kept in `C:\Program Files (x86)`, while 64-bit programs are kept in `C:\Program Files`
* macOS Mojave (`10.14`) [2018] is the last version of macOS that supports 32-bit apps
* macOS Catalina (`10.15`) [2019] is the first version of macOS to support **only** 64-bit
* Complex instruction sets use the Complex Instruction Set Computer, or CISC, technology
* Simple instruction sets use the Reduced Instruction Set Computer, or RISC, technology
* The “R” in ARM stands for RISC. (The remainder is Acord RISC Machines, Acord being the company)
* RISC is typically faster, but may require more instructions to do the same task as a CISC
* Desktop/laptops/ use CISC; mobile devices use RISC

---

## Module 3 — Network Basics
* PAN – Personal Area Network
  + Within 30 feet and wireless
  + Serves a single user
  + Smart devices
  + AirDrop in macOS
  + Syncing phone to computer
  + Sending a job to a printer
* LAN — Local Area Network
  + Home network
  + School computer lab
  + School WiFi
* WAN
  + Phone systems
  + The Internet

---

### Communication Channels
* Let’s start with a question: Is a wireless connection more or less secure than a hard-wired connection?
* A comm channel is a medium by which to transport info between network devices
* There are two comm channels
  + Wired
  + Wireless

#### Communication Channels — Wired
* See p162 for type of network cables
* Fast
* Cannot be sniffed by an outsider
* Cables can be shielded from interference
* Not susceptible to interference from the elements or other electrical devices
* More secure, because only wired devices can connect to the network. For example, you disable WiFi broadcasting on your modem and connect everything hardwired
* Disadvantages include
  + Must be hidden or buried
  + Can get damaged
  + Limited mobility
  + Messy
  + Susceptible to electrical surges

#### Communication Channels — Wireless
* Two types
  + Radio (known as RF, or Radio Frequency, channels)
    - Bluetooth
    - WiFi
    - Voice and data bet smartphone and tower
    - Uses a transmitter/receiver: a transceiver via antenna
  + Microwaves
    - Have more carrying capacity than RF
    - Line of sight must be clear
    - Cannot penetrate metal objects
    - Typically used to transmit signals bet tower in cell and wide area wireless installations
* Mobility is the most advantageous feature of wireless
* The disadvantages include speed, range, security, and licensing
  + Other electronic devices can interfere with wireless, forcing retransmission
  + Walls, flooring, and ceilings interfere with a wireless signal
  + Distance, like a radio signal, also affect wireless
  + The strength of the wireless signal
  + Insecure, as anyone who knows something about networking can access your network, akin to having someone in your home

#### Communication Channels
* Licensing fees apply to radio and TV stations, because they’re on a frequencies regulated by the FCC
* Licensing feeds *don’t* apply to 2.4 GHz or 5 GHz, ranges used by consumer-grade WiFi routers
  - 5 GHz handles interference better, but limits range
  - 2.5 GHz is more ideal for longer ranges
  - Most routers today are available in both, and this can be seen in a router’s WiFi Service Set Identifier, or SSID, which is a fancy name for the name of the wireless signal being broadcast
* Bandwidth defines the capacity of a comm channel
* Coax has a higher bandwidth than a telephone line
* Broadband is defined as 25 megabits of data per second, or Mbps
* Narrowband is defined as slower than 25 Mbps

---

## Display Devices

* Two types of displays:
  1. Liquid Crystal Display, or LCD
  2. Light-Emitting Diode display, or LED
* LCDs work by a backlight plane that displays light through a grid of liquid crystal cells
* The cells are grouped in dots, or pixels (picture elements), with each group containing 1 red, 1 green, and 1 blue liquid crystal cell
* Liquid crystals can only produce light via a light source, such as a backlight plane
* LEDs are sometimes the backlight source. These are known as LED screens.
* The specifications that define screen quality:
  + How fast it responds (response rate),
  + What distance exists between pixels (dot pitch) and,
  + The amount of pixels (screen resolution)
* **Response rate**: Black → white → black; faster is better, especially gaming; 5ms is common
* **Dot pitch (or pixel pitch)**: Distance between center of RGB liquid cell and the center of another RGB liquid crystal cell; smaller distance is clearer
* **Screen resolution**: More pixels packed into an inch (pixels per inch), the finer detail is achieved

## Touch Screens
* Resistive, where a layer hovers over the screen; a small distance exists between the screen and the resistive layer
* Capacitive, like your phones, has a layer of transparent electrical conductive material and can be triggered by the capacitance in our bodies; unlike resistive screens, there no distance between the interactive layer and the screen

## GPU
* `Integrated graphics` refers to the circuitry on the system board that handles graphics
  + It processes all the graphics data on the computer’s chip, thus sharing it
* `Dedicated graphics` refers to circuitry mounted on a board known as a graphics card or video card
  + Contains a Graphical Processing Unit, or GPU
  + It’s a microprocessor dedicated to processing graphics
  + Contains memory to store images before being displayed
  + Like a CPU, it gets hot, so it requires its own heat sink and fan
  + Works alongside a CPU, unlike integrated circuits that share the CPU

## Printers

### Printers — InkJet
* Uses liquid ink
* Uses CMYK ink cartridges: Cyan, Magenta, Yellow, and Key, or black
* Uses nozzles to spray ink onto paper
* Prints fewer pages
* Cartridges are expensive, and have to be replaced more often
* Ink will run if pages ever become wet

### Printers — Laser
* Uses ink-infused plastic
* Drum melts the plastic onto the paper
* A large burst of energy is required to heat the powdered plastic onto the paper; it’s why laser jet printed paper is warm
* This does not occur with inkjet printers
* Not susceptible to water damage
* Cartridges are much more expensive, but print much more paper than inkjet

### Printers — 3D
* Technically called additive manufacturing
* Use coil filaments
* Scanning larger objects requires a larger scan bed
* Scanning to more detail takes longer; hours in some cases

---

## Network Topology
* Structure/layout of network components
* Point-to-point
  + Connecting your phone to your computer
* Star
  + Connecting multiple devices to a central device
* Mesh
  + Connect multiple devices to each other
* Full mesh
  + Every device is connected to every other device
* Partial mesh
  + Outer nodes not connected to every other node

## Star
### Dependability (Star)
* Removing the central point breaks the entire network
* If one of the outer elements fails, the rest of the network is unscathed

### Security (Star)
* Data between two outer points crosses only the center
* The threat is only between 3 devices and 2 channels

### Capacity (Star)
* Limited by what can be handled by the center

### Expandability (Star)
* Limited by the distance from the center component, by way of wireless or wired

### Control (Star)
* Setup and updates carried out by the central device
* Entire network can be shut off from the central device

### Monitoring (Star)
* All data passes through the central device, making it easier to monitor data

## Mesh
### Dependability (Mesh)
* Redundant paths can bypass failed devices

### Security (Mesh)
* Multiple path points expose risk

### Capacity (Mesh)
* Data can be transmitted from different devices at the same time, offering higher capacities

### Expandability (Mesh)
* Simply add another device to the mesh, which will slow things down

### Control (Mesh)
* More complex to setup — Each device must send, receive, and transmit data

### Monitor (Mesh)
* Data takes diff paths, making it harder to monitor

## Network Devices (p169)
* **Hub**: Extends a network and broadcasts to all devices on the hub. *Not* what you want at home
* **Switch**: Data routed to each connection on the switch individually. What you likely want at home
* **Bridge**: Simply connects two similar networks. *Not* what you want at home
* **Repeater**: Restores signal to maximum strength, then repeats it. What you might want at home
* **WAP**: Allows wireless devices to connected to a wired network. What you likely want at home

---

## History of The Internet (p172)
* Sputnik in 1957
* The Advanced Research Projects Agency, or ARPA, was created as a result
* First Internet message was sent in 1969 between UCLA and SRI
* First browsers in the early 1990s
* ICANN (Internet Corporation for Assigned Names and Numbers) supervises Internet addressing

## The Internet
* The Internet is an interconnected network of networks
* A 3-tiered structure

### Tier 1
* The backbone is a system of high-capacity routers and fiber-optics links
* AT&T and Verizon, for example, form part of the backbone
* Configured as a mesh
* Recall that a mesh provides redundancy
* Book discussed myth that the Internet was invented to save data in the face of a nuclear disaster. *This is not true*, likely because the authors read that Time article from the 90s

### Tier 2
* Internet Service Providers, or ISPs, operate at this level
* Consumers usually connect at this level

### Tier 3
* Colleges
* Home networks
* Consumers connect at this level, also

## Packets
* Files are divided into chunks and packaged with reassembly info
* Those packets are sent over the Internet’s mesh network
* On arrival, they’re re-assembled, based on the package info
* TCP ensures the entire file reaches its destination

## Comm Port
* When data arrives on your computer, it’s redirected along a port
* Although there are about 65,535 ports, we consumers only use about 10–20
* Web data is transmitted along port 80
* Video along port 554

## Internet Addressing
* The “IP” portion of TCP/IP deals with Internet addressing
* Two IP versions: IPv4 (original) and IPv6 (2011)
* Developed in the 1970s, IPv4 can handle ~ 4 billion addresses. This was unheard of in the 1970s
* IPv6 can handle billions more devices than IPv6
* Every item connected to the Internet must have an IP address

## Static Addressing
* A single IP address that doesn’t get re-assigned. (http://whatismyip.com)

## Dynamic Addressing
* A different address is used per session

## Domain Names
* A domain name is what you type into your browser, like http://www.hartford.edu
* A domain is synonymous with an IP address, which is harder to remember than, for example, http://www.hartford.edu

## Top-Level Domains (TLD) (p183)
* “.edu” is the TLD from www.hartford.edu

## How it Works
* Around the world exist domain name servers, or DNS, that keep a key-value pair of domain name and IP address
* When you type http://hartford.edu, your request is sent to a DNS server, and it responds with the IP address of your domain, then your router fetches the site at that domain.

## Connection Basics
* Visit http://speedtest.net in class
* Use `traceroute` in The Terminal or `tracert` in Windows to show network hops

---

### Software Categories
## System Software
* OSes: macOS, Windows, Linux, iOS, Android, ChromeOS
* Device drivers for hardware
* Utilities, such as backup software, networking, etc

## Development Software
* C, C++, Java, etc
* JavaScript, PHP, Python (scripting), SQL (databases)
* QA Tools: Debuggers (to make sure there are no issues in the programs you might write in C or Java, for example)
  Security (to make sure any known security risks are found)

## Applications (or apps, as coined by Apple for the iPhone)
* Everything else

## Essential for Desktop/Laptops (p 381)
* The OS (Linux, macOS, Windows)
* System utilities
* A browser
* Network utilities

## Essential for Mobile
* The OS (iOS, Android). (It’s possible to jailbreak an iPhone)
* System utilities
* A browser
* Network utilities

## Distribution
### What Makes Up an Application?
* In Windows, a `.exe` file
* In Mac, a `.app` folder
* On the Internet, many places offer software
  * Google Play and The App Store provide best security practices for their devices
  * Open source software is fully transparent, so if you see a GitHub or Bitbucket logo, you can trust them
* When downloading software, ensure you see the lock in the address bar

---

## “Buying” Software
* Sometimes you buy a license to stop being nagged (Sublime Text), called nagware
* Sometimes it’s entirely free via an open source license
* Sometimes it’s free, but users are charged for support calls, such as Apache, the world wide web server
* Sometimes you pay for a subscription
* Sometimes you just outright buy software, which might be bound to a USB dongle
* For software on an external medium, such as a flash drive, you can make a copy for a backup
  + If you sell the software, you’re supposed to
    - also provide the copy to the buyer,
    - destroy the copy if the buyer refuses it, and
    - remove the software from your machine
* There’s also the freemium model, like Windows 10, originally

## Licenses
* Sometimes you get a license (Sketch or Max)
* That license might last a certain amount of time
* That license might only be valid for a single version (Max)
* A site license allows multiple machines to use the software, like at school
* Freeware is licensed but not charged
* Activation codes unlock software
  + Old versions of Windows were bound to a license key
    - repeat installations only required the license key
  + macOS doesn’t observe this position when it comes to their operating systems

## Operating Systems (p390)
### Desktop
* macOS
* Windows
* Linux
* ChromeOS

### Mobile
* iOS
* Android
* watchOS

### Servers
* Apache
* Linux
* Windows
* macOS Server

* On mobile devices, the OS is stored in ROM, or read-only-memory
* On computers, it’s stored on disk
* During boot, after the hardware check, the OS is loaded into RAM

## Multitasking
* Means that the processor and memory are being used by multiple programs
* Think of running Firefox and Spotify at the same time

## Multithreading
* Think of running spell check as you type into Word
  + The OS has to direct typing into Word
  + It might also be running a spell-check as you type

## Multiprocessing
* …carried out via multiple processors

## Memory Management
* The OS allocates memory to a program, or app
* If the program/app requests memory and doesn’t release it, we have a memory leak
* Your OS will buffer some tasks to ensure they don’t get lost
   - Consider lagging keyboard input

## Windows
* Originally started as Disk Operating System, or DOS
* DOS’ kernel, or skeleton, was used to create Windows, first released in 1985
* Many versions
   + Windows Home
   + Windows Pro and Enterprise that can handle encryption, remote access and managing network user groups
   + All versions can handle tablets
   + Windows Mobile
* 80% of people use Windows
* Windows used to be about 98 or 99% of users
* Windows is susceptible to viruses, malware, etc.

---

## macOS
* Classic Mac OS (Today written as macOS)
* Play 1984 commercial: https://www.youtube.com/watch?v=zIE-5hg7FoA
* Original Classic Mac OS used a Motorola 68000 microprocessor
* In 2001, Apple released Mac OS X to run on a PowerPC (Performance Optimization With Enhanced RISC – Performance Computing) processor
* In 2006, Apple pivoted again, this time from PowerPC to Intel processors
  + Universal binaries were introduced to ease the transition
  + Mac OS had to be rewritten again, this time for the new Intel chips
    - 10.4.4
    - You used have to pay for 10.4
* Mac OS’s kernel is UNIX
* Some Mac files contain two parts, called forks
  + Part I: the data fork, containing the data, such as test
  + Part II: the resource fork, `.DS_Store`, which contains info about the data fork

## iOS
* iPhones, iPads, and the discontinued iPods
* Both macOS and iOS are derived from the same UNIX kernel
* iOS limitations
  + Only apps provided by Apple may be used
  + No file manager; access to file system, like in a regular OS
  + Jailbreaking, or rooting, your phone allows you to bypass the inherent limitations
    - Access to apps outside of the Apple store
    - Access to the file system
    - Gets wiped during a software update
    - It’s illegal, but I’ve never heard of anyone being charged for the crime

## Android
* Has version names like, Ice Cream Sandwich, Eclair, and Jelly Bean
* Used on phones, WearOS, and TV streaming devices
* Made from a UNIX derivative — Linux
* Beta released in 2007; officially released in 2008
* Can be hacked onto an iPhone, although I’ve never seen it
* Has WiFi hotspot, as does iPhone
* A file manager is available
* Used to not be updated by manufacturer
  - Since the Google Pixel was released in 2013, Google updates
  - Samsung also updates
  - Compare updates with iPhone
* Jailbreak not really needed, primarily because software may be downloaded from various sources, not just the Play Store

## ChromeOS
* Also based on Linux
* A thin client, meaning it relies on an external machine for processing and storage. AKA zero clients or network computers
* Very limited — Only really a browser and some email

## Linux
* A portmanteau of Linus and UNIX
* Created while Linux Torvalds was an undergraduate at The University of Helsinki
* Open source via the General Public License, meaning anyone can fork it for commercial and non-commercial endeavors
* Android, ChromeOS, and Kindle are examples of technologies based on Linux
* Ubuntu is likely the most popular Linux distribution in existence
* There are many drivers available for legacy products
* There are many software programs for Linux, including open source equivalents of…
  + Photoshop, (The GIMP)
  + Microsoft Office (LibreOffice)
* A lot of tinkering is required to get hardware to work
* Freely downloadable from The Internet
* Requires some advanced technical knowledge

## Virtual Machines
* A software program that provides a layer onto which to install another OS
* Launching the software is like booting a computer, and then you can have one OS running as a program on top of your current OS

---

## Web Apps
* Client Side: Your browser
* Server Side: The database that cannot be seen by the user
* Examples are Google Docs
* Users don’t install anything; code is transmitted over The Internet
* Imagine if you had to install hundreds of MBs onto your machine every time you visited a web app
* Access is via browser
* You need the Internet, of course
* You can access from phone, tablets, and computers, but may not work across all
* Up to date, since the software is not maintained on your machine
* Fewer features
* You rely on the durability of the external site server
* You’re more vulnerable, since content travels between your machine and the server

## Mobile Apps
* Are applications installed on your mobile device
* Have access to your phone’s sensors
* Are potentially more secure
* Work faster, can access device and system resources, and can work without Internet access
* Are expensive to build and more difficult to maintain
* Need to be built from scratch

## Office Suites
* Google Docs
* Microsoft Office
* Apple has iWork
* LibreOffice (open source)
* OpenOffice (open source)

## File-Naming Conventions
* macOS and Windows limit to 255 characters
* File separators, such as the colon in Windows and the backslash in macOS, cannot be used

## Storage Device Designations
* Where is the storage device in the file structure tree
* `C:\`, `D:\`, etc in Windows; legacy convention left over from MS DOS (1981–2000)
*  `/Volumes/` in macOS

## Root
* In Windows, C
* In Mac /

## Partitions
* Two devices appear to be separate, but exist on the same drive
* Boot Camp (Windows) and macOS on separate partitions but the same disk
* A recovery partition might exist to help you restore your machine

## Physical Storage (p436)
* Logical Storage Model is what the user sees
* Physical Storage Model is how files are actually stored
* Windows uses New Tech File System (NTFS)
* macOS uses Hierarchical File System Plus (HFS+) or Apple File System (APFS)
* When files are deleted, they’re not really deleted. Explain lazy deletion

## Encryption (p455)
* Encryption transforms a message or a file into other data that needs to be decrypted in order to see the original message/file
* An unencrypted message/file is referred to as cleartext or plaintext
* An encrypted message/file is referred to as ciphertext
* The algorithm to encrypt data is called a cryptographic algorithm
* A cryptographic key is better known as a password
* What can be encrypted?
  + Data over the Internet
  + Email
  + Files
  + Entire drives

### Authentication
* Any technique used to verify a user’s identity
* 2FA, or 2-factor authentication, usually also requires a verification code, along w/a password
* When an iOS device is locked, its storage volume is automatically encrypted
* Long passcodes take longer to crack
* iPhone users: Take a moment to look at how to make yoru data more secure (p456)
* On laptops/desktops, require a password to wake
* Use BitLocker (if you use Pro or Enterprise version of Windows) to encrypt your drive
* Use FileVault in macOS
  + Disable automatic login

### How are Passwords Compromised?
* Physical piece of paper
  + I’ve seen people put their passwords on a Post-It note on their computers
  + People keep them on piece of paper in their wallet
* Brute-force attack — Guess every password
  + Can take days to crack
* Dictionary attack — Look for words in English, Spanish, French, German
  + Will also look like loveyou, l0vey0u, and l0v3y0u
* Look on p460. Do you use any of those passwords?

### Weak Passwords
   + Dictionary words
   + Doubled words, such as, sunsun
   + Default passwords
   + Passwords ending in 123 or a year, such as 2020
   + Dates
   + Phone numbers
   + c0ff33

* !! Password combo: # of chars ^ password length
   + 10 possible values (0–9)
   + 4-digit password
   + 10⁴ = 10,000
   + 10⁸ = 100,000,000
* Password strength is measured in entropy as log₂(POSSIBLE_COMBINATIONS) (p462)
* Larger entropy results means more secure passwords
* For example,
  + log₂(10⁴) = log₂(10000) = 13.28, rounded up, means entropy is 14-bit
  + log₂(10⁸) = log₂(100000000) = 26.57, rounded up, means entropy is 27-bit
  + log₂(94⁸) = log₂(6095689385410820) = 52.43, rounded up, means entropy is 53-bit
* Calculate entropy on your computer:
  1. Use `xʸ` on a scientific calculator to locate the result of something like 94⁸
  2. Then press `log₂` to get the amount of bits
* Hints for creating secure passphrases: p463

### Passwords Manager
* Sometimes called a “keychain”
* Create passwords for you
* May display a strength meter
* Passwords are encrypted
* A master password unlocks the manager
* Downsides
  + If master password is compromised, then everything is available
  + If you forget the master password, it can be impossible to retrieve
* Storing a passwords file…
   + On your computer is risky, because, if lost, people can take their time cracking the master password
   + In the cloud is risky, because your info can be intercepted
   + On a USB flash drive is risky, because you can lose it

## Malware (malicious software) (p467)
* Refers to any computer program designed to secretly enter a digital device
* Classifications
  + Viruses
  + Worms
  + Trojans
* An action carried out by malware is a “malware exploit” or a “payload”
* Exploits include
  + Deleting files
  + Recording keystrokes
  + Opening “doors” for others to enter
  + Remote control
  + Pop-up ads/messages
  + Encrypt data and then demand a ransom for the encryption key
  + Transfer files
  + Disable firewalls and antivirus

### Virus
* Self-replicating program that secretly attaches itself to a regular file on a host device
* They’re not self-distributing
* They’re known as “time bombs” when they do their damage at a specific time
* They’re known as “logic bombs” when they respond to some other event
* Spread when people exchange files on flash drives, via email attachments, and on file sharing networks
* Side-loaded via pirated software from app stores

### Rootkits
* Essentially, rooting a user; for example, exploiting the macOS root user account
* Can install a virus, then hide its existence

### Worms
* Self-replicating, self-distributing, and designed to carry out unauthorized activity on a device
* Mass-mailing worm
  + sends itself to everyone in a contact list
* Internet worm
  + seeks vulnerabilities in OSes, open ports, and JavaScript — including PDF
  + when it finds a host, it can connect over the wire and request more malware
* File-sharing worm
  + copies itself into a shared folder under innocuous name

### Trojans
* Appears to perform one function while actually doing another
* **Not** designed to self-replicate

---

## Intrusions
* A Remote Access Trojan, or RAT, is a Trojan w/a backdoor
* A backdoor is a secret communications link
* Ensure Remote Desktop (Win) and Screen Sharing (Mac) are disabled (p480)
* Ransomware (p481)
  + Entire device is locked
  + People who carry out ransomware rarely provide the unlock code
  + It‘s really designed to take advantage of those who don’t back up
  + Companies usually don’t pay to unlock
  + Your best plan of action
    - Backup often
    - Make sure you don’t keep questionable items on your phone
      ^ If you can’t show everything on your phone to your parents, then you’re in trouble
    - If you’re the target of ransomware
      ^ Scrub the device and start again
* Botnet: Many computers organized into a client-server network
  + Can be made up of any device that connect to the Internet, including IoT devices
  + Distributed Denial-of-service, or DDOS, attack. See https://en.wikipedia.org/wiki/2016_Dyn_cyberattack
* Zero-Day Attack
  + Dangerous, because it has been alive for 0 days, meaning no one — including antivirus software — is aware of it
  + Adobe Reader (because of JS in PDF, remember), Windows, Android, and Adobe Flash (because of JS) are most susceptible

## Netstat
* Recall that computers can have up to 65,535 ports (page 178)
* A port scan pings a packet of data to a port. If the port responds, then it’s open

## Firewall
* A device or software that allows permissible communication
* Disallows unauthorized communication
* Essentially is a deterrent to unauthorized port access
* A router may have firewall features
* Don’t use more than one, as they may conflict

## Interception Basics
* **Spyware** secretly gathers your info
  + Can take remote control of your device
* **Adware** monitors your machine’s Internet traffic and sells it to advertisers
* **Keyloggers** record keystrokes on your computer
* **MITM** is a man in the middle attack, usually carried out with a Pineapple
  + Intercepts traffic
    - May be passive
    - Or, may alter traffic
    - Tricks both parties into thinking they’re talking to each other
* **Evil Twin** is a LAN server designed to look legitimate
  + It’s a WiFi hotspot without a password
  + The content is transferred to web sites, but it’s copied along the way
  + Users may never know their data is being intercepted and copied
  + **Avoid** by never joining a network you don’t know, especially if it doesn’t require a password

## Address Spoofing
* Changes an originating/destination IP address to redirect data

## Digital Certificate
* See page 492
* A *fake* digital certificate contains
  + server’s credentials
  + encryption key
  + *fake* signature
* Keep an eye out for fake certificates; you’ve probably seen the dialog box before

## IMSI, or International Mobile Subscriber Identity, Catcher
* The mobile equivalent of a pineapple; a MITM attack
* Sometimes known as a stingray
