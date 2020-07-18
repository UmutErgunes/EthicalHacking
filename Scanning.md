## Scanning
We are going to look for 3 things: Ports, Network & Vulnerability.


<b>Port Scan</b>: Method of determining which ports on a network are open and could be receiving or sending data. It is also a process for sending packets to specific ports on a host and analyzing responses to identify vulnerabilities. <br>

<b>Network Scan</b>: Refers to the use of a computer network to gather information regarding computing systems. Network scanning is mainly used for security assessment, system maintenance, and also for performing attacks by hackers.<br>

<b>Vulnerability Scan</b>: Inspection of the potential points of exploit on a computer or network to identify security holes. A vulnerability scan detects and classifies system weaknesses in computers, networks and communications equipment and predicts the effectiveness of countermeasures. <br>


#### Port Scan - Nmap
- Exemples:
     * nmap -sP 192.168.0.1/24  -> Ping analysis performed
     * nmap -PS 192.168.0.1/24  -> TCP - SYN analysis performed
     * nmap -PA 192.168.0.1/24  -> TCP - ACK analysis performed
     * nmap -PE 192.168.0.1/24  -> ICMP Echo Request analysis performed
     * nmap -PU 192.168.0.1/24  -> UDP analysis performed