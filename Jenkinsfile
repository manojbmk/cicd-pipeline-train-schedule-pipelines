pipeline{
  agent any
  stages {
    stage("Build")
    {
      steps {
        echo "building repo"
        sh ./gradlew build --no-daemon
        archieveArtifacts artifacts: "dist/trainSchedule.zip"
      }   
  }
 }
} 
