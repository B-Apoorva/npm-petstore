pipeline{
agent any
  stages{
    stage(Get Code){
      steps{
      https://github.com/B-Apoorva/npm-petstore.git
      }
    }
    stage(build){
      steps{
      sh'mvn clean install package'
      }
    }
  }
}
