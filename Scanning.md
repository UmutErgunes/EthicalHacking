## Scanning
We are going to look for 3 things: Ports, Network & Vulnerability.


<b>Port Scan</b>: Method of determining which ports on a network are open and could be receiving or sending data. It is also a process for sending packets to specific ports on a host and analyzing responses to identify vulnerabilities. <br>

<b>Network Scan</b>: Refers to the use of a computer network to gather information regarding computing systems. Network scanning is mainly used for security assessment, system maintenance, and also for performing attacks by hackers.<br>

<b>Vulnerability Scan</b>: Inspection of the potential points of exploit on a computer or network to identify security holes. A vulnerability scan detects and classifies system weaknesses in computers, networks and communications equipment and predicts the effectiveness of countermeasures. <br>


#### Port Scan - Nmap
- Exemples:
     * nmap -sP 192.168.0.1/24  <b>-> Ping analysis </b>
     * nmap -PS 192.168.0.1/24  <b>-> TCP - SYN analysis </b>
     * nmap -PA 192.168.0.1/24  <b>-> TCP - ACK analysis </b>
     * nmap -PE 192.168.0.1/24  <b>-> ICMP Echo Request analysis </b>
     * nmap -PU 192.168.0.1/24  <b>-> UDP analysis </b>
     * nmap -PR 192.168.0.1/24  <b>-> ARP Ping analysis </b>
     * nmap -traceroute 192.168.0.1/24  <b>->Makes the path analysis of the package </b>
     * nmap -R 192.168.0.1/24  <b>-> Performs hostname exploration from IP address</b>
     * nmap -system-dns 192.168.0.1/24  <b> -> DNS servers in the operating system are used</b>

#### SYN Scan
- Example:
     * nmap -sS 192.168.0.1/24 

#### TCP Scan
- Example:
     * nmap -sT 192.168.0.1/24  

#### UDP Scan
- Example:
     * nmap -sU 192.168.0.1/24  
     
#### Specific Ports
- Exemples:
     * nmap -sS -p80 192.168.0.1/24  <b>-> Scans only the 80 port </b>
     


