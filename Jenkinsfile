pipeline{
  agent any
  stages{
    stage('docker build'){
      steps{
      sh 'docker build -t spring:v1 .'
      }
  }
  stage('docker tagging'){
    steps{
    sh 'docker tag spring:v1 malleshdevops/devopseks17:java-v1'
    }
  }
 stage('docker login'){
   steps{
   sh 'docker login'
   }
 }
    stage('docker image push'){
      steps{
    sh 'docker push malleshdevops/devopseks17:java-v1'
    }
    }
}
}
