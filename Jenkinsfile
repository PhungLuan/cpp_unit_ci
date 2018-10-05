pipeline {
  agent any
  triggers { pollSCM('*/1 * * * *') }
  stages {
    stage('make') {
      steps {
        sh '''g++ -o testBasicMath CBasicMath.cpp TestBasicMath.cpp -lcppunit
./testBasicMath'''
      }
    }
  }
}
