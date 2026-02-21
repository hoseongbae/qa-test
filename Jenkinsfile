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
      archiveArtifacts artifacts: 'GameQA실습파일/newman/*.*', fingerprint: true
    }
  }
}
