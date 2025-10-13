
# Network Traffic Analysis (Wireshark)

** Objective
Capture and analyze live network traffic to understand TCP/IP communication, identify protocols, and observe connection establishment.

** Tools Used
- Kali Linux (VirtualBox)
- Wireshark
- ping command

** Steps Performed
1. Started packet capture on interface `eth0`.
2. Sent ping requests to 8.8.8.8 to generate ICMP traffic.
3. Filtered and analyzed DNS, TCP, and HTTP packets.
4. Observed TCP three-way handshake (SYN → SYN-ACK → ACK).
5. Exported results and screenshots for documentation.

** Key Observations
- **ICMP / Internet control message protocol** Showed echo requests and replies (connectivity test).  
- **DNS / Domain name system** Revealed domain queries and responses (name resolution).  
- **TCP / Transmission control protocol** Demonstrated reliable handshake between client and server.  
- **HTTP / Hypertext tramsmission protocol** Showed secure web certificate verification traffic.

** What I Learned
- How to capture and interpret packet-level communication.  
- Difference between ICMP, TCP, DNS, and HTTP.  
- How packet analysis helps in threat detection and troubleshooting.

** Screenshots
- dns : <img width="1259" height="1307" alt="dns" src="https://github.com/user-attachments/assets/7b4fe4ec-3fd6-45f1-8e0c-fba13cc1557e" />

- http : <img width="1261" height="1305" alt="http" src="https://github.com/user-attachments/assets/98063d49-2716-49b8-b06a-4b876bcf55e2" />

- tcp :<img width="1264" height="1295" alt="tcp" src="https://github.com/user-attachments/assets/cc45e6b2-54d8-44ad-9bce-384173c6b63b" />

- icmp :<img width="1265" height="1308" alt="icmp" src="https://github.com/user-attachments/assets/f452cd37-f7a0-47ec-be4b-49fca4c30b7b" />


- handshake :
<img width="1244" height="1273" alt="syn" src="https://github.com/user-attachments/assets/e3b825a5-bd01-4dc3-b161-f175bcdffb30" />

<img width="1255" height="1302" alt="syn-ack" src="https://github.com/user-attachments/assets/ef98ede6-1888-43d4-9052-cbb968267e5b" />

<img width="1252" height="1296" alt="ack" src="https://github.com/user-attachments/assets/d74380b5-b641-46fc-94f2-9caf94996dd6" />

- dns-q :
<img width="1250" height="1291" alt="dns-q" src="https://github.com/user-attachments/assets/01e120e7-63a1-44f7-9883-f14a20911fbd" />


- http-req :
<img width="1249" height="1298" alt="http-req" src="https://github.com/user-attachments/assets/bbce936f-b074-465a-9a19-2f04c8c907ef" />


- ping :
<img width="1224" height="1297" alt="ping" src="https://github.com/user-attachments/assets/7337c981-0968-4ded-a00d-892a3ec02d55" />
