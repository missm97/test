pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'building the application'
        echo 'building the application'
      }
    }

    stage('Test') {
      steps {
        echo 'Testing the application'
      }
    }

    stage('deploy') {
      steps {
        echo 'deploying the application'
        sh 'sshagent([\'ssh\']) {ec2-user@54.152.85.133}'
      }
    }

  }
  environment {
    maven = '3.8.6'
  }
}