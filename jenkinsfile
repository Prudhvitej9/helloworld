pipeline {
  agent { label 'master' }

  tools {
    jdk 'Java8'
    maven 'Maven3.3.9'
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
