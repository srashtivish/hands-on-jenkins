pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building'
      }
    }
    stage('Test') {
      parallel {
        stage('Test firefox') {
          steps {
            sh 'echo "TEST Firefox"'
          }
        }
        stage('Test Chrome') {
          steps {
            sh 'echo "Test chrome"; exit 1'
          }
        }
        stage('Test Edge') {
          steps {
            sh 'echo "test edge"'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying'
      }
    }
  }
}
