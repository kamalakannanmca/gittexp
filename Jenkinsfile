pipeline {
    agent any
    stages {
        stage('git') {
        steps {
         git 'https://github.com/pandian3k/Maven-Demo.git'       
        }
        }
        stage('installation') {
            steps {
                bat 'mvn install'
            }
        }
    
        stage('Deployment') {
            steps {
                sh 'cp -r "C:\\Program Files (x86)\\Jenkins\\workspace\\pushpa\\multi-module\\webapp\\target\\webapp.war" "C:\\Program Files\\Apache Software Foundation\\Tomcat 8.5_Tomcat8-devops\\webapps"'
            }
        }
    }
    
}

