pipeline {
    agent any

    tools {
	maven 'maven'
      
    }

    stages {
        stage('code clone') {
            steps {
			git branch: 'main', credentialsId: 'github', url: 'https://github.com/suryavinay4435/mvnpro.git'
                
            }
            }
			stage('code clean') {
            steps {
			sh 'mvn clean'
                
            }
            }
			stage('code validate') {
            steps {
			sh 'mvn validate'
                
            }
            }
			stage('code compile') {
            steps {
			sh 'mvn compile'
                
            }
            }
			stage('code test') {
            steps {
			sh 'mvn test'
                
            }
            }
			stage('code package') {
            steps {
			sh 'mvn package'
                
            }
            }
			stage('code deploy') {
            steps {
			sh 'mvn deploy'
                
            }
            }
         }
      }