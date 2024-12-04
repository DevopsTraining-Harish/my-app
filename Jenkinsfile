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
		powershell 'mvn compile'
                  }
        }
        
        
        stage('deploy') {
            steps {
                echo 'deploy steps'
            }
        }
    }
}
