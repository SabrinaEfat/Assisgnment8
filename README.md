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

Vulnerability #2: SQL Injection(SQLi)=> The blue color site has one place where the input is not being sanitized before used in an SQL query.
![sql injection sqli](https://user-images.githubusercontent.com/42579932/48591739-348b6080-e913-11e8-8166-846c2a2ed8df.gif)

## Green

Vulnerability #1:Cross-Site Scripting(XSS).
![cross-site scripting](https://user-images.githubusercontent.com/42579932/48592108-dc555e00-e914-11e8-9db4-d03b3b5d57f0.gif)


Vulnerability #2: Username Enumeration: It can perform if web application gives hints whether user exists or not.
![username enumeration](https://user-images.githubusercontent.com/42579932/48592182-35bd8d00-e915-11e8-90f7-fa55fb5526b8.gif)


## Red

Vulnerability #1: Insecure Direct Object Reference (IDOR): The red color site is missing code which would prevent some sensitive information from being made public.
![vulnerability 1 insecure direct object reference](https://user-images.githubusercontent.com/42579932/48590376-41a55100-e90d-11e8-8400-d5cc7c3dd108.gif)

Vulnerability #2:Cross-Site Request Forgery (CSRF)=> The red color site does not have CSRF protections on the admin area. A smart hacker could design a form which would automatically submit from data to the staff area and take advantage of a logged in user's acccess permissions.
![vulnerability 2 cross-site request](https://user-images.githubusercontent.com/42579932/48590435-6ef1ff00-e90d-11e8-9d6c-26f98969b2fb.gif)



## Notes

Describe any challenges encountered while doing the work

