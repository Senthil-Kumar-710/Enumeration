# Enumeration
Enumeration Techniques

# Explore Google Hacking and Enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows

### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

## Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:yahoo.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
## Output:

![1](https://github.com/Senthil-Kumar-710/Enumeration/assets/93860256/67d1bb74-d519-4992-a780-c250e32a5f11)




filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

## Output:

![2](https://github.com/Senthil-Kumar-710/Enumeration/assets/93860256/1a946332-b3e1-4e4a-8aec-216dbb357c54)



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.


## Output:

![3](https://github.com/Senthil-Kumar-710/Enumeration/assets/93860256/dcb53a4d-3c16-4797-bbad-4a3166d59089)



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.


## Output:

![4](https://github.com/Senthil-Kumar-710/Enumeration/assets/93860256/8caeaff2-c255-412f-a60d-c813dec68339)



intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.


## Output:

![5](https://github.com/Senthil-Kumar-710/Enumeration/assets/93860256/a0dfd8a5-3a0d-4cac-a649-646bfa5234ae)



link: This operator allows you to search for pages that link to a specific URL. For example, "link:amazon.in" would search for pages that link to the example.com domain.


## Output:

![6](https://github.com/Senthil-Kumar-710/Enumeration/assets/93860256/c3efd1ae-05eb-4c3c-905c-3ed682e478bd)




cache: This operator allows you to view the cached version of a page. For example, "cache:amazon.in" would show the cached version of the example.com website.


## Output:

![7](https://github.com/Senthil-Kumar-710/Enumeration/assets/93860256/9bec8783-843e-4dd1-83d6-78325ef0db45)



 
## DNS Enumeration

DNS Recon
Provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion

## Output:

![image](https://github.com/Senthil-Kumar-710/Enumeration/assets/93860256/cb31b378-3e73-41ac-b8bc-118201acac79)



![image](https://github.com/Senthil-Kumar-710/Enumeration/assets/93860256/9c26e4b4-271d-48a5-a4d3-18b6574b7dcb)




## dnsenum

Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.


## Output:

![image](https://github.com/Senthil-Kumar-710/Enumeration/assets/93860256/99591c96-6662-45b8-b080-84f1942db996)



## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

## Output:

![image](https://github.com/Senthil-Kumar-710/Enumeration/assets/93860256/02b18009-ff3d-4d1b-83b9-dca67e8fa9df)



In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

![image](https://github.com/Senthil-Kumar-710/Enumeration/assets/93860256/65f3df74-70fc-4f32-a003-259eb6884157)



Select any username in the first column of the above file and check the same

![image](https://github.com/Senthil-Kumar-710/Enumeration/assets/93860256/cc6837e1-c5ec-477a-b53a-14942ad74c8d)



  
## nmap --script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## Output:

![image](https://github.com/Senthil-Kumar-710/Enumeration/assets/93860256/f4a07c04-af5e-4d82-b6c1-9c0983222206)




## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully
