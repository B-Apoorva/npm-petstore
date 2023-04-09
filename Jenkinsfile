pipeline{
agent any
  stages{
    stage("Git Chekout"){
      steps{
      https://github.com/B-Apoorva/npm-petstore.git
      }
    }
    stage("Build"){
      steps{
      sh 'mvn clean install package'
      }
    }
  }
}
