# This was part of my cybersecurity course

## the goal is to find vulnerabilities and mistakes on this page :

![Alt text](image.png)

first nmapped to find open ports.

![Alt text](image-1.png)

![Alt text](image-2.png)

Found 5 open ports 

lets scan the web server with nikto.

![Alt text](image-3.png)

found multiple vulnerabilities 

also /backup and /suplier directories

found this in supplier directory :

![Alt text](image-4.png)

M5joeuser/password/platnum/192.168.100.56
M6kroemer/s3Cr3t/gold/10.100.100.1
M7janeuser/waiting4Friday/172.22.12.19
M8kbookout/sendmeapo/10.100.100.20

after decoding from Base64 format

earlier nmap showed us that there is a mysql service, lets try to connect

![Alt text](image-5.png)

no password even :D

![Alt text](image-6.png)

users with hashed passwords

tried to log in with 'or 1=1 or'
and got in as test user
tried admin'/* on log in and got in as admin :D

![Alt text](image-7.png)

on admin meni we can perform different tasks like create backups 

![Alt text](image-8.png)

![Alt text](image-9.png)

lets unhash the admins password now

![Alt text](image-10.png)

lets try to order something 

![Alt text](image-11.png)

lets try to edit the card validation function

![Alt text](image-12.png)

now lets intercept this with purbsuite while we press the order button:

![Alt text](image-13.png)

changed the price from 5000€ to 12,3

![Alt text](image-14.png)

