pipeline {
    agent {
  label 'jenkins-master'
         }
 
    stages {
        stage('Compile') {
            steps {
		powershell 'mvn compile'
            }
        }
        
        
        stage('Junit') {
            steps {
		bat 'mvn test'
                  }
        }
        
        
        stage('deploy') {
            steps {
                echo 'deploy steps'
            }
        }
    }
}
