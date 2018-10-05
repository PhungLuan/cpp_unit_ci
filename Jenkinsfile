pipeline {
  agent any
  stages {
    stage('make') {
      steps {
        sh '''g++ -o testBasicMath CBasicMath.cpp TestBasicMath.cpp -lcppunit
./testBasicMath'''
      }
    }
  }
}