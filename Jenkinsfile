pipeline {
  agent any
  stages {
    stage("Build") {
      steps {
        build "PES2UG21CS905-1"
        sh "g++ main.cpp -o output"
      }
    }
    stage("Test") {
      steps {
        sh "./hehe"
      }
    }
    stage("Deploy") {
      steps {
        echo "deploy"
      }
    }
  }
  post {
    failure {
      error "Pipeline failed"
    }
  }
}
