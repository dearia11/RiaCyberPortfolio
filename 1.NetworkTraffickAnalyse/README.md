
# Network Traffic Analysis (Wireshark)

# Objective
Capture and analyze live network traffic to understand TCP/IP communication, identify protocols, and observe connection establishment.

# Tools Used
- Kali Linux (VirtualBox)
- Wireshark
- ping command

# Steps Performed
1. Started packet capture on interface `eth0`.
2. Sent ping requests to 8.8.8.8 to generate ICMP traffic.
3. Filtered and analyzed DNS, TCP, and HTTP packets.
4. Observed TCP three-way handshake (SYN → SYN-ACK → ACK).
5. Exported results and screenshots for documentation.

# Key Observations
- **ICMP / Internet control message protocol** Showed echo requests and replies (connectivity test).  
- **DNS / Domain name system** Revealed domain queries and responses (name resolution).  
- **TCP / Transmission control protocol** Demonstrated reliable handshake between client and server.  
- **HTTP / Hypertext tramsmission protocol** Showed secure web certificate verification traffic.

# What I Learned
- How to capture and interpret packet-level communication.  
- Difference between ICMP, TCP, DNS, and HTTP.  
- How packet analysis helps in threat detection and troubleshooting.

