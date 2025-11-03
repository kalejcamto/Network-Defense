# Network-Defense
Procedures - CND Certified Network Defender certification study material and labs (Ethical Hacking)

Ethical Hacking for vulnerability assessment and penetration testing in a controlled virtual environment. 

Topics of this Big Project  I executed using virtual labs and lectures. I am adding screenshots or most important info for some of them: 

>1. Ethics and legal issues
>2. Footprinting
>3. Scanning
>4. Enumeration
>5. System hacking
>6. Trojans and backdoors
>7. Sniffers
>8. Denial of Service
>9. Social Engineering
>10. Session hijacking
>11. Hacking web servers
>12. WEb application vulneratibilities
>13. Web-based password-cracking techniques
>14. Structured Query Language SQL injection
>15. Kacking wireless networks
>16. Viruses and worms
>17. Physical security
>18. Hacking Linux
>19. IDSs, firewalls and honeypots
>20. Buffer overflows
>21. Cryptography
>22. Penetration-testing methodologies


For network defense: 

Here are the primary first steps of network defense:

1. Establish a Security Baseline & Inventory: Asset Discovery, Software Inventory, Configuration Baseline.
2. Network Segmentation and Access Control: Segmentation,Perimeter Defense IPS, Least Privilege, Zero Trust.
3. Patching and Vulnerability Management: Vulnerability Scanning.
4. Visibility and Monitoring Setup: Logging, SIEM.

## LABS: 
  **1. LEGAL**
  
>*USA LEGAL tools*: The Open Organisation of Lockpickers (TOOOL) <https://toool.us/laws/html>
  
>*Costa Rica LEGAL tools*: Procuraduria General de la Republica de Costa Rica <https://www.pgr.go.cr/servicios/sinalevi/>
     Ministerio de Ciencia, Innovación, Tecnología y Telecomunicaciones (MICITT): Es la entidad gubernamental encargada de la rectoría en materia de ciberseguridad y alberga el CSIRT-CR (Centro Nacional de Respuesta a Incidentes de Seguridad Informática) y el SOC-CR.
     Ley de Protección de la Persona frente al Tratamiento de sus Datos Personales (Ley N° 8968): Esta ley regula cómo se deben tratar y proteger los datos personales.
     La Ley N° 9048 reformó el Título VII del Código Penal, Sección VIII (Delitos Informáticos y Conexos)

  **2. Footprinting**
Competitive Intelligence: Business have been doing this for years legally.
Footprinting tools also known as passive reconnaissance tools:

1. Analyze Company's Website <https://sourceforge.net/projects/metasploitable/files/Metasploitable2/>
for Security tests with company's permission use <https://www.zaproxy.org/> **Zed** Attack Proxy for Linux, MacOS and Win, ZAP is an HTTP proxy that processes HTTP requests between the browser and the user. You can gather information about a company's website and discover existing vulnerabilities. Usually start the security test with this.

2. Whois utility is a common web tool for gathering IP address and domain information. <https://whois.domaintools.com/>
Central Ops Net <https://centralops.net/co/domaindossier.aspx>
Many domains reduce the amount of info revealed to help improve security.

3. This is the most basic HTTP method: OPTIONS / HTTP/1.1 on Kalilinux terminal. (type on the browser nc www.gloogle.com 80 and press enter twice. Then go to the terminal and type: wget www.google.com and press enter. This command downloads the index page on your computer in HTML code.
4. Other methods to gather information is detecting cookies and web bugs. Some cookies can cause security issues because people might store personal information in cookies that can be used to attack a computer or server. Other cookies store sensitive data like credentials unencrypted.


  **3. Scanning**
DNS mapeo: 
Step	Proposed Tool	Description of Use
1.1 Passive Reconnaissance	Documentation/Log Review	Review existing documentation (if available and approved) like network diagrams or DHCP logs to obtain an initial list of DNS IPs.
1.2 Port Scanning	Nmap (Open-source port scanner)	Conduct a minimally intrusive scan to search for hosts responding on standard DNS ports: Port 53 (TCP/UDP). This will confirm which systems are running the DNS service.
1.3 Network Tracing	Wireshark (Protocol analyzer)	Monitor internal network traffic to identify the IP addresses that workstations query for name resolution, revealing the primary DNS servers in use.

 MyLanViewer to monitor Devices on your wifi subnet:
<img width="1024" height="768" alt="image" src="https://github.com/user-attachments/assets/11c99667-3439-463f-9b18-3aa696c6dade" />

Run this msf5 command: scanner/portscan/syn in lx terminal.


  **4. Enumeration**
I performed enumeration as well as enumaration prevention on my virtual labs: 

I was able to: Use SuperScan for NetBIOS Enumeration
Use Hyena for Enumeration
Perform LDAP Enumeration using Softerra LDAP Administrator
Perform SNMP Enumeration using IP Network Browser
Perform DNS Enumeration
Perform Windows Host Enumeration using Rpcclient
Perform Linux Host Enumeration using Nmap
Perform Website Enumeration using Nmap
Perform Server Message Block (SMB) Enumeration
Prevent Web Applications Enumeration
Prevent SNMP Enumeration
Prevent LDAP Enumeration
Prevent DNS Enumeration
Prevent Windows Enumeration

Exercise 1 - Exploiting the Webserver Vulnerabilities
Exercise 2 - Preventing Webserver Exploitations

Perform a Slowloris Attack on a Webserver
<img width="1024" height="768" alt="image" src="https://github.com/user-attachments/assets/71f3a0aa-ffe2-4891-89e6-ff3983fa4c6e" />

Enumerate a Webserver using HTTPrint
Perform Directory Traversal Attack
Perform Web Application Brute Forcing Using DirBuster
Use Skipfish to Perform Webserver Reconnaissance
Find Files on a Webserver using Metasploit Framework
Scan for Options on a Webserver using Metasploit Framework
Find the Webserver Version using Metasploit Framework
Check for WebDAV on a Webserver using Metasploit Framework
Use Common Methods to Prevent Webserver Exploitation
Disable HTTP TRACK and TRACE Verbs in Internet Information Services (IIS)

 
   **5. System Hacking**

 Hydra - KaliLinux terminal root
<https://github.com/vanhauser-thc/thc-hydra>
<img width="1024" height="768" alt="image" src="https://github.com/user-attachments/assets/5f8ecfd7-083a-4017-a76d-502fbd4b3f9c" />

Cain - Windows Server
<img width="1280" height="800" alt="image" src="https://github.com/user-attachments/assets/86d1ed2d-9d87-4ad0-b2c3-54e7d828984b" />

  **6.Trojans and backdoors**





  

   **7. Sniffing** 
 
 *Sniff-O-Matic*
<img width="1280" height="800" alt="image" src="https://github.com/user-attachments/assets/4194a1bc-bb8b-4c89-8247-6c8005a4eaa2" />

*XArp*
<img width="1024" height="768" alt="image" src="https://github.com/user-attachments/assets/07f88493-3d0f-4723-a186-c4498fcbd120" />

*KaliLinux: TCP SYNFLOOD metasploit v5.0.73-dev*
mfs5 auxiliary/dos/tcp/synflood

<img width="1024" height="768" alt="image" src="https://github.com/user-attachments/assets/387230e8-5805-4612-8cf2-3ffcb7a72c41" />

*DNS Zone Transfer*
This can be done with *dig* command, goes deeper than *nslookup*
First, determine the primary DNS server. KaliLunux command line: dig ns zonetranfer.me
<img width="576" height="384" alt="image" src="https://github.com/user-attachments/assets/9bd2752d-995c-464a-9eec-c0cf4caddcdf" />

  **8. Denial of Service**

  
  **9. Social Engineering**
Social engineers use many techniques in their atttempts to gain information from unsuspecting people
Urgency, Quid pro quo "I can make your life better if you give me info I need", Status quo "Everyone else is doing it so you should", 
Kindness, Position, shoulder surfing to watch what the user does to steal information as they press buttons or pins or reading something. Dumpster Diving: searching on trash, Piggybacking: access a restricted area by following someone with authorization. Phishing: fake email or links, Spear phising. Some security consulting companies incorporate spear phishin attacks as part of their testing, using tools that can inject shell code nto Adobe PDF files. One exaple of these tools is Metasploit, which is included in Kali Linux. Email authentication technologies such as Sender Policy Framework, DomainKeys Identified Mail, S/MIME, and PGP, as well as security awareness training for users and constant vigilance help reduce the threat of phishing and spear phishing.
Visit <https://wwwphishtank.com> if you suspect phishes to verify the sender.



