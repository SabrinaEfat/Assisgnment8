Time spent: 7 hours 

Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.
The six possible exploits are:

1.Username Enumeration
2.Insecure Direct Object Reference (IDOR)
3.SQL Injection (SQLi)
4.Cross-Site Scripting (XSS)
5.Cross-Site Request Forgery (CSRF)
6.Session Hijacking/Fixation

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)
## Blue

Vulnerability #1:Session Hijacking/Fixation: 
I can bypass the login by using another browser session ID, which can lead to steal users information.
![blue](https://user-images.githubusercontent.com/42579932/48589990-e58dfd00-e90b-11e8-8273-c5fbf733a6b8.gif)

Vulnerability #2: SQL Injection(SQLi)=> First Select the Salesperson section, there is "?id=some number" at the end of the url, by entering a ' after some number (number can be from 1 to 9), the blue section will show "Database query failed" while the green and red sections just redirect resulting the blue section has SQLI vulnerability. I used ?id=' OR 1=1'-- etc to testify it.
![blue](https://github.com/SabrinaEfat/Assisgnment8/blob/master/sql.gif)

## Green

Vulnerability #1:Cross-Site Scripting(XSS).
![cross-site scripting](https://user-images.githubusercontent.com/42579932/48592108-dc555e00-e914-11e8-9db4-d03b3b5d57f0.gif)


Vulnerability #2: Username Enumeration:By loggin using a wrong username, the alert message is in plain text. But loggin using a correct username, the alert message appeared is bold. By inspecting the page, we could found that class is "failure" for correct username. The other class is "failed" for uncorrect username.

## Red

Vulnerability #1: Insecure Direct Object Reference (IDOR): By setting the number to be 10 or 11 will give two people that can't be found in Find a Salesperson section. But in blue or green site, when you enter id=10 or id=11, then it will go back to Find a Salesperson page.
Vulnerability #2:Cross-Site Request Forgery (CSRF)=> By trying to edit the information after changing the value of csrdf_token, red section is still able to make a change, while the other two sections show "Error: invalid request" after I changed its csrf_token.





## Notes

Describe any challenges encountered while doing the work

