pipeline {
    agent any
    stages {
        stage ("SCM") {
            steps {
                git branch: 'main', 
                credentialsId: 'gitlab', 
                url: 'https://github.com/raviu2500/Webapps.git'
            }
        }
        stage("Build") {
            steps {
                sh "mvn clean install"
            }
        }
        stage("Deploy") {
            steps {
                 sh "sudo cp ./target/*.war /opt/apache-tomcat-10.1.8/webapps/springboot2.war"
            }
        }
    }
}
