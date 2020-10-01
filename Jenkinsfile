pipeline {
  agent any
  stages {
    stage('Prepare') {
      steps {
        echo 'My first blue pipe!'
        sleep 5
        sh 'php -r "echo __DIR__;"'
      }
    }

  }
}