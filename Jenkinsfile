pipeline {

    agent any
    
    stages {
         stage('install') {
          steps {
              sh 'npm install'
            }
          }
          stage('build') {
          steps {
              sh 'npm run build'
            }
          }
        
        stage('test') {
          steps {
              sh 'npm test'
            }
          }
        
        stage('Docker Comopse Up') {
            steps {
               
                    sh "docker compose up"
                
            }
        }
    }
}