pipeline {
 agent any
  stages {
    stage ('Build') {
      step {
        echo 'Running build automation'
        sh './gradlew build --no daemon'
        archiveArtifacts artifacts: 'dist/trainschedule.zip'
      }
    }
  }
}
