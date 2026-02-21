pipeline {
  agent any

  stages {
    stage('Test') {
      steps {
        echo 'Hello Jenkins'
      }
    }
  }

  post {
    always {
      archiveArtifacts artifacts: '*.html, *.json, *.xml', fingerprint: true
    }
  }
}
