pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveSrtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }    
  }
}
