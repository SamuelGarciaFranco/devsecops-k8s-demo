pipeline {
  agent any

  stages {
      stage('Build Artifact - Maven') {
            steps {
              sh "mvn clean package -DskipTests=true"
              archive 'target/*.jar'
            }
        }   
      stage('Unit Test') {
            steps { 
              sh "mvn test" /*Comment22*/
       
            }
        }   
    }
}