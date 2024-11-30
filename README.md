sudo apt-get install tomacat9
sudo apt-get install tomcat9-admin
cd /etc/tomcat9
sudo nano server.xml
--> port="8100"
--> address="0.0.0.0"
sudo nano tomcat-users.xml
<user username="tomcat" password="tomcat@123" roles="manager-gui,manager-script"/>
sudo systemctl restart tomcat9.service
sudo ufw allow 8100/tcp

on web 
localhost:8100
-->manager web app
provide credentials 
