Configuring all components in this session at a time
-----------------------------------------------------
1. Create instances
2. Create records and update Private IPaddress of the created instances in hosted zones along with 
   subdomain name and ttl 1
3. Dont forget to update in roboshop config_file(reverse proxy configuration)

What is deployment wether it is manual or automation
-----------------------------------------------------
1. Developer will update the code in git and he will push as zip file
2. Download the code
3. Stop the server
4. Remove old code or backup old code
5. Unzip new code
6. Restart the server
7. Testing

Synchronous vs Asynchronous
----------------------------
http and https websites are ---> synchronous communication server should be always up and running, 
if servers not running. we get error code like 400/500. that is called synchronous

Asynchronous
-------------
Servers should 100% up and always running it should not down for that we use asynchronous
Between, Client ---> Messaging broker(messaging queue) ---> Servers
Example:- Whatsapp messaging when other person is offline

Points to remember
*******************
1. T3.medium for mongodb,shipping,mysql. Remaining all t2.small(free tier)
2. Rabitmq is for payment it is used for messaging queue database
3. Always update records, because when you create new instances it will change the IPaddress
