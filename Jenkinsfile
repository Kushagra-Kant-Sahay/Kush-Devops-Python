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
        stage('deploy') {
            steps{
                echo "deployapp"
            }
        }
    }

        Post{
            build {
                    emailext body: 'New Python code deployed ', subject: 'Hello Build run Successfully', to: 'kksahay04@gmail.com'
            }
        }
        }
