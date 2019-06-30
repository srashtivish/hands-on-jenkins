pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building'
      }
    }
    stage('Test firefox') {
      parallel {
        stage('Test firefox') {
          steps {
            sh 'echo "TEST Fzirelkjl"'
          }
        }
        stage('Test Chrome') {
          steps {
            sh 'echo "Test chrome"'
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