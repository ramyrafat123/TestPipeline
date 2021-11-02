pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            git 'https://github.com/executeautomation/cucumberbasic.git'
          }
        }

        stage('Test') {
          steps {
            bat 'mvn test'
          }
        }

      }
    }

  }
}