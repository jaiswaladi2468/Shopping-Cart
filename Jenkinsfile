pipeline {
    agent any
    tools {
      jdk 'jdk17'
      maven 'maven3'
        
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
