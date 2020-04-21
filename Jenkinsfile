pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Build Stage'
        sh 'b./gradlew build --no-daemon'
        archiveArtifacts artifacts:'disr/trainSchedule.zip'
      }
    }
  }
}
