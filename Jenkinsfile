pipeline {
    agent any
    stages {
        stage('build') {
            steps {
              echo "buildapp"        
            }
        }
       stage('test') {
            steps {
               echo "testapp"
            }
            }

        post
            {
            always 
            {
               emailext body: 'New Python code deployed ', subject: 'Hello Build run Successfully', to: 'kksahay04@gmail.com'
            }
            } 
            }
        }