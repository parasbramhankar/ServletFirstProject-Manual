## ServletFirstProject-Manual

### Setup
--------
	1. Download tomcat--10.1
	2. Set in environment variable ---> system variable
	3. Make new entry 
classpath: C:\Program Files\Apache Software Foundation\Tomcat 10.1\lib\servlet-api.jar
	4. Check for servlet
	5. Open cmd as admin
	6. Javap jakarta.servlet.GenericServlet
	



## How to create war file manually 
--------------------------------------------
D:\Spark2.0\ServletDemo>md WEB-INF

D:\Spark2.0\ServletDemo>cd WEB-INF

D:\Spark2.0\ServletDemo\WEB-INF>md classes

D:\Spark2.0\ServletDemo\WEB-INF>cd classes

D:\Spark2.0\ServletDemo\WEB-INF\classes>start notepad FirstServlet.java

D:\Spark2.0\ServletDemo\WEB-INF\classes>javac FirstServlet.java

D:\Spark2.0\ServletDemo\WEB-INF\classes>cd ..

D:\Spark2.0\ServletDemo\WEB-INF>start notepad web.xml

D:\Spark2.0\ServletDemo\WEB-INF>cd ..

D:\Spark2.0\ServletDemo>jar cvf first.war .
added manifest
adding: WEB-INF/(in = 0) (out= 0)(stored 0%)
adding: WEB-INF/classes/(in = 0) (out= 0)(stored 0%)
adding: WEB-INF/classes/FirstServlet.class(in = 642) (out= 408)(deflated 36%)
adding: WEB-INF/classes/FirstServlet.java(in = 320) (out= 208)(deflated 35%)
adding: WEB-INF/web.xml(in = 232) (out= 104)(deflated 55%)

### How to deploy war in tomcat
----------------------------
	1. start tomcat
	2. click manage 
	3. Select war file
	4. Click on deploy
	5. Start war file
	6. Click on war file name
	7. Enter url pattern /test

<img width="792" height="1142" alt="image" src="https://github.com/user-attachments/assets/f7ac6c2b-28b7-4878-aeb8-4bec799606cd" />

