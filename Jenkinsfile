pipeline {

    agent any
    tools {
        maven 'M2'
    }
    stages {
        stage('Compile stage') {
            steps {
                 sh "mvn clean compile"
        }
    }
        
         stage('testing stage') {
             steps {
                
                sh "mvn test"
                 
        }
    }

          stage('deployment stage') {
              steps {
                 
                sh "mvn deploy"
                  
        }
    }

  }

}
