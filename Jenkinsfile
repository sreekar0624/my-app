pipeline {
  agent any
  stages{
    stage ('SCM checkout'){
      git 'https://github.com/sreekar0624/my-app'
    }
    stage("Maven Build"){
      steps{
        def mvnHome = tool name: 'Maven3', type: 'maven'
        sh "${mvnHome}/bin/mvn package"
      }
    }
  }
}
   
