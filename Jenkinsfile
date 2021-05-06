pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'Starting Build Job'
        sh 'npm install'
      }
    }

    stage('test') {
      steps {
        echo 'Starting Test Job'
        sh 'npm test'
      }
    }

    stage('package') {
      steps {
        echo 'Starting Package Job'
        sh 'npm run package'
      }
    }

  }
  tools {
    nodejs 'nodejs'
  }
  post {
    always {
      echo 'this pipeline is for shopping portal...'
    }

  }
}