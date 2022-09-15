pipeline {
  agent any
  stages {
    stage('Checkout code') {
     checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: '95d8a82d-a7c4-48c9-bfb0-f924f0eb255d', url: 'https://github.com/rutuja2810/Sonardemo.git']]])
        stage('Build') {
          steps {
            echo 'Hello'
          }
        }
        stage('Test') {
          steps {
            pwd(tmp: true)
          }
        }

      }
    }

  
}
