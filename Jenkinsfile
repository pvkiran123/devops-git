pipeline {
  agent any
  
  stages{
    stage("Maven Build"){
      steps{
        sh "mvn clean package"
      }
    }
  }
    stages{
    stage("deploy to tomcat"){
      steps{
        sh "coming soon"
      }
    }
   }
  post{
      success{
        archiveArtifacts artifacts: 'target/*.war'
        cleanWs()
      }
    }
  }
