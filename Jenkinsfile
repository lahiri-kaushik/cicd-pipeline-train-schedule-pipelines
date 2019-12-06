pipeline{
  agent any
  stages{
    stage ('Build'){
      steps{
        echo 'Running build automation'
        sh './gradle build --no-domain'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
