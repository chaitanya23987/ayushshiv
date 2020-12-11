pipeline {
    agent any
    environment {
        PATH = "/opt/maven/bin:$PATH"
    }        
    stages {
        stage("clone code"){
            steps{
                git branch: 'main', credentialsId: 'gitautomation', url: 'https://github.com/chaitanya23987/ayushshiv.git'
            }
        }
        stage("build code"){
            steps{
              sh "mvn clean install"
            }
        }
        
    } 
}
