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
![image](https://github.com/AasrithSairam/Enumeration/assets/139331438/1cde1c65-b407-4717-8709-8efb60aa87d1)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
![image](https://github.com/AasrithSairam/Enumeration/assets/139331438/598ee7d0-7489-4ce2-87b3-51c8f4db9cd9)



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![image](https://github.com/AasrithSairam/Enumeration/assets/139331438/e513d2d1-2795-4f92-a49d-f8420944aed2)


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![image](https://github.com/AasrithSairam/Enumeration/assets/139331438/562a3718-9183-4eaa-9c8a-9ba8b89da114)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![image](https://github.com/AasrithSairam/Enumeration/assets/139331438/5f475ae2-71e1-496c-8662-ce1f2043e8d9)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![image](https://github.com/AasrithSairam/Enumeration/assets/139331438/32ab7680-339a-42b7-8ea1-6aefbfa103ef)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![image](https://github.com/AasrithSairam/Enumeration/assets/139331438/755e596e-3683-4971-b4c9-76e695b49a01)

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![image](https://github.com/AasrithSairam/Enumeration/assets/139331438/12e3696d-b4ce-41a0-b9e4-b41c02d7f714)






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
![image](https://github.com/AasrithSairam/Enumeration/assets/139331438/20b01ba9-87cb-436f-a1f7-97701151ea22)


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
![image](https://github.com/AasrithSairam/Enumeration/assets/139331438/b3031c33-89d3-445b-89ab-ade955dfa207)

select any username in the first column of the above file and check the same
![image](https://github.com/AasrithSairam/Enumeration/assets/139331438/bfca1263-569a-4115-be65-e54c3a6a63e8)


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
  ![image](https://github.com/AasrithSairam/Enumeration/assets/139331438/9feccdec-2d60-477c-834e-abbcf6c2a7f1)

  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
![image](https://github.com/AasrithSairam/Enumeration/assets/139331438/162ebffd-4871-41f9-91d4-528252e21331)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

