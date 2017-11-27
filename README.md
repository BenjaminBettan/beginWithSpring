# beginWithSpringMVC

The aim of Spring is to serialize your beans if needed. 
Spring handle the lifecycle of your beans.

Note that the main spring file in your project is : 

src/main/webapp/WEB-INF/spring-servlet.xml

inside of it : <context:component-scan base-package="packagelevel_0.packagelevel_1.packagelevel_2" />

So if you want that Spring handle the instantation of your beans, they should be here :

src.main.java.packagelevel_0.packagelevel_1.packagelevel_2.packagelevel_3.MyBeanEntity.java





##########################################################################

                  PIVOTAL TC SERVER DEVELOPER EDITION

##########################################################################



Download server by searching this on google -> pivotal tc server developer download

Or use this URL : https://network.pivotal.io/products/pivotal-tcserver

And select : Pivotal tc Server Developer Edition (For me, version : 3.2.8)





##########################################################################

WINDOWS INSTALLATION AND USAGE

##########################################################################

unzip archive

open admin terminal

go to your directory

tcruntime-instance.bat create myserver 

cd myserver\bin

tcruntime-ctl.bat install
tcruntime-ctl.bat restart

logs of your server are here :

logs\catalina.out

Control your server with 

tcruntime-ctl.bat restart
tcruntime-ctl.bat stop
tcruntime-ctl.bat start

Put your war files in webapps. The server will unzip it and start it. Stop server if you want to delete files and folders in this directory.

##########################################################################

LINUX INSTALLATION AND USAGE

##########################################################################

Note : for every sh command, do first : sudo chmod 777 yourShFile

unzip archive

open terminal (don't use sudo unless you have to)

go to your directory

sh ./tcruntime-instance.sh create myserver 

cd myserver\bin

sh ./tcruntime-ctl.sh install
sh ./tcruntime-ctl.sh restart


logs of your server are here :

logs\catalina.out

Control your server with 

sh ./tcruntime-ctl.sh restart
sh ./tcruntime-ctl.sh stop
sh ./tcruntime-ctl.sh start

Put your war files in webapps. The server will unzip it and start it. Stop server if you want to delete files and folders in this directory.



##########################################################################

                              ECLIPSE STS
                              
##########################################################################



Download Eclipse STS (spring tool suite) by searching in google : spring sts download

or download here : https://spring.io/tools/sts/all

Spring boot : instead of doing " new > new Java Project / new Maven project" as usual, do instead " new > new spring starter project "

you should see this : http://www.bogotobogo.com/Java/tutorials/images/Spring-Boot/Tomcat-War/Spring-Starter-Project-WebCheckBox.png


It will create a maven project with basic dependencies for this kind of project



