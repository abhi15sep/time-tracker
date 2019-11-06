pipeline {
   agent any
   tools {
    maven 'M3'
  }
    
   stages {
      stage('Build') {
         steps {
            sh "mvn clean -f time-tracker"
         }
      }
      stage('Test') {
         steps {
            sh "mvn test -f time-tracker"
         }
      }
      stage('Deploy') {
         steps {
            sh "mvn package -f time-tracker"
         }
      }
   }
}
