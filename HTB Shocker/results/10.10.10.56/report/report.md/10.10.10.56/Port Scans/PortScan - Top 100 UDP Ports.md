```bash
nmap -vv --reason -Pn -T4 -sU -A --top-ports 100 -oN "/root/results/10.10.10.56/scans/_top_100_udp_nmap.txt" -oX "/root/results/10.10.10.56/scans/xml/_top_100_udp_nmap.xml" 10.10.10.56
```

[/root/results/10.10.10.56/scans/_top_100_udp_nmap.txt](file:///root/results/10.10.10.56/scans/_top_100_udp_nmap.txt):

```
# Nmap 7.92 scan initiated Mon Jan 17 17:01:41 2022 as: nmap -vv --reason -Pn -T4 -sU -A --top-ports 100 -oN /root/results/10.10.10.56/scans/_top_100_udp_nmap.txt -oX /root/results/10.10.10.56/scans/xml/_top_100_udp_nmap.xml 10.10.10.56
Warning: 10.10.10.56 giving up on port because retransmission cap hit (6).
Increasing send delay for 10.10.10.56 from 100 to 200 due to 11 out of 11 dropped probes since last increase.
Increasing send delay for 10.10.10.56 from 200 to 400 due to 11 out of 11 dropped probes since last increase.
Increasing send delay for 10.10.10.56 from 400 to 800 due to 11 out of 11 dropped probes since last increase.
Nmap scan report for 10.10.10.56
Host is up, received user-set (0.076s latency).
Scanned at 2022-01-17 17:01:41 EST for 198s
Not shown: 88 closed udp ports (port-unreach)
PORT      STATE         SERVICE       REASON      VERSION
7/udp     open|filtered echo          no-response
19/udp    open|filtered chargen       no-response
49/udp    open|filtered tacacs        no-response
69/udp    open|filtered tftp          no-response
120/udp   open|filtered cfdptkt       no-response
997/udp   open|filtered maitrd        no-response
1030/udp  open|filtered iad1          no-response
1701/udp  open|filtered L2TP          no-response
3456/udp  open|filtered IISrpc-or-vat no-response
30718/udp open|filtered unknown       no-response
32815/udp open|filtered unknown       no-response
65024/udp open|filtered unknown       no-response
Too many fingerprints match this host to give specific OS details
TCP/IP fingerprint:
SCAN(V=7.92%E=4%D=1/17%OT=%CT=%CU=9%PV=Y%DS=2%DC=T%G=N%TM=61E5E80B%P=x86_64-pc-linux-gnu)
SEQ(II=I)
SEQ(CI=I%II=I)
T5(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)
T6(R=Y%DF=Y%T=40%W=0%S=A%A=Z%F=R%O=%RD=0%Q=)
T7(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)
U1(R=Y%DF=N%T=40%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=G%RUD=G)
IE(R=Y%DFI=N%T=40%CD=S)

Network Distance: 2 hops

TRACEROUTE (using port 1900/udp)
HOP RTT      ADDRESS
1   75.65 ms 10.10.14.1
2   76.03 ms 10.10.10.56

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Mon Jan 17 17:04:59 2022 -- 1 IP address (1 host up) scanned in 198.00 seconds

```
