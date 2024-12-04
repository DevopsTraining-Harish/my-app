pipeline {
    agent {
  label 'jenkins-master'
         }
 
    stages {
        stage('Compile') {
            steps {
		sh 'mvn compile'
            }
        }
        
        
        stage('Junit') {
            steps {
			sh 'mvn test'
                  }
        }
        
        
        stage('deploy') {
            steps {
                echo 'deploy steps'
            }
        }
    }
}
