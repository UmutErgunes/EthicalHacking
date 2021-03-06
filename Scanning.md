## Scanning
We are going to look for 3 things: Ports, Network & Vulnerability.


<b>Port Scan</b>: Used to list open ports and services <br>

<b>Network Scan</b>: Used to list IP addresses.<br>

<b>Vulnerability Scan</b>: Used to discover the presence of known vulnerabilities <br>


## Nmap
<b>Nmap, short for Network Mapper, is a free, open-source tool for vulnerability scanning and network discovery. Network administrators use Nmap to identify what devices are running on their systems, discovering hosts that are available and the services they offer, finding open ports and detecting security risks.</b>
<br>
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

## Legion
<b> Legion is an open source, easy-to-use, super-extensible and semi-automated network penetration testing tool that aids in discovery, reconnaissance and exploitation of information systems. </b>

 ![alt text](https://i1.wp.com/lifars.com/wp-content/uploads/2020/04/LEGION-demo-adding-hosts-and-quick-overview.jpg?resize=720%2C547&ssl=1)


## Nessus
<b> Nessus is the most famous and effective cross-platform vulnerability scanner. It has a Graphical User Interface and is compatible with almost every operating system including Windows, MAC and Unix like Operating systems. </b>

 ![alt text](https://www.tenable.com/sites/all/themes/tenablefourteen/img/nessus/nessus-live-results_large.png)
 
 
 ## Nikto
<b>Nikto is a simple, free and Open Source Scanner which is able to perform scanning for more than 6400 potentials threats and files. It also scans Web Server’s version to check for version related problems. It scans Web Server’s configurations such as HTTP allowed methods, default directories and files. It also supports plugins, proxies, different output formats and multiple scan options.</b>

 ![alt text](https://i.ytimg.com/vi/sN6RU3j6f2g/maxresdefault.jpg)
