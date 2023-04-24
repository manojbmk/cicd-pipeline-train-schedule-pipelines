pipeline{
  agent any
  stages {
    stage("Build")
    {
      steps {
        echo "build repo"
        sh ./gradlew build --no-daemon
        archieveArtifacts artifacts: "dist/trainSchedule.zip"
      }   
  }
 }
} 
