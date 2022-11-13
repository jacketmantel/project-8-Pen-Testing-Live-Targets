
# Pen Testing Live Targets

Time spent: 3 hours spent in total

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

Vulnerability #1: SQL INJECTION

Description:
Vul #1: SQL injection takes place by replacing the id value associated with a salesperson with a ' OR SLEEP(5)=0--'. The Blue page takes 5 seconds to reload while the Green and Red pages are immediate.




![chrome_R20FX3zLW3](https://user-images.githubusercontent.com/112223148/201550086-4d1ad216-ebc8-4c1f-92c7-51f2e143d8ed.gif)
"


## Green


Vulnerability #1: Cross-Site Scripting

Description:
Entering the name <script>alert('James found the XSS!');</script> in the contact/feedback form will execute the script when the staff views the feedback. As you can see, a previous student added a script to redirect to Google so my script will not be able to run.

![chrome_cil9I24yTn](https://user-images.githubusercontent.com/112223148/201550213-3890c322-ea44-47be-bcce-78208915e90e.gif)



## Red

Vulnerability #1: Insecure Direct Object Reference
Description:
The error that the developer made is that he allowed for a hacker to input another id value at the top of the url. Id value 10 returns "Testy McTesterson".



![chrome_kEAG6Spnb7](https://user-images.githubusercontent.com/112223148/201550176-f739c178-9590-471a-b28f-fb1ef82565cd.gif)



## Notes

Describe any challenges encountered while doing the work
