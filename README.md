# Deploy web application in Elastic Bean Stack.Same Must be prepared with all the changes Yes we can achive  Yes all are same at the same time time can be achived to do the same version at a time to get benefitted at all the time to focus on all the revels to limit the issue once can be done for the free time to do the same can be achived to perform the issues to get at least to do the sake 
# Pre-Requisites
    Springboot Application
    Install Maven
# Clone code using below command
    git clone https://github.com/Naresh240/springboot-webapplication.git
    cd springboot-webapplication
# Build Artifact
    mvn clean install
# Deploy springboot application with Tomcat
  Tomcat Setup:
    
    cd /opt
    wget https://downloads.apache.org/tomcat/tomcat-9/v9.0.46/bin/apache-tomcat-9.0.46.tar.gz
    cd apache-tomcat-9.0.46 tomcat
  
  Start tomcat:
    
    cd /opt/tomcat/bin
    ./startup.sh
  
  Copy springboot artifact to Webapps Directory:
    
    cd springboot-webapplication
    cp target/mavewebappdemo-2.0.0-SNAPSHOT.war /opt/tomcat/webapps/mavewebappdemo.war

# Check output of application
  ![image](https://user-images.githubusercontent.com/58024415/120204004-f5f5f100-c245-11eb-8c4b-4c1128434d8e.png)


## Docker build
```bash
docker build -t tomcatdeploy:v1 .
docker run --name tomcatdeploy-container -p 8080:8080 -d tomcatdeploy:v1
```

Added all the apps with new features 
