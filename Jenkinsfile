pipeline {
  agent any
  stages {
    stage ('Build') {
      step {
        echo 'Build Stage'
        sh 'b./gradlew build --no-daemon'
        archiveArtifacts artifacts:'disr/trainSchedule.zip'
      }
    }
  }
}
