pipeline {

    agent any
    stages {
        stage('Compile stage') {
            steps {
                WithMaven(maven : 'M2'){
                 sh "mvn clean compile"
                }
        }
    }
        
         stage('testing stage') {
             steps {
                 WithMaven(maven : 'M2'){
                sh "mvn test"
                 }
        }
    }

          stage('deployment stage') {
              steps {
                  WthMaven(maven : 'M2'){
                sh "mvn deploy"
                  }
        }
    }

  }

}
