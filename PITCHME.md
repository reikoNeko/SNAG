# SECURITY IS NOT A GAME
# THE GAME

## from Tron to DefCon in 45 minutes

---

### Let's say it started with TRON

<img src="images/discs_of_tron_cabinet.png" height="400" align="right" alt="Discs of Tron video game cabinet">

In the movie and the game, Flynn encodes a disk with the data he needs to bypass the Master Control Program and has to find a way to exfiltrate it.

This is basically done by throwing a frisbee. We never get to see how the sausage is made.


---
### Push Button, Get Hack

This abstraction continued through thirty years of cyberpunk games from Neuromancer (1988) through the Deus Ex series including the latest release, Mankind Divided.

<img src="images/neuromancer_hacking.jpg" height="200" align="left" alt="Neuromancer hack screen">
<img src="images/dx_divided_camera_takeover.jpg" height="200" align="right" alt="Security Camera hack in Deus Ex">


---
### Moar Please

* More recently, hacking games like Hacknet, Hack'n'Slash, Else Heart.Break(), and Exapunks, have focused on actually chaging code within the game
---
#### Hack'n'Slash
* Zelda-like adventure where your sword is a USB device. Anything with a port can be tweaked.
* Adjust variables to change object behaviors.

<img src="images/hack_n_slash_turtle_spawner.jpg" height="300" align="center" alt="Flipped turtles can be programmed.">


---
#### Hacknet
* Story-driven through email, simplified penetration testing
* Uses some actual Linux/DOS commands (ls|dir, man, scp)  and scripts like SSHcrack

---
#### Else Heart.Break()
* Acquire a Modifier and change the code of street lights, network junctions, even beer!
* In-game language called Språk has developed a small community on github.
* Story progression is weak but the programming options are not.

<img src="images/Else_HeartBreak_hotel_code.png" height="300" align="center" alt="The hotel computer's source">


---
#### Zachtronics games
* Three different programming games that use assembly: TIS-100, Shenzhen I/O, and EXAPUNKS
* In Steam versions, your solutions are ranked against other players'.
---
#### Exapunks
* In Exapunks you solve problems by programming robotic agents that have IPC. (They look a lot like the gridbugs from TRON.)

<img src="images/exapunks_phage_hack.jpg" height="300" align="center" alt="Programming gridbots">


---
### Capture the Flag Games
* System administration and penetration skills
* This isn't Project Euler
* Find flags, score points
* Many have prizes

---
### CTFs use multiple skillsets
* Command line tools 
* Web scraping
* Steganography
* Exploiting CVEs
@color[rgba(44,00,00,0.2)](SNAG{"Do you see me, Red?"})

---
### Ybj unatvat sehvg
Introductory puzzles usually have base64 and rot13 somewhere
```
    In [7]: import codecs
    In [8]: codecs.decode('Ybj unatvat sehvg', 'rot_13')
    Out[8]: 'Low hanging fruit'
```
* Have perl, ipython or Jupyter notebooks handy!

---
### One team, two team, red team, blue team
* The Red Team attacks systems. Many CTFs are only about exercising Red Team skills.
* The Blue Team defends systems. Most system administration jobs are only about exercising Blue Team skills.

---
#### Online CTFs
* Great place to build skills
* Often have internal chat systems or comunity boards
* Play anywhere any time
* Usually stay available after the scoring period ends

---
#### Microcorruption
* More programming than system adminstration
* Binary disassembly challenge!
* If you loved Zachtronics games, this is the place to be.
* Watch what happens when you overflow a buffer.

https://microcorruption.com

---
#### OWASP Juice Shop
* Deliberately subjectable to web attacks
* Based on Open Web Application Security Project top 10 vulnerabilities
* Source available on Github
* Attack by hand or use it to learn Kali|Parrot|ArchStrike

https://juice-shop.herokuapp.com

@color[rgba(44,00,00,0.2)](SNAG{"Shiny! Let's be bad guys!"})

---
#### SANS Holiday Hack
* Sponsored by SANS Institute (who also do expensive training and live CTFs)
* Annual Xmas-themed competition dating back to 2015
* Have problems that use recent or famous bugs
* Watch blogs at sans.org and major CVEs to get a head start
* Reports are a major requirement

https://holidayhackchallenge.com

$ t-shirts, admission to online classes

---
#### More online stuff
* Smash the Stack: http://smashthestack.org
* Google CTF: https://capturetheflag.withgoogle.com

---
### Try this at home
After getting your feet wet online, you can download virtual machines to test at home.
* DO NOT expose these to your outside network.
* Great way to set up packet capturing|filtering to see what attacks look like
* Attack, defend, attack again, wipe and reinstall
* Require VirtualBox, KVM, or VMWare Player

---
#### Damn Vulnerable Linux
* One of the first deliberately insecure releases
* Discontinued ten years ago and based on slackware, for true horror fans.

---
#### Metasploitable
* Testbed for the Metasploit framework
* Free resources from the folks who make Kali

https://www.offensive-security.com/metasploit-unleashed/requirements/

---
#### OWASP BWA
* Broken Web Appications, the precursor to Juice Shop
* Still available as a VM

https://www.owasp.org/index.php/OWASP_Broken_Web_Applications_Project

---
#### VulnHub
* Many, MANY more deliberately insecure virtual machines

---
### Come up to the lab
* Old hardware is great! 
* Don't throw away that insecure D-Link router, use it to make a quarantined network!
* I have a cheap $200 laptop just for running Kali.

Dumpster diving ain't what it used to be, but there are always Raspberry Pis

---
#### RasPwn
* Virtual network of insecure machines running on a single Pi.
* Supports RPi 2 or 3B (not 3B+ or 3A+)
```
    Bind (192.168.99.1, 192.168.99.10) - DNS Server
    Postfix (192.168.99.18) - Mail Transfer Agent
    Dovecot (192.168.99.18) - Mail Client Server
    Samba (192.168.99.10) - Windows File Sharing Server
    Apache2 (192.168.99.13) - Web Server
    Nginx (192.168.99.7) - Web Server
    MySQL Server (127.0.0.1) - Database Server
    OpenSSH (92.168.99.1) - SSH server
```

https://raspwn.org

---
#### Sticky Fingers
* Damn Vulnerable Linux updated to run on the Raspberry Pi
* Includes suppport for touchscreens
* Also have a Pi build of Kali

https://whitedome.com.au/re4son/sticky-fingers-dv-pi/


---
### Hello World!

<img src="images/oreilly_do_it_live.jpg" height="400" align="center" alt="We'll do it live!">


---
Live CTF events happen everywhere, particularly at security conferences and collegiate competitions.

Bring friends or form pick-up teams.

Some feature offense and defense at the same time.

Fabulous(?) prizes!

---
#### BSides
* Regional information security conferences
* Free or cheap events held all over the country
* Some feature multiple CTF and wireless hacking events.
* Another great place to pitch talks!


* Newark, DE, November 8-9
* Philadelphia, probably February 2020
* Baltimore, April 4-5, 2020

https://www.securitybsides.com/

---
#### WOPR Summit
* New conference. 
* 0x00 March 2019 in Atlantic City included a hardware hack space
* 0x01 March 2020 in Fort Washington
* Organizer is a CTF writer

https://www.woprsummit.org/

---
#### CyberSEED
* Collegiate competition at UConn
* Coming up October 19
* Top team prize $15,000

https://ash.engr.uconn.edu/grav/

---
#### DefCon
<img src="images/HolyGrail086.jpg" height="200" align="right" alt="Our beacon, it's grail shaped.">
* Online team qualifiers
* Finals held live at Defcon
* 2019 results up soon at https://www.oooverflow.io/dc-ctf-2019-finals/

---
### More Resources
* https://www.cyberstudents.org/blog-post/build-your-own-lab/
* https://CTFTime.org
* http://www.wechall.net/
* http://www.cis.syr.edu/~wedu/seed/all_labs.html
* https://www.vulnhub.com/resources/
* LiveOverflow's video introduction to CTFs:<br> https://www.youtube.com/watch?v=8ev9ZX9J45A
