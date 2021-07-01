# **Gathering Information**

**Tools used:**

1. Maltego
2. Nmap
3. Google dorks

**MALTEGO**

Maltego is an open source intelligence (OSINT) and graphical link analysis tool for gathering and connecting information for investigative tasks. So I used maltego to find the information of the page

![](https://github.com/whitedevil1710/GatheringInformation/blob/main/maltego.png)

**Nmap**

Nmap is a tool used for network discovery and security auditing. So let&#39;s find the open ports of metasploitable which is an intentionally vulnerable Ubuntu Linux virtual machine that is designed for testing.

So now we can check the ip that is active.

![](https://github.com/whitedevil1710/GatheringInformation/blob/main/ipfind.png)

So now let&#39;s scan the open ports of the ip we got

![](https://github.com/whitedevil1710/GatheringInformation/blob/main/portscan.png)

So these many are open port of the Ip

Following are the some commands that can be used in Nmap:

nmap 192.168.1.1-Scan a single IP,

nmap 192.168.1.1 192.168.2.1-Scan specific IPs

nmap 192.168.1.1-254-Scan a range

nmap scanme.nmap.org-Scan a domain

nmap 192.168.1.1 -sT- TCP connect port scan

nmap 192.168.1.1 -sU-UDP port scan

nmap 192.168.1.1 -sV, -Attempts to determine the version of the service running on port

nmap 192.168.1.1 -O - Remote OS detection using TCP/IP
stack fingerprinting

**Google Dorks**

Google hacking involves using advanced operators in the Google search engine to locate specific errors of text within search results. Some of the more popular examples are finding specific versions of vulnerable Web applications. A search query with

**intitle:admbook intitle:Fversion filetype:php**

would locate all web pages that have that particular text contained within them.

Robots.txt is a well-known file for search engine optimization and protection against google dorking. It involves the use of robots.txt to disallow everything or specific endpoints (hackers can still search robots.txt for endpoints) which prevents google bots from crawling sensitive endpoints such as admin panels.

![](https://github.com/whitedevil1710/GatheringInformation/blob/main/Screenshot%202021-07-01%20233030.png)

So this will find the login page containing a title plesk.
