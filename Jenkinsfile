pipeline {

  agent any

    stages {
      stage('build'){
        steps{
          sh 'ant -f build.xml -v'
        }
      }
    }
    post {
      always {
        archiveArtifacts '/var/lib/jenkins/workspace/MyJavaProject/dist/rectangle.jar'
      }
    }
  }
