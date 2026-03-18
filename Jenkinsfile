
pipeline{
    agent any
    environment{
        TOMCAT_USER="ec2-user"
        TOMCAT_IP="172.31.11.38"
    }
    stages{
        stage("Code Checkout"){
            steps{
                git 'https://github.com/andynzeka/my-app'
            }
        }
        stage("Maven Build"){
            steps{
                sh 'mvn clean package'
            }
        }
    }
}
