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
Following searches for all the sites that is in the domain openai.com


<img width="928" height="1064" alt="Screenshot 2026-02-04 083133" src="https://github.com/user-attachments/assets/ab2a601b-5df3-4ce0-af48-ae9f64dd01de" />


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain openai.com

<img width="940" height="1121" alt="Screenshot 2026-02-04 083216" src="https://github.com/user-attachments/assets/0e61c994-e4ef-4455-9260-bb719ab94029" />


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

<img width="938" height="1015" alt="Screenshot 2026-02-04 083323" src="https://github.com/user-attachments/assets/471c36f8-9bf0-443a-9bb6-f64d78072233" />


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

<img width="934" height="1173" alt="Screenshot 2026-02-04 083356" src="https://github.com/user-attachments/assets/1a42b358-a932-4677-ad13-b3b509ffa014" />

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

<img width="948" height="1107" alt="Screenshot 2026-02-04 083514" src="https://github.com/user-attachments/assets/57364b82-7af1-447b-96bf-0cb14e153035" />


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.


<img width="922" height="1167" alt="Screenshot 2026-02-04 083548" src="https://github.com/user-attachments/assets/d3d9e1a4-d13c-432d-b24a-d0917f15918e" />

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

<img width="938" height="1161" alt="Screenshot 2026-02-04 084128" src="https://github.com/user-attachments/assets/d3c37b55-7774-46ec-ad50-242d57a1cdb8" />

#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:




<img width="920" height="803" alt="Screenshot 2026-02-04 084837" src="https://github.com/user-attachments/assets/005903c6-9953-4724-a52b-74d0653a08cb" />



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

<img width="939" height="798" alt="Screenshot 2026-02-04 085039" src="https://github.com/user-attachments/assets/9764ac6e-5549-4cba-aa09-081c374ffa0a" />


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

<img width="838" height="425" alt="Screenshot 2026-02-04 090937" src="https://github.com/user-attachments/assets/72ab99a3-8096-411f-801e-638523aea5e2" />


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
  
  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

<img width="739" height="288" alt="Screenshot 2026-02-04 091328" src="https://github.com/user-attachments/assets/3f7919c2-3d57-4c59-8b20-ebccce8ba96e" />



## OUTPUT:


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

