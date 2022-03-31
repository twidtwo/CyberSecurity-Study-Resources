# CyberSecurity-Study-Resources
__ALL LINKS IN THE TEXT ARE TO FREE RESOURCES__ (Please add an issue if a resource becomes unavailable or is not free)
# Paid / Free #
  Free content is just as good sometimes better as paid content. You pay for CONVIENCE or a certification 
  # Free platforms
  
   [Tryhackme](https://tryhackme.com/) - Beginner friendly variety of content
   
   [Hacktricks Online Book](https://book.hacktricks.xyz/) - Good book of notes
    
   **Most free content is in blog posts and youtube videos it doesn't belong in this section other links are under specific topics**
    
  # Paid Platforms #
   [Tryhackme](https://www.tryhackme.com) $10 a month - Beginner friendly
   
   [HackTheBox](https://www.hackthebox.com) $10 + a month - Better hacking challenges then tryhackme but less beginner friendly
   
   [PentesterLab](https://pentesterlab.com/) $20 a month - Video walkthroughs more structured learning less googling to fill the gaps Specific badges for topics
# Background 
  The general order of things to learn before security is 
    
    Unix command line -> Basic Networking -> How the web works    -> Windows command line
                                           
                                             Common services         Powershell (get-help & invoke-webrequest is enough for now)
                                             
                                             Basics of python
                                             
 [Presecurity THM Module](https://tryhackme.com/path/outline/presecurity) <- Covers all of these topics 
  ### Unix command line resources
   [Short web book](http://www.ee.surrey.ac.uk/Teaching/Unix/)
   
   [THM linux fundamentals](https://tryhackme.com/module/linux-fundamentals)
  ### Networking resources 
   [THM net fundamentals](https://tryhackme.com/module/network-fundamentals) - functional knowledge you will need to understand things
   
   [Video on OSI Model](https://www.youtube.com/watch?v=vv4y_uOneC0)
   
   [Video on TCP & IP](https://www.youtube.com/watch?v=2QGgEk20RXM)
   
   [Article on Packets & Frames](https://www.baeldung.com/cs/networking-packet-fragment-frame-datagram-segment)
   
   [Video on Packets & Frames](https://www.youtube.com/watch?v=P5jC8D5zndc) - very indepth explanation of packets frames and encapsulation **
   
   [Playlist of Networking videos](https://youtu.be/As6g6IXcVa4) - For Comptia net+ cert has good information and is explained well, skip stuff about configuring an enterprise network unless you find it interesting
  
  ### How the web works
  [THM How the web works](https://tryhackme.com/room/webfundamentals) 
  
  [Video on websites](https://www.youtube.com/watch?v=vcRmKtL4o_4&ab_channel=TechWorldwithNana)
  
  ### Common Services
  **REMEBER TO READ MANUAL ENTRIES FOR COMMANDS USING "_man COMMAND_"**
  **YOU SHOULD KNOW HOW TO USE : **
    
    ssh - remote access to a machine NO GUI also has SFTP  and SCP which allow for secure ftp functions and secure file copying
    
    ftp - server that hosts files and allows for upload (sometimes) and download of files
    
    curl (Windows equivalent is Invoke-webRequest) - command line tool for communicating with webpages 
    
    rdp (xfreerdp on linux) - remote access to a machine through GUI
  #### SSH / SCP
  [ssh Explained in depth](https://wiki.archlinux.org/title/OpenSSH)
  
  [scp Explained in depth](https://wiki.archlinux.org/title/SCP_and_SFTP#General_Usage)
  ### Python Scripting (Intro)
  [Pwntools documentation](https://docs.pwntools.com/en/stable/) - PWNtools is a python library that makes exploit development easier will be referenced later dont't worry about it on your first pass of this document
  
  [Python documentation](https://docs.python.org/3/)
  
  [EdaBit (Website to learn coding languages)](https://edabit.com/challenges/python3) - Good for learning python fast edabit + python docs should get you set up with enough knowledge of python in an hour or two
  
  
  ### Windows Command Line
   [cheatsheet for windows cmd](http://www.cs.columbia.edu/~sedwards/classes/2017/1102-spring/Command%20Prompt%20Cheatsheet.pdf) - cheatsheet on windows commands
   
   [Windows Fundamentals THM Module](https://tryhackme.com/module/windows-fundamentals) - gives basics on using windows cmd line

  # Universal CyberSec tools 
  ### [Vmware Player](https://docs.vmware.com/en/VMware-Workstation-Player/index.html) - type 2 hypervisor free
  #### ISO IMAGE SOURCES
  [Windows <11 developer version](https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/) - [Win 11](https://developer.microsoft.com/en-us/windows/downloads/virtual-machines) 
  
  Linux has too many distros iso files for each hypervisor will usually be posted on that distro's webpage
  
  ### [nmap wiki](https://nmap.org/) - port scanner modular with nse scripting engine used by both blue and red teams, [nessus](https://www.tenable.com/products/nessus) is more in depth better in general for blue teaming
  [quick nmap tutorial](https://youtu.be/IoIsTrKrl-0) 
  
  ### [wireshark](https://www.wireshark.org/) - packet capturing tool
   
   [quick wireshark tutorial](https://youtu.be/TkCSr30UojM)
   
   [wireshark practice THM](https://tryhackme.com/room/overpass) - overpass is a good indication of whether you can use wireshark or not and is one of the best designed rooms on THM, [overpass sequel](https://tryhackme.com/room/overpass2hacked) , [overpass triquel cause its that good](https://tryhackme.com/room/overpass3hosting)
   

  ### ISACs - Information Sharing and Analaysis Center are public platforms that have databases of cybersecurity threats *NOT all of these are techniqually ISACs but same idea*
    
   [Mitre ATT&CK](https://attack.mitre.org/matrices/enterprise/) - Database of attack types
    
   [Exploit DB](https://www.exploit-db.com/) - database of exploits
   
   [NIST](https://www.nist.gov/cybersecurity) - [NVD (NIST exploit db)](https://nvd.nist.gov/)
   
   [SHODAN](https://www.shodan.io/) 
  # REMEMBER if you don't know what something is look it up before continuing reading
  # Basic Cyber Security Hygiene 
    Checksum - A checksum is often posted on an offical release page for a software. It is the output of a hashing algortihm when the file is hashed. If the file you downloaded is the file you meant to then the checksums will match what the release page says.
    
        MD5sum FILE to generate a md5 checksum of FILE on linux 
    
        certutil -hashfile FILE ALGORITHM to generate a ALGORITHM checksum of FILE on windows
    
    Wifi - Use WPA2 or WPA3  others are insecure
    
    Links - 
    
      Don't click suspicious links, at least check them on virusTotal. 
      
      It is safer to avoid clicking links in messages or emails and go to the webpage manually instead.
    
    Web browsing - 
      
      Configure for Least functionality needed to be usuable. 
      
      Disable pop-ups put exceptions for sites that rely on pop-ups. 
      
      Disable js if you can get away with it.
      
      Configure your browser to prevent third party cookies. 
      
      Use strong different varying passwords for accounts. 
 
  # Starting point
    CIA Triad - Cornerstones of infoSec infrastructure has three parts a breach of any of these parts is bad 
      
      Confidentiality - Information hasn't been exposed to unauthorized people 
      
      Integrity - Information has not been modified or altered without proper authorization
      
      Availability - Information is able to be stored, accessed, or protected at all times
      
    Teams - The main three diverging paths in cybersecurity are 
      
      Offensive - hacking to find vulnerabilties in technology
      
      Defensive - Cybersecurity guard and network administrator responsible for keeping data secure and company/organization protected as well as stop threats as they happen
      
      Incident Response - Cybersecurity Detective and police responsible for backtracing what happened during an incidient or responding to an incidient as it happens 
      
*CREATION IN PROGRESS MORE RESOURCES WILL BE ADDED OVER TIME*
