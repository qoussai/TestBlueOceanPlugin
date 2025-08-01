pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build complate'
      }
    }

    stage('TestStages') {
      parallel {
        stage('Test0') {
          steps {
            echo 'test1 complated succe'
          }
        }

        stage('test1') {
          steps {
            echo 'all test complated'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'complated Deploy for app'
      }
    }

  }
}