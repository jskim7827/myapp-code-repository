pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building....'
      }
    }
    stage('Test Firefox') {
      parallel {
        stage('Test Firefox') {
          steps {
            sh 'echo \'firefox\''
          }
        }
        stage('test chrome') {
          steps {
            sh 'echo \'test chrome\''
          }
        }
        stage('test ie') {
          steps {
            sh 'echo \'dl\''
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }
  }
}