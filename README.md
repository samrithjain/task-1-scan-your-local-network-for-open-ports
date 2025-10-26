# scan-your-local-network-for-open-ports-
cyber security internship at elevate labs
## Task-1-Open-Port-Scanning 
cyber security internship 
## install Nmap
we install nmap from official website (or) used nmap for kali linux virtual machine 
## Finding IP range
Normal to finding we used ipconfig in windows and ifconfig in linux.Now we know your ipaddress eg:192.168.1.0/24 (or) 10.128.129.0/24.It means we using class C ip range.The C class is for first three bytes for constant and four byte is changing. [1 byte = 8 bit] [1 bit = 0(or)1] [0/24 means first three bytes are fulled.] Form knowing ip address is ifcongig in kali linux. Now we know ipaddress. ip address : 10.128. . 
## Nmap 
Nmap stands for Network Mapper.
It’s a powerful open-source tool used by hackers, penetration testers, and security analysts to discover and analyze devices connected to a network.
You can think of Nmap as the “radar” of a hacker — it scans networks to see:
1.which devices (computers, routers, phones, servers) are online
2.which ports are open (e.g., 22 for SSH, 80 for HTTP)
3.which services and versions are running
4.even what operating system a target might be using
## Nmap using our ip address 
n nmap there so many scans are avaliable.But we using -sS for TCP SYN scan it for knowing open ports in system. It display opens ports with services is running with them. I used this command to google.we all know that ipaddress is 8.8.8.8.
nmap -sS 8.8.8.8
result: open ports are 53 is domain. 433 is https.
## Wireshark
It captures and shows every single packet (the small chunks of data) that travels through your system — whether it’s a website you open, a login request, or a file being downloaded.
## open ports with services 
Open ports with services means one service is have port number. Example : HTTPS is 433 DNS is 53 HTTP is 80 FTP is 20/21 SMTP is 25 SSH is 22
## security risks from open ports
Open ports are network entry points that allow communication between a device and the internet. Each port corresponds to a specific service, such as HTTP (port 80) or SSH (port 22). While some open ports are necessary for normal operations, unused or poorly secured ones can expose a system to serious risks. Hackers can exploit these open ports to gain unauthorized access, perform brute-force attacks, or inject malicious code. They may also use open ports to gather system information or launch denial-of-service (DoS) attacks. Therefore, regularly scanning, securing, and closing unnecessary ports is essential for network safety.
## firewall
In firewall there IDS and TPS for blocking or pervent for scannings.It works like wall between request and receive traffic.Firewall is monitoring and filter traffic of network.
