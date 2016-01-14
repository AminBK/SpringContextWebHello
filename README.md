# SpringContextWebHello
Spring MVC Hello World with Maven Tomcat7 deploy according to 

http://www.mkyong.com/maven/how-to-create-a-web-application-project-with-maven/


=============
Important step
=============

1) Modify tomcat-users.xml file accordingly

<role rolename="manager-script"/>
<role rolename="manager-gui"/>
<role rolename="manager-jmx"/>
<role rolename="manager-status"/>
<user username="tomcat" password="tomcat" roles="manager-gui,manager-jmx,manager-script,manager-status"/>

2) Environment variables

CATALINA_HOME
C:\apache-tomcat-8.0.12

JAVA_HOME
C:\Program Files\Java\jdk1.7.0_79

JRE_HOME
C:\Program Files\Java\jre7

M2
%M2_HOME%\bin

M2_HOME
C:\apache-maven-3.3.9


3) After compile project run embedded tomcat or deploy

mvn package
mvn eclipse:eclipse
mvn tomcat7:run OR mvn tomcat7:deploy

http://tomcat.apache.org/maven-plugin-2.0/tomcat7-maven-plugin/plugin-info.html


=============
Reminder
=============

git init
git remote add origin https://github.com/verdeairo/SpringContextWebHello.git
git add -A
git commit -m "initial commit"
git push -u origin master
