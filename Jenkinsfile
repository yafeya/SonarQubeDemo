pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''cd ./OpenCppCoverageDemo/cmake
./build.sh'''
        sh '''cd ./OpenCppCoverageDemo/cmake/x64/debug
make'''
      }
    }
  }
}