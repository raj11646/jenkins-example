pipeline {

    agent any
    stages {
        stage('Compile stage') {
            steps {
                maven(name : 'M2'){
                 sh "mvn clean compile"
                }
        }
    }
        
         stage('testing stage') {
             steps {
                 maven(name : 'M2'){
                sh "mvn test"
                 }
        }
    }

          stage('deployment stage') {
              steps {
                  maven(name : 'M2'){
                sh "mvn deploy"
                  }
        }
    }

  }

}
