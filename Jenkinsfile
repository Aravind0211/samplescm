pipeline{
  agent any
  stages{
   stage('Repo Checkout'){
     steps{
        checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Aravind0211/samplescm.git']])
      }
    }
    stage('Build'){
      tools{
        jdk 'java-8'
      }
     steps{
       sh './gradlew build'
      }
    }
  }
}
