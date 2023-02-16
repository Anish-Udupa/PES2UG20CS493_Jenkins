pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'g++ -o hello hello.cpp'
        echo 'build successful'
      }
    }
    stage('Test') {
      steps {
        sh './helloe'
      }
    }
  }
  post {
    always {
      echo 'Pipeline completed'
    }
    failure {
      echo 'Failure'
    }
  }
}
