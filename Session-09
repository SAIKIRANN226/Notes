Configuring remaining components
---------------------------------
1. Configure all components as per the documentation 
2. Create records for all instances in the route53 and (Public_IP for only web and Private_IP for 
   remaining) and no need to give the sub domain for web instance
3. Dont forget to give all other components IPaddress information in the roboshop.conf in web

All components first hit redis because it is a cache server if the data is not available in redis 
then it will hit to the DB and while configuring redis component we can see bind 127.0.0.1 and 
remove #(uncomment) first then keep "bind 0.0.0.0 ::1" wherever you see bind change it to 0.0.0.0

Steps to install any application in linux
------------------------------------------
1. First we should have server or instance
2. Which ever application like nodejs,.net,java,python etc. any language
3. Install that programming language
4. Create a directory for this and create separate user for that application
5. Download the application, and also install dependencies,
   If nodejs ---> install "npm" dependency
   If java ---> install "maven" dependency
   If python ---> install "pip" dependency
   If .net ---> install "nuget" dependency
   After downloading the code then how to run? for that we have it in .service file 
   "/etc/systemd/system/application.service"
6. Systemctl start application
7. Systemctl enable application

Points to remember
*******************
1. npm will install dependencies and similarly mvn clean package will also install dependencies and 
   give us a jar file
2. If we compile java ---> We get bytecode(jarfile), remaining languages like python,nodejs no need
   to compile it will run directly.
