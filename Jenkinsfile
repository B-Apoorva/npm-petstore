pipeline{
agent any
  tools {
    nodejs "NodeJS 19.9.0"
}
  stages{
    stage('Git Chekout'){
      steps{
        git credentialsId: 'ba0f45f0-7b2b-4c7f-b804-5a843cd4a163', url: 'https://github.com/B-Apoorva/npm-petstore.git'
      }
    }
    stage('Install Dependencies'){
      steps{
      sh 'npm install'
      }
    }
    stage('Build'){
      steps{
      sh 'npm cit'
      }
    }
    stage('Test'){
      steps{
      sh 'node test'
      }
    }
  }
}
