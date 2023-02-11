- ![No.Starch-2018-Linux.Basics.For.Aspiring.Hackers.pdf](../assets/No.Starch-2018-Linux.Basics.For.Aspiring.Hackers_1668369134663_0.pdf)
- ((63714b6b-a5da-42cd-a718-7b6198ebec6b))
  collapsed:: true
	- pwd - where you are
	- whoami - returned username or root name
	- cd - change file direction
	- ls - listing contents of directory
	- ls -l - get more info about files and directories
	- ls -al - get more info and hidden files or directory
	- aircrack-ng --help or nmap -h or nmap -? - will display the helpful info about each app
	- man aircrack-ng - manual pages for specific app 
	  we can use PG DN and PG UP keys
	  q - for exit or quit
	- **Finding stuffs**
		- locate - uses database that update only once a day and it can be very overwhelming
		- whereis - return only binaries and man page of specific app
		- which - only return location of binaries in PATH variable in LINUX.
		- find / -type f -name apache2.* 
		  * *find directory options expression*
		  * including, of course, the filename but also the date of creation or modification, 
		  * the owner, the group, permissions, and the size.
	- Filtering with grep
		- allows us to take the output of one command and send it as input to another command.
		  * e.i ps aux | grep apache2
	- cat - display and can create a file for concatenation of a file or created file.
	  * cat > hackingskills - create file and content
	  * cat >> hackingskills - concatenation
	  * cat hacking skills - display content of a file
	- touch file - create a file or edit a file
	  * file to change some of its details, such as the date it was created or modified.
	- mkdir - make a directory
	- cp - copy a file or we can rename a file  and copy the content
	- mv - move a file or rename a file
	- rm - remove a file
	- rmdir - remove a directory 
	  * rm -r - remove directory and all content
	-
	-
	-
	-
	-
		-
	-
- ((638d06af-19dd-4dcf-9333-60fecad1728b))
  collapsed:: true
	- head - view beginning of file 10 lines
	  * head -20 /etc/snort/snort.conf - show lines less or more than 10 lines
	- tail - view last 10 lines of a file
	  * tail -20 /etc/snort/snort.conf - show lines less or more than 10 last lines
	- nl /etc/snort/snort.conf - show the line numbers of content
	  * nl /etc/snort/snort.conf | grep output
	- tail -n+507 /etc/snort/snort.conf | head -n 6
	  * Here, we use tail to start at line 507 and then output into head, and we return just the top six lines, giving us the five lines preceding the Step#6 line, with that line included.
	- sed  - find and replace (stream editor)
		- sed s/mysql/MySQL/g /etc/snort/snort.conf > snort2.conf - replace all
		- sed s/mysql/MySQL/ snort.conf > snort2.conf - replace first occurence don't include g
		- sed s/mysql/MySQL/2 snort.conf > snort2.conf - replace second occurence
	- more - display first page press ENTER for viewing more
	- less - allow us filter the content
		- / allow us to search content
		- n for next
- ((638d0c36-e630-4e3b-bdb2-7eadb8795d18))
  collapsed:: true
	- `ifconfig` -
		- ((638e1b9b-7cde-4156-b179-24087e9f73fa))
		- eth0
		  * Ethernet0 first wired connection
		  * Ethernet - type of connection  
		  * follow by Hwaddr 
		  * NIC (network interface card) or MAC (media access control) - global unique address
		- inet - ip adress which is connected to local network.
		  * Bcast - Broad cast address use for send out info to all IPs on the subnet
		  * network mask - determine part of IP addr is connected to local network
		- ((638e1ba8-976c-4f2a-a5c2-9cf84b42416d))
		- lo - loopback address or localhost software address connected to local machine
		- wlan0 - appears only if you have wireless interface or adapter HWaddr have MAC address
	- iwconfig -
	  collapsed:: true
		- Gather wireless info
		  * wlan0 - cable of b,g, and n latest standard
		  * AP - wire less may or may not associated with Access Point devices
		  * 20 dBm - strength of wireless signal
		  * mode - manage mode or promiscuous mode
		- more info likes 
		  * adapter's IP address
		  * MAC address
	- ((638e2c02-e88b-4840-a353-74d7684d2941))
		- spoof you IP  in DoS attack - for avoiding capture during forensic analysic
		- change eth0 IP address
		  ifconfig eth0 192.168.181.115
		- change IP, netmask, broadcast
		  ifconfig eth0 192.168.181.115 netmask 255.255.0.0 broadcast 192.168.1.255
	- Spoofing MAC addr 
	  * MAC addrr use for keep hackers out or trace them
	  * We can Spoof MAC addr
	  * kali >ifconfig eth0 down 
	  * kali >ifconfig eth0 hw ether 00:11:22:33:44:55 
	  * kali >ifconfig eth0 up
	  * will change to spoofed IP addr
	- ((638e4cb0-b787-4936-83cc-b2a75b9761e8))
	- Assigning New IP addr DHCP Server
	  * dhclient eth0 - sends DHCPDISCOVER request from NIC
	  * receive offer from DHCP server
	  * confirms IP assignment to DHCP server with dhcp request
	- ((638e5477-5df4-4431-bacf-4a39d08ca420))
		- DNS or BIND
		- Examining DNS with dig 
		  * DNS translate IP addr to domain name and dig is good for examing
		  * target's nameserver, target's email server, subdomains and IP addr 
		  * dig hackers-arise.com ns
		- Exam email server 
		  * dig hackers-arise.com mx
	- ((638e55d6-5afd-49c1-ae41-40816b4c459b))
		- If we want to use DNS change DNS
		  leafpad /etc/resolv.conf
		- nameserver have the local DNS server and can be change with
		  * change local dns server with google server
		  * echo "nameserver 8.8.8.8"> /etc/resolv.conf
		- renewing DHCP address renew DNS
	- ((638e5794-436d-4b8b-b134-b0dcf0e516c3))
		- hosts file perform domain name IP address translation
		- we can redirect which IP address browser go to
		  * leafpad /etc/hosts
		  * we can add addr like bankof america
		  * good for dnspoof
- ((638e7a9b-22c8-4028-844e-5727b151c52e))
- ((638e7bd3-5ccf-4bef-acde-1a62b0288176))
- ((638e7c1f-1a8d-4c17-9f50-1490442cb87e))
-