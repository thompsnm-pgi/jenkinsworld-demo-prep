pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building'
      }
    }
    stage('Test') {
      steps {
        parallel(
          "Test 1": {
            echo 'Test suite 1'
            
          },
          "Test 2": {
            echo 'Test suite 2'
            
          }
        )
      }
    }
    stage('Release') {
      steps {
        echo 'Release'
      }
    }
  }
}