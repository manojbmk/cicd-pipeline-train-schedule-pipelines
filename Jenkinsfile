pipeline{
  agent any
  stages {
    stage("Build")
    {
      steps {
        echo "building repo"
        sh './gradlew build --no-daemon'
      }   
    }
    stage("archieve")
    {
      steps {
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
 }
} 
