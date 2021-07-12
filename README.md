#Folloooowing task questions sort


Q: What networking constructs are used to direct traffic to the right application on a server?

A: ports

Q: How many of these are available on any network-enabled computer?

A: 65535

Q: [Research] How many of these are considered "well-known"? (These are the "standard" numbers mentioned in the task)

A: 1024

Q:What is the first switch listed in the help menu for a 'Syn Scan' (more on this later!)?

A:-sS

Q: Which switch would you use for a "UDP scan"?

A: -sU

Q: If you wanted to detect which operating system the target is running on, which switch would you use?

A: -O

Q: Nmap provides a switch to detect the version of the services running on the target. What is this switch?

A: -sV

Q: The default output provided by nmap often does not provide enough information for a pentester. How would you increase the verbosity?

A: -v

Q: Verbosity level one is good, but verbosity level two is better! How would you set the verbosity level to two?
(Note: it's highly advisable to always use at least this option)

A: -vv

Q: What switch would you use to save the nmap results in three major formats?

A: -oA

Q: What switch would you use to save the nmap results in a "normal" format?

A: -oN

Q: A very useful output format: how would you save results in a "grepable" format?

A: -oG

Q: Sometimes the results we're getting just aren't enough. If we don't care about how loud we are, we can enable "aggressive" mode. This is a shorthand switch that activates service detection, operating system detection, a traceroute and common script scanning
.

A: -A

Nmap offers five levels of "timing" template. These are essentially used to increase the speed your scan runs at. Be careful though: higher speeds are noisier, and can incur errors!

Q: How would you set the timing template to level 5?

A: -T5

We can also choose which port(s) to scan.
Q: How would you tell nmap to only scan port 80?

A: -p80

Q: How would you tell nmap to scan ports 1000-1500?

A: -p 1000-1500

A very useful option that should not be ignored:
Q: How would you tell nmap to scan all ports?

A: -p-

Q: How would you activate a script from the nmap scripting library (lots more on this later!)?

A: --script

Q: How would you activate all of the scripts in the "vuln" category?

A: --script==vuln

Q: Which RFC defines the appropriate behaviour for the TCP protocol?

A: RFC 793

Q: If a port is closed, which flag should the server send back to indicate this?

A: RST


Q: There are two other names for a SYN scan, what are they?

A: Half-open,Stealth

Q: Can Nmap use a SYN scan without Sudo permissions (Y/N)?

A: N


Q: Which of the three shown scan types uses the URG flag?

A: xmas

Q:Why are NULL, FIN and Xmas scans generally used?

A: firewall evasion

Q:Which common OS may respond to a NULL, FIN or Xmas scan with a RST for every port?

A: Microsoft Windows

Q: How would you perform a ping sweep on the 172.16.x.x network (Netmask: 255.255.0.0) using Nmap? (CIDR notation)

A: nmap -sn 172.16.0.0/16

Q: What language are NSE scripts written in?

A: lua

Q: Which category of scripts would be a very bad idea to run in a production environment?

A: intrusive

Q: What optional argument can the ftp-anon.nse script take?

A: maxlist

Q: Search for "smb" scripts in the /usr/share/nmap/scripts/ directory using either of the demonstrated methods.
What is the filename of the script which determines the underlying OS of the SMB server?

####Follow these step:####
sudo apt update && sudo apt install nmap
nmap --script-updatedb
simple cd ls find the file location

A: smb-os-discovery.nse

Q: Read through this script. What does it depend on?

A: smb-brute

Q: Which simple (and frequently relied upon) protocol is often blocked, requiring the use of the -Pn switch?

A: ICMP

Q: [Research] Which Nmap switch allows you to append an arbitrary length of random data to the end of packets?

A: --data--length

Q: Does the target (10.10.85.0)respond to ICMP (ping) requests (Y/N)?

A: N

Q: Perform an Xmas scan on the first 999 ports of the target -- how many ports are shown to be open or filtered?

A: 999

Q: There is a reason given for this -- what is it?

A: No response

Q: Note: The answer will be in your scan results. Think carefully about which switches to use -- and read the hint before asking for help!

A: 5

Q: Deploy the ftp-anon script against the box. Can Nmap login successfully to the FTP server on port 21? (Y/N)

A: Y

