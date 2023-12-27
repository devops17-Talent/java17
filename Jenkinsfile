pipeline{
  agent any
  stages{
    stage('docker build'){
      sh 'docker build -t spring:v1 .'
  }
  stage('docker tagging'){
    sh 'docker tag spring:v1 malleshdevops/devopseks17:java-v1'
  }
 stage('docker login'){
   sh 'docker login'
 }
    stage('docker image push'){
    sh 'docker push malleshdevops/devopseks17:java-v1'
    }
}
}
