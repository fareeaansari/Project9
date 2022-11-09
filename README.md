# Project9
# Pen Testing Live Targets

Time spent: 5 hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:

* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each color is vulnerable to only 2 of the 6 possible exploits. First discover which color has the specific vulnerability, then write a short description of how to exploit it, and finally demonstrate it using screenshots compiled into a GIF.

## Blue

Vulnerability #1: SQL Injection

Description: in the ID parameter, i injected a Sql Injection and found the vulnerability
1- I added 'OR SLEEP(5)=0--' and the webpag ewas gone for 5 seconds
2- I added 11' AND SLEEP(5)=0--' And the lazy employee Id was off for 5 seconds and when it was off we found the information.

<img src="blue-vuln1.gif">


## Green

Vulnerability #1:Cross Site Scripting

Description:
In the contact section, i sent a javascript code in the feedback and update it. the script is excuted when admin viewed the feedback.
<script>alert('Hacked')</script>

<img src="green-vuln1.gif">


## Green

Vulnerability #2:User Enumeration

Description:When enterd the wrong username, the message was in bold letters but when it was right and thge password was wrong only then the message was not bold. 
<img src="green-vuln2.gif">


## Red

Vulnerability #1: IDOR

Description: By changing the ID parameter the non visible salesperson information will be visible.

<img src="red-vuln1.gif">


