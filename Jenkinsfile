node {
    stage ('SCM checkout'){
      git 'https://github.com/sreekar0624/my-app'
    }
    stage ("Maven Build"){
        def mvnHome = tool name: 'Maven3', type: 'maven'
        sh "${mvnHome}/bin/mvn package"
      }
  }

   
