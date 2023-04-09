pipeline{
agent any
  tools {
    nodejs "nodejs-10.0.0"
}
  stages{
    stage('Git Chekout'){
      steps{
      git credentialsId: '562435e9-a8b4-4856-98be-f55860c39eea', url: 'https://github.com/B-Apoorva/npm-petstore.git'
      }
    }
    stage('Build'){
      steps{
      sh 'mvn clean install package'
      }
    }
  }
}
