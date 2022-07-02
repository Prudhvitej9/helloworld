pipeline {
  agent { label 'master' }

  tools {
    maven 'maven3'
  }
  
  stages {
    stage('Git checkout'){
      steps {
        git branch: 'develop',
        url: 'https://github.com/chinni4321/helloworld.git'
      }
    }
    stage('Maven build'){
      steps {
        sh 'mvn clean install'
      }
    }

 }
}
