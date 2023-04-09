pipeline{
agent any
  tools {
    nodejs "nodejs-10.0.0"
}
  stages{
    stage('Git Chekout'){
      steps{
      git credentialsId: 'bacf9471-7e4e-424f-91a8-6109e11e5e4a', url: 'https://github.com/B-Apoorva/npm-petstore.git'
      }
    }
    stage('Build'){
      steps{
      sh 'mvn clean install package'
      }
    }
  }
}
