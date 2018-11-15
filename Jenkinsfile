pipeline {

    agent any
    stages {
        stage('Compile stage') {
            steps {
                Maven(maven : 'M2'){
                 sh "mvn clean compile"
                }
        }
    }
        
         stage('testing stage') {
             steps {
                 Maven(maven : 'M2'){
                sh "mvn test"
                 }
        }
    }

          stage('deployment stage') {
              steps {
                  Maven(maven : 'M2'){
                sh "mvn deploy"
                  }
        }
    }

  }

}
