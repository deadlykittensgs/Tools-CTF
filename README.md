# Tools-CTF



Toolbox 




Nmap detailed scan \

Basic Nmap

nmap -sC -sV

Deep nmap 

nmap -sS -sV -sC -p- <ip_address>

-sS (Stealth/SYN scan)
 Sends SYN packets without completing the TCP handshake. It’s faster and stealthier than a full connect scan.


-sV (Version detection)
 Attempts to detect service versions running on open ports (e.g., Apache 2.4.41, OpenSSH 8.2).


-sC (Default scripts)
 Runs Nmap’s default NSE (Nmap Scripting Engine) scripts for common checks (like SSL cert info, HTTP methods, etc.).


-p- (All ports)
 Scans all 65,535 TCP ports instead of just the top 1,000.



Upgrade the shell:

 python3 -c 'import pty; pty.spawn("/bin/bash")


Catch a reverse shell with NC:

 nc -lvnp <port>
Connect to a port with netcat 
nc ip address port



Search for files by name:

 find / -type f -name "user.txt" 2>/dev/null

Search inside files (long):

 grep -rn "user.txt" / 2>/dev/null

Find SUID binaries:

 find / -user root -perm -4000 -exec ls -ldb {} \; 2>/dev/null

See file permissions 

ls -la

Basic enumeration on a rev shell 

whoami

Id

sudo -l 



Learn linPEAS


SSH to connect 


