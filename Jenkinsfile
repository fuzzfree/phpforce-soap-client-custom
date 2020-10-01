pipeline {
  agent any
  stages {
    stage('Prepare') {
      environment {
        eee111 = '111'
        eee222 = '222'
      }
      steps {
        echo 'My first blue pipe!'
        sleep 5
        sh 'php -r "echo __DIR__;"'
      }
    }

    stage('Repo') {
      environment {
        eee333 = '333'
      }
      steps {
        sh 'mkdir -p _BUILD && cd _BUILD/ &&  git clone https://github.com/composer/ca-bundle.git --depth=1 _BUILD/'
      }
    }

  }
}