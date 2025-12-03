pipeline {
    agent any
    
    stages {
      
      stage('clone project') {
            steps {
                      git branch:'main',url:'https://github.com/tsarjun/b7-java.git'  
              }
      }

      stage('clean') {
            steps {
                      sh 'mvn clean'
              }
      }

      stage('compile') {
            steps {
                      sh 'mvn compile'
              }
      }

      stage('test') {
            steps {
                      sh 'mvn test'
              }
      }

      stage('build') {
            steps {
                      sh 'mvn clean install'
              }
      }


    }
}
