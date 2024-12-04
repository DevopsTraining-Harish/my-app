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
        stage('Package') {
            steps {
		bat 'mvn -DskipTests clean package'
                  }
        }

        stage('Upload package into Nexus') {
            steps {
		bat 'mvn -DskipTests deploy'
                  }
        }        
        stage('Cleanup Workspace') {
            steps {
                cleanWs()
            }
        }
    }
}
