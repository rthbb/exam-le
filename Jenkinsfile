pipeline {
 agent any
 stages {
   stage ('Build') {
     steps {
       echo 'Running building automation'
       sh './gradlew build --no-daemon'
       archieveArtifacts artifacts: 'dist/trainSchedule.zip'
     }
   }
 }
}
