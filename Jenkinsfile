pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'g++ -o PES2UG20CS386-1 ./main/hello.cpp'
        echo 'Build Successful'
      }
    }
    stage('Test') {
      steps {
        sh './PES2UG20CS386-2'
        echo 'Test Successful'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Successfully Deployed'
      }
    }
  }
  post {
    failure{
      echo 'Pipeline Failed Unfortunately!! :( '
    }
  }
}
