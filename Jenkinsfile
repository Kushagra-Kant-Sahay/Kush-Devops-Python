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
            
            post {
                always
                {
                    mail bcc: '', body: '$DEFAULT_CONTENT', cc: 'kksahay04@gmail.com', from: 'trickygyan818@gmail.com', replyTo: '', subject: 'Pipebuild Successfully', to: 'diksha1999tripathi@gmail.com'
                }
            }
        }
