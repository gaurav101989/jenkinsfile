pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'date'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test case'
          }
        }

        stage('par') {
          steps {
            echo 'run par'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy success'
        sleep 10
      }
    }

  }
}
