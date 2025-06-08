pipeline {
    agent any  // Use any available agent

    tools {
        gradle 'Gradle' 
        jdk 'JDK'
    }
    stages {
        stage('Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/varun0981/varungrad.git'
            }
        }

        stage('Build') {
            steps {
                sh 'gradle build'  
            }
        }

       stage('Test') {
           steps {
               sh 'gradle test'  
           }
        }

              
        stage('Run Application') {
            steps {
                sh 'gradle run'
            }
        }

        
    }
