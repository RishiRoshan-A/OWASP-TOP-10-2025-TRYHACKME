## OWASP TOP 10 2025

![img](1.png)

The first phase of the Room basic idea of identification , Authentication , Authorization and Accountability 

![img](2.png)


## BROKEN ACCESS CONTROL 

We have a site to test for broken access control lets click on view site 

![img](3.png)

In the url parameter we can notice the id parameter which value is initially 5 

?id=5 

lets change it to 6 and we got another users profile detail 

lets change it to 7 , we found the flag 

![img](4.png)

![img](5.png)

## AUTHENTICATION FAILURES 

We have a site to test for Authentication Failures lets click on view site

![img](6.png)

![img](7.png)

Initially we have given a login page , lets try the default credentials 

username: admin
password: admin 

![img](8.png)

invalid credentials unable to login , lets try to register with username admin

![img](9.png)

we found that admin user exists , lets create a account with 

username : aDmiN  --> this might give us a admin privilege since server might treat admin and aDmiN as same 

![img](10.png)

register andlogn and we got admin privilege as well the flag 

![img](11.png)

## LOGGING & ALERTING FAILURES

![img](12.png)

We have given a SIEM Dashboard to understand Logging and Alerting Failures , click on view site  

![img](13.png)

lets analyze the siem dashboard

![img](14.png)

looks like a attacker trying different combinations of password with username admin to login , 203.0.113.45 is the attacker ip

![img](15.png)

seems like the attacker sussfully loged in as admin with password Password123

![img](16.png)

## CONCLUSION 

This lab demonstrate a basic idea of :

--> Broken Access Control (A:01)
--> Authentication Failures (A:07)
--> security Logging or Monitoring Failures (A:09)

With an pratical example 

