pipeline{
  agent any
  stages{
   stage('Repo Checkout'){
     steps{
        checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Aravind0211/samplescm.git']])
      }
    }
    stage('Build'){
     steps{
       sh './gradlew build'
      }
    }
  }
}
