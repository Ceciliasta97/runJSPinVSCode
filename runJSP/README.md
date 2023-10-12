how to connect tomcat and vscode:
1. download apache tomcat file in your program
2. go to the extension page, install: "community server connector" and "extension pack for java", "Java Extension Pack", "Askia QeXML generator"(xml extension)
3. "Explorer" page: right click "Community Server Connector", click "create new server"
4. choose "no", choose file that you have download "apache-tomcat-9.0.81"
5. a new page of "new serevr: tomcat 9.x", click "finish"
6. connect to the apache-tomcat-9.0.41 in terminal: /home/yc97/Documents/Programs/o1heima/03-javaweb/csdnJSP/apache-tomcat-9.0.81/bin/startup.sh
7. download mvn in terminal: mvn archetype:generate -DgroupId=com.example -DartifactId=mywebapp -DarchetypeArtifactId=maven-archetype-webapp -DinteractiveMode=false
8. terminal shows "build success", and a new directory "mywebapp" is created automatically.
9.  "Server" -- "Community Server Connector" -- "Tomcat 9.x": right click and choose "add deployment" -- "File", choose the mywebapp/pom.xml file.
10. page "Run and Debug" : click "Run and Debug" (it might notice you to find XML Extension, install it)
11. after install xml extension, back to page "Run and Debug", click "Run and "Debug" again
12. the page shows "select debugger", select "webapp(chrome)" or "webapp"(Edge)"
13. vscode jump to a new page "launch.json", click the button "add configuration"
14. "add configuration" -- choose "{}chrome: Attach" (first one)
15. create a directory webapp (/createjsp/webapp), create your own .jsp file
16. for example, create a hello.jsp file under directory "webapp"
17. copy the file "hello.jsp" to /apache-tomcat-9.0.81/webapps/ROOT/, under ROOT directory
18. click menu "Run" -- "Run without Debugging"
19. a new chrome page is shown, with the address: http://localhost:8080/
20. as we create a "hello.jsp" under ROOT direcotry, type "http://localhost:8080/hello.jsp" in web browser, it will show sth.
tips: the .jsp file must running under "apache-tomcat-9.0.81/webapps/ROOT" directory
tips: remember to start server before running .jsp file