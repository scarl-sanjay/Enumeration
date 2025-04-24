# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion

##dnsenum
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


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT:
# site:example.com
![image](https://github.com/user-attachments/assets/19ba4039-fcd1-47ea-96c0-e2a9a6c6bc83)
# filetype:pdf 
![image](https://github.com/user-attachments/assets/73617bf0-3235-4db9-b2b5-b0899fce25d3)
# intext:password
![image](https://github.com/user-attachments/assets/3bad798f-c6c7-4bc6-883e-424febca269e)
# inurl:admin
![image](https://github.com/user-attachments/assets/c1f530f6-172e-46b9-978b-2ea41262083c)
# intitle:index of
![image](https://github.com/user-attachments/assets/42b11718-6b80-4245-baf5-8488ee8d204e)
# link:example.com
![image](https://github.com/user-attachments/assets/c5db0a95-031e-40ac-84e3-34e589300f4b)
# cache:example.com
![image](https://github.com/user-attachments/assets/65ccc8fb-814d-47df-8fbb-dd17053ae38d)
# DNS Enumeration
# DNS Recon
![image](https://github.com/user-attachments/assets/8770779a-63c0-4d27-af67-5eb7045d2ac6)
# dnsenum
![image](https://github.com/user-attachments/assets/e4838cec-c94b-4835-8739-ed190f12ee95)
# smtp-user-enum
![image](https://github.com/user-attachments/assets/eaafb90a-ac1e-4ff0-bbaf-51d5ce4e6618)
![image](https://github.com/user-attachments/assets/b4d65497-265e-4213-9c54-4a6426156acd)
# Telnet for smtp enumeration
![image](https://github.com/user-attachments/assets/cb2a9d75-fc15-4f8b-b38e-23af661a2448)
# nmap-script smtp-enum-user.nse
![image](https://github.com/user-attachments/assets/8adf4d87-a531-42d2-a9cb-2628fa9fa3cb)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

