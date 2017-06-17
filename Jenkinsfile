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
        archiveArtifacts allowEmptyArchive: true, artifacts:'/var/lib/jenkins/workspace/MyJavaProject/dist/rectangle.jar'
      }
    }
  }
