## Scanning
We are going to look for 3 things: Ports, Network & Vulnerability.


<b>Port Scan</b>: Used to list open ports and services <br>

<b>Network Scan</b>: Used to list IP addresses.<br>

<b>Vulnerability Scan</b>: Used to discover the presence of known vulnerabilities <br>


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
     * nmap -sS -p1-100 192.168.0.1/24  <b>-> Scans the ports between 1 to 100 </b>
     * nmap -sS -p1,55,155 192.168.0.1/24  <b>-> Scans only ports 1, 55 and 155 </b>
     * nmap -sS -p- 192.168.0.1/24  <b>-> Scans all the ports (65535 ports) </b>
     
#### Service and version exploration
- Exemples:
     * nmap -sS -O 192.168.0.1/24  <b>-> Scans the Operating System </b>
     * nmap -sS -A 192.168.0.1/24  <b>-> Scans the Operating System and Version </b>
     
#### Bypass Firewalls
- Exemples:
     * nmap -f 192.168.0.1/24  <b>-> It sends the packages by splitting with the 'Fragroute' technique. </b>
     * nmap -D {spoofif} 192.168.0.1/24  <b>-> Makes Fake Ip Request</b>
     * nmap -spoof-mac {mac} 192.168.0.1/24  <b>-> Makes a Request by changing MAC address</b>

