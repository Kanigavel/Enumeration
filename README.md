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
Following searches for all the sites that is in the domain tesla.com



![Screenshot 2025-03-15 205913](https://github.com/user-attachments/assets/cae5f81d-17d1-4d78-b7f1-df2c63306d44)




filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain tesla.com



![Screenshot 2025-03-15 205924](https://github.com/user-attachments/assets/971a4af6-0bb0-4823-a820-28db85dfeed9)




intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.




![Screenshot 2025-03-15 205937](https://github.com/user-attachments/assets/fbf47654-89ee-41f3-825e-bee0307c6a0d)





inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.




![Screenshot 2025-03-15 205952](https://github.com/user-attachments/assets/15371adc-3c8a-4106-8a87-08a4b2dd1aa3)




intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.




![Screenshot 2025-03-15 210004](https://github.com/user-attachments/assets/efe5cd93-5bc0-4650-8ba9-a8dcfcec637d)




link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the tesla.com domain.





![Screenshot 2025-03-15 210018](https://github.com/user-attachments/assets/7314d51b-8b20-4610-aa0a-a481c2dd7b95)

![Screenshot 2025-03-15 210052](https://github.com/user-attachments/assets/6efb6766-8a3c-4da5-ae9e-4289e95662da)



cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the tesla.com website.



 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![Screenshot 2025-03-14 171321](https://github.com/user-attachments/assets/76acd299-0617-44c7-aec7-04176a251ced)

![Screenshot 2025-03-14 171333](https://github.com/user-attachments/assets/4bb7ed11-a7ec-4517-a3ae-6605ee57669b)






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

![Screenshot 2025-03-14 171711](https://github.com/user-attachments/assets/b048467f-84e6-42e5-b0f8-c7934054d5f2)



##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![Screenshot 2025-03-14 171738](https://github.com/user-attachments/assets/50f89803-32d8-40b1-b4ca-053eaafe7666)


select any username in the first column of the above file and check the same
![Screenshot 2025-03-14 171724](https://github.com/user-attachments/assets/f46013e1-f1ff-4c4b-86b2-2076d5b63d81)



#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
  ![Screenshot 2025-03-14 172327](https://github.com/user-attachments/assets/3429914e-bf18-4b0c-bee9-4cdafe1ed879)
![Screenshot 2025-03-15 204123](https://github.com/user-attachments/assets/ff27922d-6560-4dac-8193-9379f7a97512)
![Screenshot 2025-03-14 205807](https://github.com/user-attachments/assets/fe400755-2746-4d28-aa5a-066d07c12f2d)


## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT:
![Screenshot 2025-03-14 205807](https://github.com/user-attachments/assets/3140ac46-12a6-4dff-8c8d-498ab477e06a)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

