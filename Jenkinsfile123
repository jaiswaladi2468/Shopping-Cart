pipeline {
    agent any
  
    stages {
        stage('Git Checkout') {
            steps {
              git branch: 'feature', url: 'https://github.com/advikpadhye/Shopping-Cart-new.git'
            }
        }
        
        stage('Compile the Code') {
            steps {
              sh "mvn clean compile"
            }
        }
        
        stage('test the Code') {
            steps {
              sh "mvn clean test"
            }
        }
        
        
        stage('package the Code') {
            steps {
              sh "mvn clean package"
            }
        }
        
    }
}
