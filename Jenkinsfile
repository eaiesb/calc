pipeline {
  agent any
  stages {
    stage('Unit Test') {
      steps {
        sh 'mvn clean test'
      }
    }  
    stage('Deploy CloudHub') {
      steps {
        sh 'mvn deploy -P cloudhub -Dmule.version=3.9.0 -Danypoint.username=kiran_padam123 -Danypoint.password=Eaiesb@123'
      }
    }
  }
}
