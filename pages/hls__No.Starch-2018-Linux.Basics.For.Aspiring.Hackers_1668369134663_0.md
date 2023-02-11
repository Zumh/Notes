file-path:: ../assets/No.Starch-2018-Linux.Basics.For.Aspiring.Hackers_1668369134663_0.pdf

- Basic Commands in Linux
  ls-type:: annotation
  hl-page:: 50
  hl-color:: yellow
  id:: 63714b6b-a5da-42cd-a718-7b6198ebec6b
- TEXT MANIPULATION
  ls-type:: annotation
  hl-page:: 66
  hl-color:: yellow
  id:: 638d06af-19dd-4dcf-9333-60fecad1728b
- head -20 /etc/snort/snort.conf
  ls-type:: annotation
  hl-page:: 68
  hl-color:: yellow
  id:: 638d0731-c22b-480e-b9a9-568a8ba3f8f0
- ls-type:: annotation
  hl-page:: 69
  hl-color:: yellow
  id:: 638d08b0-2f59-4888-b553-c28992be47c9
  >nl /etc/snort/snort.conf
- ls-type:: annotation
  hl-page:: 71
  hl-color:: yellow
  id:: 638d0983-fda7-45cf-a334-c9abeadf5b31
  >tail -n+507 /etc/snort/snort.conf | head -n 6
- Here, we use tail to start at line 507 and then output into head, and we return just the top six lines, giving us the five lines preceding the Step#6 line, with that line included.
  ls-type:: annotation
  hl-page:: 71
  hl-color:: yellow
  id:: 638d09b9-03c3-46fc-b008-266bcc0ad0c7
- ls-type:: annotation
  hl-page:: 72
  hl-color:: yellow
  id:: 638d0a3d-0a00-4fe9-892d-131035483414
  >sed s/mysql/MySQL/g /etc/snort/snort.conf > snort2.conf
- ANALYZING AND MANAGING NETWORKS
  ls-type:: annotation
  hl-page:: 76
  hl-color:: yellow
  id:: 638d0c36-e630-4e3b-bdb2-7eadb8795d18
- [:span]
  ls-type:: annotation
  hl-page:: 76
  hl-color:: yellow
  id:: 638e1b9b-7cde-4156-b179-24087e9f73fa
  hl-type:: area
  hl-stamp:: 1670257563238
- [:span]
  ls-type:: annotation
  hl-page:: 77
  hl-color:: yellow
  id:: 638e1ba8-976c-4f2a-a5c2-9cf84b42416d
  hl-type:: area
  hl-stamp:: 1670257575886
- Changing Your Network Information
  ls-type:: annotation
  hl-page:: 79
  hl-color:: yellow
  id:: 638e2c02-e88b-4840-a353-74d7684d2941
- ifconfig eth0 192.168.181.115
  ls-type:: annotation
  hl-page:: 79
  hl-color:: yellow
  id:: 638e2c7f-1ce8-4412-b98e-eb4d17236d18
- ifconfig eth0 192.168.181.115 netmask 255.255.0.0 broadcast 192.168.1.255
  ls-type:: annotation
  hl-page:: 79
  hl-color:: yellow
  id:: 638e2cb4-eb4c-4eb7-a395-892db83de734
- kali >ifconfig eth0 down kali >ifconfig eth0 hw ether 00:11:22:33:44:55 kali >ifconfig eth0 up
  ls-type:: annotation
  hl-page:: 80
  hl-color:: yellow
  id:: 638e2dcb-7e4d-4980-82f0-8e42d01f9a63
- The DHCP server assigns IP addresses to all the systems on the subnet and keeps log files of which IP address is allocated to which machine at any one time. This makes it a great resource for forensic analysts to trace hackers with after an attack. For that reason, it’s useful to understand how the DHCP server works.
  ls-type:: annotation
  hl-page:: 80
  hl-color:: red
  id:: 638e4cb0-b787-4936-83cc-b2a75b9761e8
- Manipulating the Domain Name System
  ls-type:: annotation
  hl-page:: 81
  hl-color:: red
  id:: 638e5477-5df4-4431-bacf-4a39d08ca420
- dig hackers-arise.com ns
  ls-type:: annotation
  hl-page:: 82
  hl-color:: red
  id:: 638e5492-7f54-494d-921a-630071938f6e
- dig hackers-arise.com mx
  ls-type:: annotation
  hl-page:: 82
  hl-color:: red
  id:: 638e553c-cae5-475c-9ae9-0b6c9e6145f5
- Changing Your DNS Server
  ls-type:: annotation
  hl-page:: 83
  hl-color:: red
  id:: 638e55d6-5afd-49c1-ae41-40816b4c459b
- leafpad /etc/resolv.conf
  ls-type:: annotation
  hl-page:: 83
  hl-color:: red
  id:: 638e55e7-189c-4743-9c0f-33991563f150
- echo "nameserver 8.8.8.8"> /etc/resolv.conf
  ls-type:: annotation
  hl-page:: 84
  hl-color:: red
  id:: 638e566a-b0be-4c46-af03-73b16023a646
- Mapping Your Own IP Addresses
  ls-type:: annotation
  hl-page:: 84
  hl-color:: red
  id:: 638e5794-436d-4b8b-b134-b0dcf0e516c3
- leafpad /etc/hosts
  ls-type:: annotation
  hl-page:: 85
  hl-color:: red
  id:: 638e5807-3df0-41ab-8f75-f047abbd25de
- ADDING AND REMOVING SOFTWARE
  ls-type:: annotation
  hl-page:: 87
  hl-color:: red
  id:: 638e7a9b-22c8-4028-844e-5727b151c52e
- CONTROLLING FILE AND DIRECTORY PERMISSIONS
  ls-type:: annotation
  hl-page:: 99
  hl-color:: red
  id:: 638e7bd3-5ccf-4bef-acde-1a62b0288176
- PROCESS MANAGEMENT
  ls-type:: annotation
  hl-page:: 114
  hl-color:: red
  id:: 638e7c1f-1a8d-4c17-9f50-1490442cb87e