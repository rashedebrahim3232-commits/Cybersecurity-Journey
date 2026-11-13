 Cybersecurity-Journey
My cybersecurity learning journey, starting from networking fundamentals and Linux basics 
## Day 1-2
- Learned the OSI model (7 layers).
- Started learning TCP/IP Model.
- Set up Ubuntu in Virtualbox.
- learned basic Linux terminal commands: `whoami`, `pwd`, `ls`, `cd` 
- Discovered Linux is case-sensitive.
# Day 3
Networking Foundamentals
- Stated learning about IP addresses.
- Learned the difference between public and private IP addresses.
- learned the basic purpose of subnetting
# Linux commands
- Practiced the following commands in the Linux terminal:
  `pwd`,
  `mkdir test-folder`,
  `ls`,
  `cd test-folder`,
  `touch myfile.txt`,
  `ls`,
  `cat myfile.txt`,
  `cd ..`,
 ` pwd`
  # Key Takeaways
  - Practiced creating files and directories.
  - Learned to navigated between directories.
  - Practiced listing files and displaying file contents.
  - Started learning IP Addressing and subnetting .
  # Day 4 - Linux File Operations and Networking Basics.
   Networking Theory.
  - Learned the difference between TCP and UDP.
  - Learned what network ports are and why they are used.
  # Linux Practical
  - Practiced the following commands in the Linux terminal:
    `echo ''hello'' > myfile.txt`,
    `cat myfile.txt`,
    `cp myfile.txt copy.txt`,
   `mv copy.txt renamed.txt`,
   `rm renamed.txt`,
    `ls -l`
   # Day 5 - Networking & Linux Practice.
    Networking.
   - Reviewed ARP and the relationship between IP and MAC addresses.
   - learned ARP Request (Broadcast) and ARP Reply (Unicast).
   - Understood the role of the Default Gateway when communicating outside the local network.
    # Linux commands.
    - Practiced the following commands in the Linux terminal:
    -`ip neigh` - viewed neighbor information.
    - `ip route` - viewed routing information and the default gateway. 
    - `clear` - cleared the terminal screen.
    - `history` - viewed previously used commands.
     # Key Takeways.
   - ARP helps a device find the MAC address associated with an IP Address on the local network.
    # Day 6 - DHCP Practical Lab
    # commands Used
    - `Ip addr`
    - `Ip route`
    # Results
    - IPv4 Address: 10.0.2.15/24
    - Default Gateway: 10.0.2.2
    - Subnet Mask: 255.255.255.0
    # What I Learned
    - DHCP automatically assigns network configuration.
    - `ip addr` - displays network interfaces and IP addresses.
    - `ip route` - displays the routing table.
    - The Default Gateway forwards traffic to other networks.
    # Day 7 - DNS Practical Basics
    # DNS Lookup
    - Used `nslookup` to query DNS records and resolve domain names, 
    `nslookup google.com`.
    # DNS Records Practiced
    - A Record - IPv4 Address: `nslookup -type=A google.com`,
      Resolves a domain name to an IPv4 address.
    - AAAA Record - IPv6 Address: `nslookup -type=AAAA google.com`, 
      Resolves a domain name to an IPv6 address.
    - CNAME Record - Canonical Name: `nslookup -type=CNAME www.github.com`
    - MX Record - Mail Exchange: `nslookup -type=MX google.com`,
      Identifies the mail servers responsible for receiving emails for a domain. Lower MX priority values are preferred.
    - PRT Record - Pointer record: `nslookup -type=PRT 8.8.8.8`, Resolves an IPv4 address to a domain name.
    - NS - Name Server: `nslookup -type=NS google.com`,
      Identifies the name servers responsible for DNS information for a domain.
    - SOA Record - Start of authority: `nslookup -type= SOA google.com`, Provides administrative information about a DNS zone , including Serial, Refresh, Retry, Expire, and Minimum.
     ## DNS Tools Practiced
    - nslookup : Used to query DNS records and analyze DNS response.
    - dig : Used to perform detailed DNS queries and analyze response sections.
    - `dig google.com`
    - `dig google.com MX`
    - `dig google.com NS`
    - `dig google.com NS +noall +answer`
    - `dig -x 8.8.8.8`
    - host : Used to perform simple DNS stub resolver.
    - `host google.com`
     ## Understanding DNS Output
    - `127.0.0.53`: Ubuntu's local DNS stub resolver.
    - `#53`:DNS server port.
    - Non-authoritative answer: The response came from a resolver that is not authoritative for the queried domain.
    - TTL: Determines how long a DNS response can remain cached.
    - DNS answers, including IP addresses, may change over time.
    - NOERROR: The DNS query was processed successfully.
    - NXDOMAIN: The queried domain name does not exist according to the DNS response. 
     ## Key concepts learned
    - A = IPv4.
    - AAAA = IPv6.
    - MX = Mail servers.
    - CNAME = Alias.
    - TXT = Text information.
    - PTR = Reverse DNS lookup.
    - NS = Name servers.
    - SOA = DNS zone administrative information.
    - DNS translates domain names into information computers can use.
    - `nslookup`, `dig`, and `host` are DNS lookup tools.
     ## Day 8-NAT and PAT Practical Basics
     # Network Configuration
    - Used `ip addr` to inspect network interfaces and IP configuration.
    - Used `ip route` to identify the default gateway and routing information.
     # Network information
    - Network interface: `enp0s3`
    - Private IP address: `10.0.2.15`
    - Subnet:`/24`
    - MAC Address: `08.00.27.18.ce.a5`
    - Default Gateway: `10.0.2.2`
    - Network Address: `10.0.2.0/24`
    - IP Assignment: Dynamic.
     # Public IP Lookup
    - Used curl -4 ifconfig.com to retrieve the externally visible IPv4 address.
    - Public IP Address: `156.207.125.45`
     # NAT and PAT Concepts
    - NAT (Network address Translation): Translates IP addresses between private and public networks.
    - PAT(Port address Translation): Uses port translation to distinguish multiple connections to their internet devices.
    - NAT Translation Table: Maps translated connections to their internet devices.
    - Default Gateway: Forwards traffic destined for external network.
     # Key concepts learned
    - Private IP = Internal network address.
    - Public IP = Externally visible IP address.
    - NAT = IP address translation.
    - PAT = IP and port translation.
    - PAT allows multiple devices to share one public IP address.

     ## Day 9 - Routing & Switching Basics
     # Theory covered
    - Hub vs Switch vs Router
    - OSI Layer 2 and Layer 3
    - Routing Table
    - Static Routing and Dynamic Routing
    - Default Route and Default Gateway
    - Next Hop
    - Connected Routes
    - Longest Prefix Match
     # Practical Commands
     1. Display Routing Table
   
   
