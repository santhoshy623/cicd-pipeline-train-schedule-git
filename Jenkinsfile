pipeline {
  agent any
  stages {
    stage {"build"} {
      steps {
        echo "running build automation"
        sh './gredflow build --no-demon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
