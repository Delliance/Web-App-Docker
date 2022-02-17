# since in this case we not only need a jvm, we also need an application server, we use tomcat
# it includes both the app server and the jvm, here you use tomcat version 10 with version 17 of the jdk
FROM tomcat:10-jdk17

# since we are using tomcat we need to specify the directory where tomcat will use the .war
ADD target/MyWebApp.war /usr/local/tomcat/webapps/MyWebApp.war

# here we are exposing the port where the app is running, so Docker understand that this port must be exposed
EXPOSE 8080

# this is what will be run when the container starts, the catalina script starts the tomcat server
CMD ["catalina.sh", "run"]