pipeline {
    agent {
  label 'jenkins-master'
         }
   #agent  any

    stages {
        stage('checkout code from SCM') {
            steps {
                git branch: 'feature1', url: 'git@github.com:DevopsTraining-Harish/my-app.git'
            }
        }
        
        
        stage('test') {
            steps {
                echo 'test steps'
            }
        }
        
        
        stage('deploy') {
            steps {
                echo 'deploy steps'
            }
        }
    }
}
