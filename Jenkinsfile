pipeline {
    agent {
  label 'jenkins-master'
         }
 
    stages {
        stage('Compile') {
            steps {
		mvn compile
            }
        }
        
        
        stage('Junit') {
            steps {

		mvn test
                  }
        }
        
        
        stage('deploy') {
            steps {
                echo 'deploy steps'
            }
        }
    }
}
