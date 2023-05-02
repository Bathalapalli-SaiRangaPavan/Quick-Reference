1. ```/opt/tomcat/bin/version.sh```: Display the Tomcat version
2. ```systemctl start tomcat```: Start the Tomcat server
3. ```systemctl stop tomcat```: Stop the Tomcat server
4. ```systemctl restart tomcat```: Restart the Tomcat server
5. ```systemctl status tomcat```: Check the status of Tomcat
6. ```cp app.war /var/lib/tomcat/webapps/```: Deploy a WAR file to Tomcat
7. ```rm -rf /var/lib/tomcat/webapps/app*```: Undeploy a WAR file from Tomcat
8. ```export CATALINA_OPTS="-Xms512m -Xmx1024m"```: Set the Tomcat memory settings
##### Configure Tomcat users and roles in the tomcat-users.xml file.
Step 1 - Open the tomcat-users.xml file for editing 

- vi /opt/tomcat/conf/tomcat-users.xml

Step 2 - Add a new user with a username and password:
`
- ```<user username="myusername" password="mypassword" roles="myrole"/>```

Step 3 - Add a new role

- ```<role rolename="myrole"/>```

Step 4 - Map the role to the user

- ```<user username="myusername" password="mypassword" roles="myrole"/>```

Step 5 - Save and close the tomcat-users.xml file

Step 6 - Restart Tomcat to apply the changes
- ```systemctl restart tomcat```
